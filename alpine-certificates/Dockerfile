# isso é um place holder, permitindo-nos refletir as imagens dos certificados para alpine-certificates
ARG CI_REGISTRY_IMAGE="registry.inure.com/inure-org/build/cng"
ARG FROM_IMAGE="$CI_REGISTRY_IMAGE/certificates"

FROM --platform=${TARGETPLATFORM} ${FROM_IMAGE}:${COMMIT_REF_SLUG}
