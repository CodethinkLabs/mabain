COPTS = ["-Wall -Werror -g -O2 -std=c++11"]

cc_test(
    name = "mb_test",
    size = "small",
    srcs = glob(["mabain_test.cpp"]),
    copts = COPTS,
    deps = [
        "//src:mabain",
    ],
    linkopts = ["-lcrypto -lpthread"],
    args = ["/tmp", "test_list"],
)

cc_test(
    name = "mb_test1",
    size = "small",
    srcs = glob(["mbtest1.cpp", "test_key.h"]),
    copts = COPTS,
    deps = [
        "//src:mabain",
    ],
    linkopts = ["-lcrypto -lpthread"],
    args = ["/tmp", "5"],
)

cc_test(
    name = "mb_test2",
    size = "small",
    srcs = glob(["mbtest2.cpp", "test_key.h"]),
    copts = COPTS,
    deps = [
        "//src:mabain",
    ],
    linkopts = ["-lcrypto -lpthread"],
    args = ["/tmp", "5"],
)

cc_test(
    name = "mb_test_mp",
    size = "small",
    srcs = glob(["mbtest_mp.cpp", "test_key.h"]),
    copts = COPTS,
    deps = [
        "//src:mabain",
    ],
    linkopts = ["-lcrypto -lpthread"],
    args = ["-d", "/tmp"],
)
