
GOPATH:=$(shell go env GOPATH)

.PHONY:
build: 
	GOOS=linux GOARCH=amd64 CGO_ENABLED=0 go build -o orders-web main.go plugin.go

.PHONY: docker
docker:docker
	docker build . -t orders-web:latest
