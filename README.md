Forked from: https://github.com/loong64/cross-tools

Diff: 
- Change stable GCC version to 12.3.0. 
- Build stable gnu target only.

# cross-tool-loong64

LoongArch64 cross-compile toolchain, supports both x86_64(amd64) and aarch64(arm64) architectures.

## Supported targets

| Version      | Target                             | Kernel      | Binutils   | GCC        | Libc(glibc) |
|--------------|------------------------------------|-------------|------------|------------|-------------|
| stable       | loongarch64-unknown-linux-gnu      | 6.6.101     | 2.41       | 12.3.0     | 2.38        |


## How to use

Download the tarball from the [release page](https://github.com/czhehua/cross-tool-loong64/releases) and extract it to `/opt/x-tools`:

x86_64 for example:

```sh
sudo mkdir -p /opt/x-tools
sudo tar -xf x86_64-cross-tools-loongarch64-unknown-linux-gnu-stable.tar.xz -C /opt/x-tools
```

## How to build

Fork this project and create a new release, or build manually:

```sh
./scripts/make ${Target} ${VERSION}
```

## License

MIT

## Acknowledgements

We would like to express our gratitude to the following individuals and projects:

- [crosstool-ng](https://github.com/crosstool-ng/crosstool-ng)
- [musl-cross](https://github.com/musl-cross/musl-cross)
