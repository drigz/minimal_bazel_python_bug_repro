load("@third_party_py//:requirements.bzl", "requirement")

py_binary(
    name = "repro",
    srcs = [
        "repro.py",
    ],
    deps = [
        requirement("google-cloud-bigquery"),
        requirement("google-cloud-storage"),

        # Work around https://github.com/bazelbuild/rules_python/issues/30
        requirement("futures"),
    ],
)
