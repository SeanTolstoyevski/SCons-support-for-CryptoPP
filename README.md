# SCons Support For CryptoPP

this repo adds SCons support to [CryptoPP library](https://github.com/weidai11/cryptopp).

***

In order to use SCons, python and SCons must be installed on your system.
You can use the relevant resources to install Python and SCons.

## building

Open the terminal and clone this repository. For example:

`git clone --recursive https://github.com/SeanTolstoyevski/SCons-support-for-CryptoPP`

this command pulls the latest version of CryptoPP.

first option: shared library:

`scons`

second option: static library:

`scons static=1`

Outputs are generated in the `bin/[platform]` directory.

## compilation flags

You can specify how to compile CryptoPP with the following flags.
For example, you can activate the static and release flags as follows:

`scons static=1 release=1`

Any value other than __0__ indicates that the flag is active.

### `debug`: default: 0 --> **[1 | 0]**

compiles the library in debug mode.
Can be used with all other flags

example:

`scons debug=1`

`scons debug=1 release=1 static=1`

### `release`: default: 1 --> **[1 | 0]**

Compiles the library in release mode. In this mode, all optimizations of the compiler are activated.

Can be used with other flags.

example:

`scons release=1`

### `static`: default: 0 --> **[1 | 0]**

Compiles the library as a static library.

example:

`scons static=1`

## Planned

* [ ] MSVC support
* [ ] release / debug / sanitize options
* [ ] test programs
