# stunnel for the deadend tls-terminator sidecar (profile-plugin-deadend).
# Built once with the package baked in, so the sidecar never installs
# anything at start-up: airgapped clusters have no internet egress.
FROM alpine:3.22.6@sha256:5291449c3df73caf6ed85e649dec1b9e818b39a5d8c871e97afc13e9cd5e8fa8
RUN apk add --no-cache stunnel=5.75-r0
CMD ["stunnel", "/etc/stunnel/stunnel.conf"]
