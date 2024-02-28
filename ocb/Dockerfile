FROM golang:alpine
RUN GO111MODULE=on go install go.opentelemetry.io/collector/cmd/builder@latest
ENTRYPOINT [ "/go/bin/builder" ]
