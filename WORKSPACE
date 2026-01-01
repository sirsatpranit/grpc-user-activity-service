workspace(name = "grpc_user_activity_service")

load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

# Protobuf
http_archive(
    name = "com_google_protobuf",
    urls = ["https://github.com/protocolbuffers/protobuf/archive/v25.1.tar.gz"],
    strip_prefix = "protobuf-25.1",
)

# gRPC
http_archive(
    name = "com_github_grpc_grpc",
    urls = ["https://github.com/grpc/grpc/archive/v1.60.0.tar.gz"],
    strip_prefix = "grpc-1.60.0",
)

load("@com_google_protobuf//:protobuf_deps.bzl", "protobuf_deps")
protobuf_deps()

load("@com_github_grpc_grpc//bazel:grpc_deps.bzl", "grpc_deps")
grpc_deps()
