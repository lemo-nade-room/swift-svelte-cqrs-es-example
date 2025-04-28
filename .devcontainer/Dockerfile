FROM mcr.microsoft.com/devcontainers/javascript-node:20-bookworm

RUN apt-get update \
 && apt-get install -y --no-install-recommends curl git ca-certificates \
 && rm -rf /var/lib/apt/lists/*

RUN curl -fsSL https://bun.sh/install | bash \
 && cp /root/.bun/bin/bun /usr/local/bin/ \
 && ln -s /usr/local/bin/bun /usr/local/bin/bunx \
 && chmod +x /usr/local/bin/bun \
 && rm -rf /root/.bun
