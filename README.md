# Docker image of Zensical

This is [Zensical](https://zensical.org/) as a Docker container image.

## How to build

### Latest

```sh
docker buildx build \
    --platform linux/amd64,linux/arm64 \
    --output=type=registry \
    --tag sig9/zensical:latest \
    versions/0.0.11/
```

### 0.0.11

```sh
docker buildx build \
    --platform linux/amd64,linux/arm64 \
    --output=type=registry \
    --tag sig9/zensical:0.0.11 \
    versions/0.0.11/
```

## References

- Official
    - [Zensical](https://zensical.org/)
    - [Zensical Documentation](https://zensical.org/docs/get-started/)
    - [Backlog](https://github.com/orgs/zensical/projects/2/views/1)
    - [GitHub](https://github.com/zensical/zensical)
- Unofficial
    - DockerHub
        - [sig9/zensical](https://hub.docker.com/r/sig9/zensical)
    - GitHub
        - [Docker image of Zensical](https://github.com/sig9org/zensical-docker)
        - [Template for Zensical](https://github.com/sig9org/zensical-template)
