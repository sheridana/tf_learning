TAG="sheridana/tf_ml:v0.1"

.PHONY: default push

default:
	docker build -t $(TAG) .

push: default
	docker push $(TAG)
