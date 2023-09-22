load("//build_tools/rules:variables.bzl", "PLATO_OPTS")

cc_binary (
    name = "personalized_pagerank",
    srcs = [
        "personalized_pagerank.cc",
    ],
    copts = ['-g', '-O2', ] + PLATO_OPTS,
    linkopts = [ ] + PLATO_OPTS,
    deps = [
        "//3rd/glog:glog",
        "//3rd/gflags:gflags",

        "//3rd/boost:boost_include",
        "//3rd/boost:boost_iostreams",

        "//plato/graph:graph",
        "//plato/algo/ppr:personalized_pagerank",
    ],
    defines = [
        # "__DCSC_DEBUG__",
    ],
    linkstatic = 1,
)

cc_binary (
    name = "pushpull_ppr",
    srcs = [
        "pushpull_ppr.cc",
    ],
    copts = ['-g', '-O2', ] + PLATO_OPTS,
    linkopts = [ ] + PLATO_OPTS,
    deps = [
        "//3rd/glog:glog",
        "//3rd/gflags:gflags",

        "//3rd/boost:boost_include",
        "//3rd/boost:boost_iostreams",

        "//plato/graph:graph",
        "//plato/algo/ppr:personalized_pagerank",
    ],
    defines = [
        # "__DCSC_DEBUG__",
    ],
    linkstatic = 1,
)

cc_binary (
    name = "trustrank",
    srcs = [
        "trustrank.cc",
    ],
    copts = ['-g', '-O2', ] + PLATO_OPTS,
    linkopts = [ ] + PLATO_OPTS,
    deps = [
        "//3rd/glog:glog",
        "//3rd/gflags:gflags",

        "//3rd/boost:boost_include",
        "//3rd/boost:boost_iostreams",

        "//plato/graph:graph",
        "//plato/algo/trustrank:trustrank",
    ],
    defines = [
        # "__DCSC_DEBUG__",
    ],
    linkstatic = 1,
)

cc_binary (
    name = "belief_propagation",
    srcs = [
        "belief_propagation.cc",
    ],
    copts = ['-g', '-O2', ] + PLATO_OPTS,
    linkopts = [ ] + PLATO_OPTS,
    deps = [
        "//3rd/glog:glog",
        "//3rd/gflags:gflags",

        "//3rd/boost:boost_include",
        "//3rd/boost:boost_iostreams",

        "//plato/graph:graph",
        "//plato/algo/bp:belief_propagation",
    ],
    defines = [
        # "__DCSC_DEBUG__",
    ],
    linkstatic = 1,
)