# ext2fs-sys: Low-level Rust bindings for libext2fs from e2fsprogs

[![CI](https://github.com/francium-os/ext2fs-sys/actions/workflows/ci.yml/badge.svg)](https://github.com/francium-os/ext2fs-sys/actions/workflows/ci.yml)
[![license](https://img.shields.io/github/license/francium-os/ext2fs-sys.svg)](https://github.com/francium-os/ext2fs-sys/blob/master/LICENSE)

This crate makes available functionality from libext2fs. The bindings are automatically created by bindgen.

## Requirements
* libext2fs, including development headers. Linux distributions typically packages those under one of the following names:
  * e2fsprogs(-dev)
  * e2fslibs(-dev)
  * libext2fs(-dev)
* libclang is required by bindgen. This is sometimes packaged as libclang1.

Note that after an update of libext2fs, you may need to rebuild this crate to get access to any newly introduced flags.

## Intended Use
This crate should not be used directly. It's intended to be used to form higher-level abstractions.
