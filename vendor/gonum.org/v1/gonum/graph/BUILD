load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "doc.go",
        "graph.go",
        "multigraph.go",
        "undirect.go",
    ],
    importmap = "k8s.io/kubernetes/vendor/gonum.org/v1/gonum/graph",
    importpath = "gonum.org/v1/gonum/graph",
    visibility = ["//visibility:public"],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [
        ":package-srcs",
        "//vendor/gonum.org/v1/gonum/graph/encoding:all-srcs",
        "//vendor/gonum.org/v1/gonum/graph/formats/dot:all-srcs",
        "//vendor/gonum.org/v1/gonum/graph/internal/ordered:all-srcs",
        "//vendor/gonum.org/v1/gonum/graph/internal/set:all-srcs",
        "//vendor/gonum.org/v1/gonum/graph/internal/uid:all-srcs",
        "//vendor/gonum.org/v1/gonum/graph/simple:all-srcs",
    ],
    tags = ["automanaged"],
    visibility = ["//visibility:public"],
)
