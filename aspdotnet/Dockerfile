ARG DOCKER_TAG
FROM mcr.microsoft.com/dotnet/aspnet:$DOCKER_TAG
ENV DOTNET_SYSTEM_GLOBALIZATION_INVARIANT=false
RUN \
  apk update && \
  apk upgrade && \
  apk add \
  icu-libs && \
  rm -rf /var/cache/apk/*
