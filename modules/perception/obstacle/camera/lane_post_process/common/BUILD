load("//tools:cpplint.bzl", "cpplint")

package(default_visibility = ["//visibility:public"])

cc_library(
    name = "type",
    srcs = ["type.cc"],
    hdrs = ["type.h"],
    deps = [
        "//modules/common:log",
        "//modules/perception/proto:perception_proto",
        "@eigen",
        "@opencv2//:core",
    ],
)

cc_library(
    name = "util",
    hdrs = ["util.h"],
    deps = [
        ":type",
        "//modules/common:log",
    ],
)

cc_library(
    name = "connected_component",
    srcs = ["connected_component.cc"],
    hdrs = ["connected_component.h"],
    deps = [
        ":type",
        "//modules/common:log",
        "@eigen",
        "@opencv2//:core",
    ],
)

cc_library(
    name = "projector",
    hdrs = ["projector.h"],
    deps = [
        "//modules/common:log",
        "//modules/perception/lib/config_manager",
        "//modules/perception/obstacle/camera/common",
        "@eigen",
        "@opencv2//:core",
    ],
)

cpplint()
