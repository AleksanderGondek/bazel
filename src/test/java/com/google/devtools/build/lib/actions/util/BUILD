load("@rules_java//java:defs.bzl", "java_library")

package(
    default_applicable_licenses = ["//:license"],
    default_testonly = 1,
    default_visibility = ["//src:__subpackages__"],
)

filegroup(
    name = "srcs",
    testonly = 0,
    srcs = glob(["*"]),
    visibility = ["//src:__subpackages__"],
)

java_library(
    name = "util",
    srcs = glob(["*.java"]),
    deps = [
        "//src/main/java/com/google/devtools/build/lib/actions",
        "//src/main/java/com/google/devtools/build/lib/actions:action_lookup_data",
        "//src/main/java/com/google/devtools/build/lib/actions:action_lookup_key",
        "//src/main/java/com/google/devtools/build/lib/actions:artifact_owner",
        "//src/main/java/com/google/devtools/build/lib/actions:artifacts",
        "//src/main/java/com/google/devtools/build/lib/actions:file_metadata",
        "//src/main/java/com/google/devtools/build/lib/actions:fileset_output_tree",
        "//src/main/java/com/google/devtools/build/lib/actions:package_roots",
        "//src/main/java/com/google/devtools/build/lib/actions:runfiles_metadata",
        "//src/main/java/com/google/devtools/build/lib/actions:runfiles_tree",
        "//src/main/java/com/google/devtools/build/lib/actions:thread_state_receiver",
        "//src/main/java/com/google/devtools/build/lib/analysis:actions/custom_command_line",
        "//src/main/java/com/google/devtools/build/lib/analysis:actions/spawn_action_template",
        "//src/main/java/com/google/devtools/build/lib/analysis:analysis_cluster",
        "//src/main/java/com/google/devtools/build/lib/analysis/platform",
        "//src/main/java/com/google/devtools/build/lib/bugreport",
        "//src/main/java/com/google/devtools/build/lib/buildeventstream/proto:build_event_stream_java_proto",
        "//src/main/java/com/google/devtools/build/lib/clock",
        "//src/main/java/com/google/devtools/build/lib/cmdline",
        "//src/main/java/com/google/devtools/build/lib/collect/nestedset",
        "//src/main/java/com/google/devtools/build/lib/events",
        "//src/main/java/com/google/devtools/build/lib/exec:single_build_file_cache",
        "//src/main/java/com/google/devtools/build/lib/skyframe:action_execution_value",
        "//src/main/java/com/google/devtools/build/lib/skyframe:action_template_expansion_value",
        "//src/main/java/com/google/devtools/build/lib/skyframe:tree_artifact_value",
        "//src/main/java/com/google/devtools/build/lib/skyframe/config",
        "//src/main/java/com/google/devtools/build/lib/skyframe/serialization/autocodec",
        "//src/main/java/com/google/devtools/build/lib/skyframe/serialization/autocodec:serialization-constant",
        "//src/main/java/com/google/devtools/build/lib/util",
        "//src/main/java/com/google/devtools/build/lib/util:crash_failure_details",
        "//src/main/java/com/google/devtools/build/lib/util:detailed_exit_code",
        "//src/main/java/com/google/devtools/build/lib/util:filetype",
        "//src/main/java/com/google/devtools/build/lib/util/io",
        "//src/main/java/com/google/devtools/build/lib/vfs",
        "//src/main/java/com/google/devtools/build/lib/vfs:pathfragment",
        "//src/main/java/com/google/devtools/build/lib/vfs/inmemoryfs",
        "//src/main/java/com/google/devtools/build/skyframe:skyframe-objects",
        "//src/main/java/com/google/devtools/common/options",
        "//src/main/java/net/starlark/java/syntax",
        "//src/main/protobuf:action_cache_java_proto",
        "//src/test/java/com/google/devtools/build/lib/exec/util",
        "//src/test/java/com/google/devtools/build/lib/testutil",
        "//third_party:error_prone_annotations",
        "//third_party:guava",
        "//third_party:jsr305",
        "//third_party:truth",
        "@com_google_protobuf//:protobuf_java",
    ],
)
