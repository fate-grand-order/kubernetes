package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = ["storage.go"],
    tags = ["automanaged"],
    deps = [
        "//pkg/api/rest:go_default_library",
        "//pkg/apis/certificates:go_default_library",
        "//pkg/genericapiserver/api/request:go_default_library",
        "//pkg/registry/certificates/certificates:go_default_library",
        "//pkg/registry/generic:go_default_library",
        "//pkg/registry/generic/registry:go_default_library",
        "//vendor:k8s.io/apimachinery/pkg/runtime",
    ],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [":package-srcs"],
    tags = ["automanaged"],
)
