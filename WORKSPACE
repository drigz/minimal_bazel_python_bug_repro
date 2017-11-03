# Helpful macros to support requirements/pip integration.
git_repository(
    name = "io_bazel_rules_python",
    commit = "5f78b4a04a50d660ec346df1a1ab76b02130c304",
    remote = "https://github.com/drigz/rules_python.git",
)

load("@io_bazel_rules_python//python:pip.bzl", "pip_repositories", "pip_import")

pip_repositories()

pip_import(
    name = "third_party_py",
    requirements = "//:requirements.txt",
)

load("@third_party_py//:requirements.bzl", "pip_install")

pip_install()
