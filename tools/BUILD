"""
Build supporting tools.

The tools subpackage is used to define build rules and configurations for tools
used throughout the repository. Firstparty tools not required for build support
should live elsewhere.

Of special note is that we're using the `bazel_env.bzl` tool to re-export tools
used under Bazel as a `bin/` tree which can be added to the `$PATH`. The
included `.envrc` automates this for you.

"""
load("@bazelrc-preset.bzl", "bazelrc_preset")
load("@bazel_env.bzl", "bazel_env")
load("@multitool//:tools.bzl", MULTITOOL_TOOLS = "TOOLS")

package(default_visibility = ["//visibility:public"])

bazelrc_preset(
    name = "preset",
    doc_link_template = "https://registry.build/flag/bazel?filter={flag}",
)





bazel_env(
    name = "bazel_env",
    toolchains = {




    },
    tools = {
        # Mapping from tool binary name ($PATH entry) to Bazel label







    } | MULTITOOL_TOOLS,
)
