load(
    "@bazel_tools//tools/jdk:default_java_toolchain.bzl", "default_java_toolchain",
)

package(default_visibility = ["//visibility:public"])

TOOLCHAIN_CONFIGURATION = dict(
    jvm_opts = [],
    ijar = ["@remote_java_tools//:ijar_cc_binary"],
    singlejar = ["@remote_java_tools//:singlejar_cc_bin"],
    java_runtime = "@jdk8_macos_x86//:jdk",
)

default_java_toolchain(
    name = "toolchain_jdk_8",
    configuration = TOOLCHAIN_CONFIGURATION,
    java_runtime = "@jdk8_macos_x86//:jdk",
    source_version = "8",
    target_version = "8",
)
