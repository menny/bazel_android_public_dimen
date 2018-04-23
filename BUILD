
android_library(
    name = "lib",
    srcs = ["Lib.java"],
    resource_files = glob(["lib_res/**"]),
    custom_package="bazel",
    manifest = "AndroidManifest.xml",
)

android_binary(
    name = "hello_world",
    srcs = glob([
        "MainActivity.java",
    ]),
    manifest = "AndroidManifest.xml",
    resource_files = glob(["res/**"]),
    custom_package="bazel",
    deps = [
        ":lib",
        "@androidsdk//com.android.support:appcompat-v7-25.0.0",
    ],
)
