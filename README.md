# grpc-docker-demo
Sample Demo to run gRPC server in Docker container




$ cd grpc-server

$ sudo docker build -t mahendrabagul/grpc-server .

$ docker run -it -p 5300:5300 mahendrabagul/grpc-server

$ cd ../grpc-client

$ go build -o reverse

$ ./reverse "this is a test"

tset a si siht
