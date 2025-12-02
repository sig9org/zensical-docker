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

## References

- [Zensical](https://zensical.org/)
- GitHub
    - [Zensical documentation](https://github.com/zensical/docs)
    - [Docker image of Zensical](https://github.com/sig9org/zensical-docker)
    - [Template for Zensical](https://github.com/sig9org/zensical-template)
- DockerHub
    - [sig9/zensical](https://hub.docker.com/r/sig9/zensical)
