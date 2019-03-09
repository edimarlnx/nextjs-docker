# nextjs-docker

Usage example

```dockerfile
FROM edimarlnx/nextjs-docker:7

ENV API_URL ${API_URL:+"http://localhost:8080"}
COPY .next /app/.next
COPY static /app/static
COPY server /app/server
COPY package.json /app/package.json
COPY next.config.js /app/next.config.js

RUN yarn install --production
```
