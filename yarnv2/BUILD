files(
    name="package_config",
    sources=[
        ".yarnrc.yml",
        ".yarn/releases/*.cjs",
        "tsconfig.json",
    ],
)

files(
    name="code",
    sources=["**/*.ts"],
)

package_json(
    dependencies=[
        ":package_config",
        ":code",
    ],
    scripts=[
        node_build_script(
            entry_point="build",
            output_directories=["src"],
        ),
    ],
)
