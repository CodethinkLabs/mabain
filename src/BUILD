COPTS  = ["-Wall",
          "-Werror",
          "-c",
          "-Wwrite-strings",
          "-Wsign-compare",
          "-Wcast-align",
          "-Wformat-security",
          "-fdiagnostics-show-option",
          "-g -ggdb -fPIC -O2 -std=c++11",
          "-D__SHM_LOCK__ -D__LOCK_FREE__ -D__SHM_QUEUE__"]

cc_library(
    name = "mabain",
    copts = COPTS,
    srcs = glob(["*.cpp", "util/*.cpp"]),
    includes = [".", "./util"],
    hdrs = glob(["*.h", "util/*.h"]),
    visibility = ["//visibility:public"],
)
