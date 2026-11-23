# stunnel for the deadend tls-terminator sidecar (profile-plugin-deadend).
# Built once with the package baked in, so the sidecar never installs
# anything at start-up: airgapped clusters have no internet egress.
FROM alpine:3.24.4@sha256:f59abe656b692d901e184be3445e084786602108599d2a51d229c0f5a48c71bf
RUN apk add --no-cache stunnel=5.75-r0
CMD ["stunnel", "/etc/stunnel/stunnel.conf"]
