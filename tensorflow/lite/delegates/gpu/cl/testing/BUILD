package(
    default_visibility = ["//visibility:public"],
    licenses = ["notice"],  # Apache 2.0
)

cc_binary(
    name = "delegate_testing",
    srcs = ["delegate_testing.cc"],
    tags = [
        "nobuilder",
        "notap",
    ],
    deps = [
        "//tensorflow/lite/delegates/gpu:delegate",
        "//tensorflow/lite/delegates/gpu/cl:gpu_api_delegate",
        "//tensorflow/lite/delegates/gpu/common:status",
        "//tensorflow/lite/delegates/gpu/common/testing:tflite_model_reader",
        "//tensorflow/lite/kernels:builtin_ops",
        "//tensorflow/lite/kernels:kernel_util",
        "@com_google_absl//absl/time",
    ],
)

cc_binary(
    name = "internal_api_samples",
    srcs = ["internal_api_samples.cc"],
    deps = [
        "//tensorflow/lite/delegates/gpu:api",
        "//tensorflow/lite/delegates/gpu/cl:api",
        "//tensorflow/lite/delegates/gpu/cl:environment",
        "//tensorflow/lite/delegates/gpu/cl:inference_context",
        "//tensorflow/lite/delegates/gpu/common:model",
        "//tensorflow/lite/delegates/gpu/common:status",
        "//tensorflow/lite/delegates/gpu/common/testing:tflite_model_reader",
        "//tensorflow/lite/kernels:builtin_ops",
        "//tensorflow/lite/kernels:kernel_util",
        "@com_google_absl//absl/time",
    ],
)

cc_binary(
    name = "performance_profiling",
    srcs = ["performance_profiling.cc"],
    deps = [
        "//tensorflow/lite/delegates/gpu/cl:environment",
        "//tensorflow/lite/delegates/gpu/cl:inference_context",
        "//tensorflow/lite/delegates/gpu/common:model",
        "//tensorflow/lite/delegates/gpu/common:status",
        "//tensorflow/lite/delegates/gpu/common/testing:tflite_model_reader",
        "//tensorflow/lite/kernels:builtin_ops",
        "@com_google_absl//absl/time",
    ],
)
