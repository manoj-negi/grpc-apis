# grpc-apis

protoc: The Protocol Buffers compiler command.
--go_out=pb: Specifies the output directory for the generated Go code. In this case, it's the pb directory.
--plugin=protoc-gen-go=$(which protoc-gen-go): Specifies the path to the protoc-gen-go plugin.
--go_opt=paths=source_relative: Generates the output files with paths relative to the source .proto file location.
--go-grpc_out=pb: Specifies the output directory for the generated gRPC Go code. In this case, it's also the pb directory.
--plugin=protoc-gen-go-grpc=$(which protoc-gen-go-grpc): Specifies the path to the protoc-gen-go-grpc plugin.
--go-grpc_opt=paths=source_relative: Ensures that the gRPC service files are generated with paths relative to the source .proto file location.
proto/chat.proto: The path to the input .proto file.
