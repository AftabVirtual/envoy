licenses(["notice"])  # Apache 2

load(
    "//bazel:envoy_build_system.bzl",
    "envoy_cc_test",
    "envoy_package",
)

envoy_package()

envoy_cc_test(
    name = "fault_config_test",
    srcs = ["fault_config_test.cc"],
    deps = [
        "//source/extensions/filters/common/fault:fault_config_lib",
        "//test/test_common:utility_lib",
        "@envoy_api//envoy/config/filter/fault/v2:pkg_cc_proto",
    ],
)
