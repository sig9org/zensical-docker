# Docker image of Zensical

This is [Zensical](https://zensical.org/) as a Docker container image.

## How to build

### Latest

```sh
docker buildx build \
    --platform linux/amd64,linux/arm64 \
    --output=type=registry \
    --tag sig9/zensical:latest \
    versions/0.0.12/
```

### 0.0.11

```sh
docker buildx build \
    --platform linux/amd64,linux/arm64 \
    --output=type=registry \
    --tag sig9/zensical:0.0.12 \
    versions/0.0.12/
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

## Releases

- [0.0.12](https://github.com/zensical/zensical/releases/tag/v0.0.12) (2025/12/18)
- [0.0.11](https://github.com/zensical/zensical/releases/tag/v0.0.11) (2025/12/03)
- [0.0.10](https://github.com/zensical/zensical/releases/tag/v0.0.10) (2025/11/26)
- [0.0.9](https://github.com/zensical/zensical/releases/tag/v0.0.9) (2025/11/20)
- [0.0.8](https://github.com/zensical/zensical/releases/tag/v0.0.8) (2025/11/15)
- [0.0.7](https://github.com/zensical/zensical/releases/tag/v0.0.7) (2025/11/13)
- [0.0.6](https://github.com/zensical/zensical/releases/tag/v0.0.6) (2025/11/12)
- [0.0.5](https://github.com/zensical/zensical/releases/tag/v0.0.5) (2025/11/08)
- [0.0.4](https://github.com/zensical/zensical/releases/tag/v0.0.4) (2025/11/06)
- [0.0.3](https://github.com/zensical/zensical/releases/tag/v0.0.3) (2025/11/05)
