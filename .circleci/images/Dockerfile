FROM alpine:3.11

RUN apk update
RUN apk add --no-cache wget openssh git bash tar gzip ca-certificates
RUN rm -rf /var/cache/apk/*
RUN wget --quiet https://releases.hashicorp.com/terraform/0.12.26/terraform_0.12.26_linux_amd64.zip \
  && unzip terraform_0.12.26_linux_amd64.zip \
  && mv terraform /usr/bin \
  && rm terraform_0.12.26_linux_amd64.zip
