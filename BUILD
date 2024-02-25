load("@rules_cc//cc:defs.bzl", "cc_binary", "cc_library")
load("@rules_flatbuffers//flatbuffers:flatbuffers_library.bzl", "flatbuffers_library")
load("@rules_flatbuffers//flatbuffers:cc_flatbuffers_library.bzl", "cc_flatbuffers_library")

# BUILD

flatbuffers_library(
    name = "dummy_fbs",
    srcs = [
        "dummy.fbs",
    ],
    visibility = ["//visibility:public"],
)

cc_flatbuffers_library(
   name = "dummy",
   deps = ["dummy_fbs"],
)

cc_binary(
   name = "main",
   srcs = ["main.cc"],
   deps = [":dummy"],
)
