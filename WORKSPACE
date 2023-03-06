load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
	name="greet_lib",
	url="https://github.com/EmilePapillon/bazel_tutorial/tarball/master/filename.tar.gz",
	sha256="0d92f0a739db26004166666b5045423255f6df6320ae8422155bebf1f4f1acea",
	build_file="//greet_lib:greeter.BUILD",
	strip_prefix="EmilePapillon-bazel_tutorial-252c76d"
)

http_archive(
    name = "com_google_protobuf",
    sha256 = "25680843adf0c3302648d35f744e38cc3b6b05a6c77a927de5aea3e1c2e36106",
    strip_prefix = "protobuf-3.19.4",
    urls = ["https://github.com/protocolbuffers/protobuf/archive/refs/tags/v3.19.4.zip"],
)

load("@com_google_protobuf//:protobuf_deps.bzl", "protobuf_deps")

protobuf_deps()
