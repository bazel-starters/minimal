"""Targets in the repository root"""





load("@gazelle//:def.bzl", "gazelle")



# We prefer BUILD instead of BUILD.bazel
# gazelle:build_file_name BUILD
# gazelle:exclude githooks/*
gazelle(
    name = "gazelle",
    gazelle = "@multitool//tools/gazelle",
    env = {
        "ENABLE_LANGUAGES": ",".join([
            "starlark",
            "proto",
        ]),
    }
)


