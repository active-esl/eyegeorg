# eyegeorg

Demo of the HTML version can be found at https://goatchurch.itch.io/eyes

## Linux ARM64 build

GitHub Actions exports a Godot 4.3 Linux ARM64 bundle for use in the screen
machine's Yocto image. Download the `eyegeorg-linux-arm64` workflow artefact
and unpack `eyegeorg-linux-arm64.tar.gz`; it contains the AArch64 executable
and its resource pack:

```text
eyegeorg.arm64
eyegeorg.pck
elf.txt
```

The CI job verifies that the executable is an AArch64 ELF before publishing
the artefact. Keep both the executable and `.pck` file together when installing
them into the target root filesystem.
