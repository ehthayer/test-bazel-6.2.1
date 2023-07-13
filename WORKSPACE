load("@bazel_tools//tools/jdk:remote_java_repository.bzl", "remote_java_repository")

remote_java_repository(
    name = "jdk8_macos_x86",
    prefix = "cg_jdk",
    version = "8",
    urls = [ "https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_x64_mac_hotspot_8u292b10.tar.gz" ],
    sha256 = "5646fbe9e4138c902c910bb7014d41463976598097ad03919e4848634c7e8007",
    target_compatible_with = [
        "@platforms//os:macos",
        "@platforms//cpu:x86_64",
    ],
)

remote_java_repository(
  name = "jdk8_linux_x86",
  prefix = "cg_jdk",
  version = "8",
  urls = ["https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_x64_linux_hotspot_8u292b10.tar.gz"],
  sha256 = "0949505fcf42a1765558048451bb2a22e84b3635b1a31dd6191780eeccaa4ada",
  target_compatible_with = [
      "@platforms//os:linux",
      "@platforms//cpu:x86_64",
  ]
)

register_toolchains("//tools/java:all")
