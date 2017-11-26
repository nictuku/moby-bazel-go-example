http_archive(
    name = "io_bazel_rules_go",
    sha256 = "91fca9cf860a1476abdc185a5f675b641b60d3acf0596679a27b580af60bf19c",
    url = "https://github.com/bazelbuild/rules_go/releases/download/0.7.0/rules_go-0.7.0.tar.gz",
)

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_register_toolchains",
    "go_rules_dependencies",
    "go_repository",
)

go_rules_dependencies()

go_register_toolchains()

load(
    "@io_bazel_rules_go//proto:def.bzl",
    "proto_register_toolchains",
)

proto_register_toolchains()

go_repository(
    name = "com_github_fsouza_go_dockerclient",
    commit = "5ffdfff51ec0eba739b1039e65ba3625ef25f7c0",
    importpath = "github.com/fsouza/go-dockerclient",
)

#go_repository(
#    name = "com_github_docker_docker",
#    commit = "dfe2c023a34de3e1731e789f4344ef4d85070bc6",
#    importpath = "github.com/docker/docker",
#)

go_repository(
    name = "com_github_docker_docker",
    build_file_generation = "on",
    build_file_name = "BUILD.bazel",
    importpath = "github.com/docker/docker",

    # runtime.PluginSpec not defined
    #commit = "dfe2c023a34de3e1731e789f4344ef4d85070bc6",
    # Temporary fix:
    strip_prefix = "docker-fcd145b091709a720c130a52196904dadafc5dda",
    urls = ["https://github.com/nictuku/docker/archive/fcd145b091709a720c130a52196904dadafc5dda.tar.gz"],
)

go_repository(
    name = "com_github_Microsoft_go_winio",
    commit = "78439966b38d69bf38227fbf57ac8a6fee70f69a",
    importpath = "github.com/Microsoft/go-winio",
)

go_repository(
    name = "com_github_docker_go_units",
    commit = "0dadbb0345b35ec7ef35e228dabb8de89a65bf52",
    importpath = "github.com/docker/go-units",
)

go_repository(
    name = "com_github_docker_go_connections",
    commit = "3ede32e2033de7505e6500d6c868c2b9ed9f169d",
    importpath = "github.com/docker/go-connections",
)

go_repository(
    name = "com_github_opencontainers_image_spec",
    commit = "577479e4dc273d3779f00c223c7e0dba4cd6b8b0",
    importpath = "github.com/opencontainers/image-spec",
)

go_repository(
    name = "com_github_pkg_errors",
    commit = "f15c970de5b76fac0b59abb32d62c17cc7bed265",
    importpath = "github.com/pkg/errors",
)

go_repository(
    name = "com_github_docker_distribution",
    commit = "bc3c7b0525e59d3ecfab3e1568350895fd4a462f",
    importpath = "github.com/docker/distribution",
)
go_repository(
    name = "com_github_opencontainers_go_digest",
    commit = "279bed98673dd5bef374d3b6e4b09e2af76183bf",
    importpath = "github.com/opencontainers/go-digest",
)
go_repository(
    name = "com_github_Nvveen_Gotty",
    commit = "cd527374f1e5bff4938207604a14f2e38a9cf512",
    importpath = "github.com/Nvveen/Gotty",
)

go_repository(
    name = "com_github_opencontainers_runc",
    commit = "fb871d9cd069aad4c8beacd261bbe36ebbf7ffd9",
    importpath = "github.com/opencontainers/runc",
)
go_repository(
    name = "org_golang_x_sys",
    commit = "4ff8c001ce4cc464e644b922325097228fce14d8",
    importpath = "golang.org/x/sys",
)
go_repository(
    name = "com_github_Azure_go_ansiterm",
    commit = "d6e3b3328b783f23731bc4d058875b0371ff8109",
    importpath = "github.com/Azure/go-ansiterm",
)
go_repository(
    name = "com_github_sirupsen_logrus",
    commit = "95cd2b9c79aa5e72ab0bc69b7ccc2be15bf850f6",
    importpath = "github.com/sirupsen/logrus",
)
go_repository(
    name = "com_github_containerd_continuity",
    commit = "0cf103d319cc2d7efe085224094f466d1f8b9640",
    importpath = "github.com/containerd/continuity",
)

go_repository(
    name = "org_golang_x_crypto",
    commit = "b080dc9a8c480b08e698fb1219160d598526310f",
    importpath = "golang.org/x/crypto",
)
