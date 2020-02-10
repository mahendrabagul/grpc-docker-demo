FROM golang
ADD . /go/src/github.com/mahendrabagul/grpc-docker-demo/grpc-server
RUN go version
RUN go get -d -u github.com/golang/protobuf/protoc-gen-go \
    && go install github.com/golang/protobuf/protoc-gen-go
RUN go get golang.org/x/net/context
RUN go get google.golang.org/grpc
RUN go get google.golang.org/grpc/codes
RUN go get google.golang.org/grpc/grpclog
RUN go get google.golang.org/grpc/status
RUN go install github.com/mahendrabagul/grpc-docker-demo/grpc-server
ENTRYPOINT ["/go/bin/grpc-server"]
EXPOSE 5300
