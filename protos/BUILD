load("@rules_proto//proto:defs.bzl", "proto_library")
load("@rules_proto_grpc_python//:defs.bzl", "python_grpc_library")

package(
    default_visibility = ["//visibility:public"],
)

proto_library(
    name = "helloworld_proto",
    srcs = ["helloworld.proto"],
)

proto_library(
    name = "routeguide_proto",
    srcs = ["routeguide.proto"],
)

python_grpc_library(
    name = "routeguide_py_grpc",
    # output_mode = "NO_PREFIX",
    protos = [":routeguide_proto"],
)

