package(default_visibility = ["//visibility:public"])

load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = ["noop.go"],
    visibility = ["//visibility:public"],
    deps = ["//mixer/pkg/adapter:go_default_library"],
)

go_test(
    name = "go_default_test",
    size = "small",
    srcs = ["noop_test.go"],
    library = ":go_default_library",
    deps = [
        "//mixer/pkg/adapter:go_default_library",
        "//mixer/pkg/adapterManager:go_default_library",
        "//mixer/pkg/config:go_default_library",
    ],
)
