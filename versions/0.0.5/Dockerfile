# Build Stage
FROM python:3.14.2-slim AS builder

# Environment variables
ENV PACKAGES=/usr/local/lib/python3.14/site-packages
ENV PYTHONDONTWRITEBYTECODE=1

# Set build directory
WORKDIR /build

# Perform build and cleanup artifacts and caches
RUN apt-get update && apt-get install -y \
    gcc \
    g++ \
    tini \
    && rm -rf /var/lib/apt/lists/*

RUN pip install --no-cache-dir --upgrade pip && \
    pip install --no-cache-dir \
        click==8.3.1 \
        deepmerge==2.0 \
        markdown==3.10 \
        pygments==2.19.2 \
        pymdown-extensions==10.19.1 \
        pyyaml==6.0.3 \
        zensical==0.0.5

RUN find . -type d -name "__pycache__" -exec rm -rf {} + 2>/dev/null || true && \
    find . -type f -name "*.pyc" -delete && \
    rm -rf venv/ && \
    rm -rf .git/ && \
    rm -rf .pytest_cache/ && \
    rm -rf *.egg-info/ && \
    rm -rf .coverage && \
    rm -rf htmlcov/

# Runtime Stage
FROM python:3.14.2-slim AS runtime

# Copy all from builder
COPY --from=builder /usr/local/lib/python3.14/site-packages /usr/local/lib/python3.14/site-packages
COPY --from=builder /usr/local/bin /usr/local/bin
COPY --from=builder /usr/bin/tini /usr/bin/tini

# Set working directory
WORKDIR /docs

# Expose MkDocs development server port
EXPOSE 8000

# Shell
CMD ["/bin/sh"]