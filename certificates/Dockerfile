## IMAGEM FINAL ##
# certificates
# - construído em inure-base, porém com ca-certificados já instalados.

ARG CI_REGISTRY_IMAGE="registry.inure.com/inure-org/build/cng"
ARG TAG="master"
ARG INURE_BASE_IMAGE="${CI_REGISTRY_IMAGE}/inure-base:${TAG}"

FROM --platform=${TARGETPLATFORM} $INURE_BASE_IMAGE

COPY scripts/bundle-certificates /scripts/

VOLUME /etc/ssl/certs /usr/local/share/ca-certificates

CMD ["/scripts/bundle-certificates"]
