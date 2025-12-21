# Docker image of Zensical

This is [Zensical](https://zensical.org/) as a Docker container image.

## How to Use

```sh
docker run --rm -v ${PWD}:/docs sig9/zensical:0.0.14 zensical build --clean
```

## DockerHub Supported tags

- [0.0.14](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.14/)
- [0.0.13](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.13/)
- [0.0.12](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.12/)
- [0.0.11](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.11/)
- [0.0.10](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.10/)
- [0.0.9](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.9/)
- [0.0.8](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.8/)
- [0.0.7](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.7/)
- [0.0.6](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.6/)
- [0.0.5](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.5/)
- [0.0.4](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.4/)
- [0.0.3](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.3/)
- [0.0.2](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.2/)
- [0.0.1](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.1/)
- [0.0.0](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.0/)

## Example CI/CD Configuration for GitLab Pages (.gitlab-ci.yml)

```yaml
stages:
  - build

build-job:
  stage: build
  script:
    - docker run --user $(id -u):$(id -g) --rm -v ${PWD}:/docs sig9/zensical:0.0.14 zensical build --clean
    - rm -rf /var/www/html/*
    - cp -R site/* /var/www/html/
```

## How to Build a Docker Container Image

### Latest

```sh
docker buildx build \
    --platform linux/amd64,linux/arm64 \
    --output=type=registry \
    --tag sig9/zensical:latest \
    versions/0.0.14/
```

### 0.0.14

```sh
docker buildx build \
    --platform linux/amd64,linux/arm64 \
    --output=type=registry \
    --tag sig9/zensical:0.0.14 \
    versions/0.0.14/
```

## References

- Official
    - [Zensical](https://zensical.org/)
    - [Zensical Documentation](https://zensical.org/docs/get-started/)
    - [Backlog](https://github.com/orgs/zensical/projects/2/views/1)
    - [GitHub](https://github.com/zensical/zensical)
    - [PyPi](https://pypi.org/project/zensical/) ([History](https://pypi.org/project/zensical/#history))
    - [DockerHub](https://hub.docker.com/r/zensical/zensical)
- Unofficial
    - DockerHub
        - [sig9/zensical](https://hub.docker.com/r/sig9/zensical)
    - GitHub
        - [Docker image of Zensical](https://github.com/sig9org/zensical-docker)
        - [Template for Zensical](https://github.com/sig9org/zensical-template)

## Releases

- [0.0.14](https://github.com/zensical/zensical/releases/tag/v0.0.14) (2025/12/22)
- [0.0.13](https://github.com/zensical/zensical/releases/tag/v0.0.13) (2025/12/19)
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
