load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = [
        "addons.go",
        "bootstraptoken.go",
        "certs.go",
        "controlplane.go",
        "etcd.go",
        "kubeconfig.go",
        "kubelet.go",
        "markcontrolplane.go",
        "preflight.go",
        "uploadconfig.go",
        "util.go",
        "waitcontrolplane.go",
    ],
    importpath = "k8s.io/kubernetes/cmd/kubeadm/app/cmd/phases",
    visibility = ["//visibility:public"],
    deps = [
        "//cmd/kubeadm/app/apis/kubeadm:go_default_library",
        "//cmd/kubeadm/app/apis/kubeadm/scheme:go_default_library",
        "//cmd/kubeadm/app/apis/kubeadm/v1beta1:go_default_library",
        "//cmd/kubeadm/app/apis/kubeadm/validation:go_default_library",
        "//cmd/kubeadm/app/cmd/options:go_default_library",
        "//cmd/kubeadm/app/cmd/phases/workflow:go_default_library",
        "//cmd/kubeadm/app/cmd/util:go_default_library",
        "//cmd/kubeadm/app/constants:go_default_library",
        "//cmd/kubeadm/app/phases/addons/dns:go_default_library",
        "//cmd/kubeadm/app/phases/addons/proxy:go_default_library",
        "//cmd/kubeadm/app/phases/bootstraptoken/clusterinfo:go_default_library",
        "//cmd/kubeadm/app/phases/bootstraptoken/node:go_default_library",
        "//cmd/kubeadm/app/phases/certs:go_default_library",
        "//cmd/kubeadm/app/phases/controlplane:go_default_library",
        "//cmd/kubeadm/app/phases/etcd:go_default_library",
        "//cmd/kubeadm/app/phases/kubeconfig:go_default_library",
        "//cmd/kubeadm/app/phases/kubelet:go_default_library",
        "//cmd/kubeadm/app/phases/markcontrolplane:go_default_library",
        "//cmd/kubeadm/app/phases/patchnode:go_default_library",
        "//cmd/kubeadm/app/phases/uploadconfig:go_default_library",
        "//cmd/kubeadm/app/preflight:go_default_library",
        "//cmd/kubeadm/app/util:go_default_library",
        "//cmd/kubeadm/app/util/apiclient:go_default_library",
        "//cmd/kubeadm/app/util/config:go_default_library",
        "//cmd/kubeadm/app/util/dryrun:go_default_library",
        "//cmd/kubeadm/app/util/pkiutil:go_default_library",
        "//pkg/util/normalizer:go_default_library",
        "//pkg/version:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/util/sets:go_default_library",
        "//staging/src/k8s.io/client-go/kubernetes:go_default_library",
        "//vendor/github.com/pkg/errors:go_default_library",
        "//vendor/github.com/renstrom/dedent:go_default_library",
        "//vendor/github.com/spf13/cobra:go_default_library",
        "//vendor/github.com/spf13/pflag:go_default_library",
        "//vendor/k8s.io/klog:go_default_library",
        "//vendor/k8s.io/utils/exec:go_default_library",
    ],
)

go_test(
    name = "go_default_test",
    srcs = [
        "certs_test.go",
        "util_test.go",
    ],
    embed = [":go_default_library"],
    deps = [
        "//cmd/kubeadm/app/apis/kubeadm:go_default_library",
        "//cmd/kubeadm/app/apis/kubeadm/v1beta1:go_default_library",
        "//cmd/kubeadm/app/cmd/phases/workflow:go_default_library",
        "//cmd/kubeadm/app/phases/certs:go_default_library",
        "//cmd/kubeadm/app/util/pkiutil:go_default_library",
        "//cmd/kubeadm/test:go_default_library",
        "//cmd/kubeadm/test/certs:go_default_library",
        "//pkg/version:go_default_library",
        "//vendor/github.com/spf13/cobra:go_default_library",
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
    srcs = [
        ":package-srcs",
        "//cmd/kubeadm/app/cmd/phases/workflow:all-srcs",
    ],
    tags = ["automanaged"],
    visibility = ["//visibility:public"],
)
