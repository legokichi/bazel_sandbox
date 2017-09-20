genrule(
  name = "hello",
  outs = ["hello_world.txt"],
  cmd = "echo Hello World > $@",
)

cc_library(
  name = "hello-greet",
  srcs = [
    "hello-greet.cpp"
  ],
  hdrs = [
    "hello-greet.hpp"
  ],
)

cc_binary(
  name = "main",
  srcs = [
    "main.cpp",
  ],
  copts = [
    "-fno-rtti",
  ],
  deps = [
    "@taxi_code_socialworkout_webrtc_linux//:rtc",
    ":hello-greet",
  ],
)
