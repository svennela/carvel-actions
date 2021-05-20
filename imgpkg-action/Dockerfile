#FROM debian:9.5-slim
FROM alpine:latest
# installs required packages for our script
RUN apk add --no-cache \
  bash \
  ca-certificates \
  curl \
  jq

ADD entrypoint.sh /entrypoint.sh
RUN chmod +x /entrypoint.sh
ENTRYPOINT ["/entrypoint.sh"]