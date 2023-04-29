load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

load("//:fixed_containers_deps.bzl", "fixed_containers_deps")
fixed_containers_deps()

http_archive(
    name = "com_google_googletest",
    urls = ["https://github.com/google/googletest/archive/16f637fbf4ffc3f7a01fa4eceb7906634565242f.tar.gz"],
    strip_prefix = "googletest-16f637fbf4ffc3f7a01fa4eceb7906634565242f",
    sha256 = "879a4064738cb3c76a11d449145b442654d7282f3cd0f5f03ec8c3dc862646c6",
    patches = [
            "//:patches/gtest_use_maybe_unused_instead_of_attribute_unused.patch",
    ],
)
