# caddy-docker-proxy-cloudflare
caddy-docker-proxy with support for Cloudflare DNS verification

docker buildx create --platform linux/arm64,linux/amd64 --use

Update CADDY_VERSION in Dockerfile
docker buildx build --platform linux/amd64,linux/arm64 --push -t theraapster/caddy-proxy-cloudflare:latest -t theraapster/caddy-proxy-cloudflare:2.7.6 .

# docker build -t theraapster/caddy-proxy-cloudflare:latest -t theraapster/caddy-proxy-cloudflare:2.7.6 .
docker push theraapster/caddy-proxy-cloudflare
docker push theraapster/caddy-proxy-cloudflare:2.7.6