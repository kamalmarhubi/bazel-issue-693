load("/tools/build_defs/docker/docker", "docker_build")

docker_build(
    name = "img",
    data_path = ".",
    tars = ["base.tar"],
)

docker_build(
    name = "img-with-link",
    data_path = ".",
    base = "img",
    symlinks = { "a-dir/a-file-link": "a-file-at-root" },
)
