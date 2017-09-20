workspace(name = "bazel_sandbox")

http_archive(
    name = "taxi_code_socialworkout_webrtc_linux",
    sha256 = "a21516985f438a23ee57d85fd87cdf8d99e4e6cfa29b6ff6a18685310d7a01f2",
    url = "https://code.taxi/download/webrtc-58-5-linux.tar.gz",
)

http_archive(
    name = "com_github_nelhage_boost",
    sha256 = "bc42251e12bc35b03eab2edb6179cc06ca4caf9bf884566a28420253d6e118c3",
    strip_prefix = "rules_boost-dbfed66073378041cd0ee2a92d75ddd6def612ec",
    type = "tar.gz",
    urls = [
        "https://github.com/nelhage/rules_boost/archive/dbfed66073378041cd0ee2a92d75ddd6def612ec.tar.gz"
    ],
)

load("@com_github_nelhage_boost//:boost/boost.bzl", "boost_deps")
boost_deps()