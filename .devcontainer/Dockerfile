FROM node@sha256:5c4012d11d9857c42713ba511fbc19645cac1706bb710d51d42b0d301dff7f88
RUN npx -y playwright@1.64.1 install-deps chromium \
 && npm install -g pnpm@11.19.0 \
 && rm -rf /var/lib/apt/lists/* \
 && npm cache clean --force
USER node