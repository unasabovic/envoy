load(
    "//bazel:envoy_build_system.bzl",
    "envoy_cc_library",
    "envoy_extension_package",
)

licenses(["notice"])  # Apache 2

envoy_extension_package()

envoy_cc_library(
    name = "well_known_names",
    hdrs = ["well_known_names.h"],
    # well known names files are public as long as they exist.
    visibility = ["//visibility:public"],
    deps = [
        "//source/common/config:well_known_names",
        "//source/common/singleton:const_singleton",
    ],
)
