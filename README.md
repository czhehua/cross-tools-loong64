Forked from: https://github.com/loong64/cross-tools

Diff: 
- Change stable GCC version to 12.3.0. 
- Build stable gnu target for amd64 only.

# cross-tool-loong64

LoongArch64 cross-compile toolchain for x86_64(amd64) architecture.

## Supported targets

| Version      | Target                             | Kernel      | Binutils   | GCC        | Libc(glibc) | Libc(musl) |
|--------------|------------------------------------|-------------|------------|------------|-------------|------------|
| stable       | loongarch64-unknown-linux-gnu      | 6.6.101     | 2.41       | 12.3.0     | 2.38        |            |


## How to use

Download the tarball from the [release page](https://github.com/czhehua/cross-tools-loong64/releases) and extract it to `/opt/x-tools`:

```sh
sudo mkdir -p /opt/x-tools
sudo tar -xf ${Target}.tar.xz -C /opt/x-tools
```

## How to build

Fork this project and create a new release, or build manually:

```sh
./scripts/make ${Target}
```

## License

MIT

## Acknowledgements

We would like to express our gratitude to the following individuals and projects:

- [crosstool-ng](https://github.com/crosstool-ng/crosstool-ng)
- [musl-cross](https://github.com/musl-cross/musl-cross)
