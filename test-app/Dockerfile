# test-app/Dockerfile

FROM alpine:3.19

LABEL maintainer="ci-test"
LABEL description="Simple test image for GitHub Actions multi-arch build"

RUN echo "Building on $(uname -m)"

CMD ["sh", "-c", "echo Hello from $(uname -m) && sleep 3600"]