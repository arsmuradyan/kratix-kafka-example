FROM alpine:latest
RUN [ "mkdir", "/tmp/transfer" ]
RUN apk update && apk add --no-cache yq

ADD resources/ /tmp/transfer/
ADD execute-pipeline execute-pipeline
RUN chmod 777 execute-pipeline

CMD [ "sh", "-c", "./execute-pipeline" ]
ENTRYPOINT []