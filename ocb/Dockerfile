FROM golang:alpine
RUN GO111MODULE=on go install go.opentelemetry.io/collector/cmd/builder@v0.95.0
ENTRYPOINT [ "/go/bin/builder" ]
