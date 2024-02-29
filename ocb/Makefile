.PHONY: default
default: build

.PHONY: build
build:
	@docker buildx build -t opencodeco/ocb:v0.95.0 .

.PHONY: push
push:
	@docker push opencodeco/ocb:v0.95.0

.PHONY: run
run:
	@docker run --rm \
		-v ./otelcol-builder.yaml:/otelcol-builder.yaml -v ./output:/output \
		opencodeco/ocb --config /otelcol-builder.yaml
