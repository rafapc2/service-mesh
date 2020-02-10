FROM consul:1.5.1

FROM envoyproxy/envoy:v1.10.0
COPY --from=0 /bin/consul /bin/consul
ENTRYPOINT ["dumb-init", "consul", "connect", "envoy"]