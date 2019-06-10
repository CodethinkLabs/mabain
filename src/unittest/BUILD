COPTS = ["-Wall -Werror -g -O2 -std=c++11",
        "-fprofile-arcs -ftest-coverage -fPIC -D__SHM_QUEUE__"]


cc_test(
    name="mabain-test",
    size = "small",
    srcs=glob(["*.cpp", "*.h"]),
    copts = COPTS,
    deps = [
        "@gtest//:main",
        "@gtest-tap//:main",
        "//src:mabain",
    ],
    linkopts = ["-lcrypto -lpthread -lgcov --coverage"],
)
