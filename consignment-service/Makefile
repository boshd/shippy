build:
	protoc -I. --go_out=plugins=grpc:. \
		proto/consignment/consignment.proto
	docker build -t consignment-service .

run:
	docker run -p 50051:50051 consignment-service