# RebbleOS Resource Packs

This repository contains resources for the RebbleOS system.  The `json`
files in this directory are built using the `Utilities/mkpack.py` script
that lives in the RebbleOS repository; for the initial phase of RebbleOS
development, resources are imported from the publicly distributed Pebble
QEMU images.  As a result, it is important that one *should not distribute*
a generated resource pack until the PebbleOS components have been removed.

## In this repository...

In this repository, you will find some files and subdirectories:

* `images/` contains PNG-format image resources for both monochrome and 6-bit RGB devices.
* `qemu-tintin-images/` is a Git submodule with PebbleOS firmware images.
* `build/` contains some intermediate build products (usually, extracted resource packs from official PebbleOS firmware).
* `*.json` are resource descriptors for each supported RebbleOS device.

## Building a `.json` file

The format of the `.json` file is as described in `mkpack.py`, in the
RebbleOS repository; please take a look at `snowy.json` for an example of
extracting resources from an existing `pbpack` (from Pebble firmware), and
at `tintin.json` for an example of importing resources from a file on disk.
