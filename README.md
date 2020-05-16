# GRPC Example

Proto for GRPC Server & Client

```bash
# Generate protoc
$ protoc proto/math/math.proto --go_out=plugins=grpc:.

# Build base image for GRPC Server & Client
$ docker build -f ./docker/base/Dockerfile -t ${USER_NAME}/grpc-common-example .
$ docker push ${USER_NAME}/grpc-common-example
```
