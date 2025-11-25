# Docker image of Zensical

This is [Zensical](https://zensical.org/) as a Docker container image.

## How to build

### Latest

```sh
docker buildx build \
    --platform linux/amd64,linux/arm64 \
    --output=type=registry \
    --tag sig9/zensical:latest \
    versions/0.0.10/
```

### 0.0.10

```sh
docker buildx build \
    --platform linux/amd64,linux/arm64 \
    --output=type=registry \
    --tag sig9/zensical:0.0.10 \
    versions/0.0.10/
```
