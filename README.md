# Nextjs Docker

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

## Version 7
##### Node and package manager
- Node: 8
- npm
- yarn

##### NPMs versions
- next: ~7.0.3
- next-routes: ~1.4.2
- react: ~16.8.4
- react-dom: ~16.8.4
- @zeit/next-css: ~1.0.1
