# Container image that runs the code
FROM alpine:3.10

RUN apk update
RUN apk add bash
RUN apk add git

# Copies the code file from your action directory to the filesystem path `/` of the container
COPY entrypoint.sh /entrypoint.sh

# Code file to execute when the docker container starts up (`entrypoint.sh`)
ENTRYPOINT ["/entrypoint.sh"]
