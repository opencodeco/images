.PHONY: default
default: build run

.PHONY: build
build:
	@docker buildx build -t opencodeco/ocb .

.PHONY: run
run:
	@docker run --rm \
		-v ./otelcol-builder.yaml:/otelcol-builder.yaml -v ./output:/output \
		opencodeco/ocb --config /otelcol-builder.yaml
