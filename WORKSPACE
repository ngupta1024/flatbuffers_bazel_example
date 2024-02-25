load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "rules_cc",
    urls = ["https://github.com/bazelbuild/rules_cc/releases/download/0.0.9/rules_cc-0.0.9.tar.gz"],
    sha256 = "2037875b9a4456dce4a79d112a8ae885bbc4aad968e6587dca6e64f3a0900cdf",
    strip_prefix = "rules_cc-0.0.9",
)

http_archive(
    name = "rules_flatbuffers",
    sha256 = "902e649b358846c762829e7aae78db346571ffed7f4a849deebf0f0f69fb398e",
    strip_prefix = "rules_flatbuffers-0.2.0",
    urls = ["https://github.com/kgreenek/rules_flatbuffers/archive/refs/tags/v0.2.0.tar.gz"],
)

load(
    "@rules_flatbuffers//flatbuffers:repositories.bzl",
    "flatbuffers_cc_toolchain",
    "flatbuffers_dependencies",
    "flatbuffers_toolchain",
)

flatbuffers_dependencies()

flatbuffers_toolchain()

flatbuffers_cc_toolchain()