package(licenses = ["notice"])  # BSD

load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "fdbased",
    srcs = ["endpoint.go"],
    importpath = "gvisor.googlesource.com/gvisor/pkg/tcpip/link/fdbased",
    visibility = [
        "//visibility:public",
    ],
    deps = [
        "//pkg/tcpip",
        "//pkg/tcpip/buffer",
        "//pkg/tcpip/header",
        "//pkg/tcpip/link/rawfile",
        "//pkg/tcpip/stack",
    ],
)

go_test(
    name = "fdbased_test",
    size = "small",
    srcs = ["endpoint_test.go"],
    embed = [":fdbased"],
    deps = [
        "//pkg/tcpip",
        "//pkg/tcpip/buffer",
        "//pkg/tcpip/header",
        "//pkg/tcpip/stack",
    ],
)
