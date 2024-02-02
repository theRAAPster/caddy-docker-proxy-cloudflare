# caddy-docker-proxy-cloudflare

caddy-docker-proxy with support for Cloudflare DNS verification.

Build new version steps:

1.

``` shell
docker buildx create --platform linux/arm64,linux/amd64 --use
```

1.

Update CADDY_VERSION in Dockerfile

1.

``` shell
docker buildx build --platform linux/amd64,linux/arm64 --push -t theraapster/caddy-proxy-cloudflare:latest -t theraapster/caddy-proxy-cloudflare:2.7.6 .
```
