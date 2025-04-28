FROM mcr.microsoft.com/devcontainers/javascript-node:20-bookworm

RUN apt-get update && apt-get install -y --no-install-recommends curl git ca-certificates && \
    rm -rf /var/lib/apt/lists/*

RUN curl -fsSL https://bun.sh/install | bash \
 && mv /root/.bun/bin/bun  /usr/local/bin/ \
 && mv /root/.bun/bin/bunx /usr/local/bin/ \
 && chmod +x /usr/local/bin/bun /usr/local/bin/bunx \
 && rm -rf /root/.bun
