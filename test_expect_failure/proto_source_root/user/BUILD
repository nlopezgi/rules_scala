load(
    "//scala_proto:scala_proto.bzl",
    "scalapb_proto_library",
)

proto_library(
    name = "user",
    srcs = glob(["*.proto"]),
    proto_source_root = package_name(),
    deps = ["//test_expect_failure/proto_source_root/dependency"],
)

scalapb_proto_library(
    name = "user_scala",
    visibility = ["//visibility:public"],
    deps = [":user"],
)
