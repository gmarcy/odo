package(default_visibility = ["//visibility:public"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = [
        "controller.go",
        "hollow_kubelet.go",
        "hollow_proxy.go",
    ],
    importpath = "k8s.io/kubernetes/pkg/kubemark",
    deps = [
        "//cmd/kube-proxy/app:go_default_library",
        "//cmd/kubelet/app:go_default_library",
        "//cmd/kubelet/app/options:go_default_library",
        "//pkg/controller:go_default_library",
        "//pkg/kubelet:go_default_library",
        "//pkg/kubelet/apis/config:go_default_library",
        "//pkg/kubelet/cadvisor:go_default_library",
        "//pkg/kubelet/cm:go_default_library",
        "//pkg/kubelet/container/testing:go_default_library",
        "//pkg/kubelet/dockershim:go_default_library",
        "//pkg/kubelet/types:go_default_library",
        "//pkg/proxy:go_default_library",
        "//pkg/proxy/iptables:go_default_library",
        "//pkg/util/iptables:go_default_library",
        "//pkg/util/mount:go_default_library",
        "//pkg/util/node:go_default_library",
        "//pkg/util/oom:go_default_library",
        "//pkg/util/sysctl:go_default_library",
        "//pkg/volume/emptydir:go_default_library",
        "//pkg/volume/projected:go_default_library",
        "//pkg/volume/secret:go_default_library",
        "//staging/src/k8s.io/api/core/v1:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/fields:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/labels:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/types:go_default_library",
        "//staging/src/k8s.io/client-go/informers:go_default_library",
        "//staging/src/k8s.io/client-go/informers/core/v1:go_default_library",
        "//staging/src/k8s.io/client-go/kubernetes:go_default_library",
        "//staging/src/k8s.io/client-go/kubernetes/typed/core/v1:go_default_library",
        "//staging/src/k8s.io/client-go/listers/core/v1:go_default_library",
        "//staging/src/k8s.io/client-go/tools/cache:go_default_library",
        "//staging/src/k8s.io/client-go/tools/record:go_default_library",
        "//test/utils:go_default_library",
        "//vendor/k8s.io/klog:go_default_library",
        "//vendor/k8s.io/utils/exec:go_default_library",
        "//vendor/k8s.io/utils/pointer:go_default_library",
    ],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [":package-srcs"],
    tags = ["automanaged"],
)
