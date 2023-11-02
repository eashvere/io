load("@build_bazel_rules_swift//swift:swift.bzl", "swift_library")

package(default_visibility = ["//visibility:public"])

swift_library(
    name = "audio_video_swift",
    srcs = [
        "//tensorflow_io/core:swift/audio.swift",
        "//tensorflow_io/core:swift/video.swift",
    ],
    copts = [
        "-target",
        "arm64-apple-macos11.0",
    ],
    linkopts = [
        "-L/usr/lib/swift",
        "-Wl,-rpath,/usr/lib/swift",
        "-target",
        "arm64-apple-macos11.0",
    ],
    module_name = "audio_video",
    alwayslink = True,
)
