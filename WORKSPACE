load("@bazel_tools//tools/build_defs/repo:git.bzl",
     "git_repository", "new_git_repository")

new_git_repository(
    name = "gtest",
    remote = "https://github.com/google/googletest.git",
    tag = "release-1.8.1",
    build_file = "gtest.BUILD",
    strip_prefix = "googletest",
)

new_git_repository(
    name = "gtest-tap",
    remote = "https://github.com/kinow/gtest-tap-listener.git",
    tag = "0.6",
    build_file = "gtest-tap.BUILD",
)
