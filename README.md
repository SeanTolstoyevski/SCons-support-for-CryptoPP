# SCons Support For CryptoPP

this repo adds SCons support to [CryptoPP library](https://github.com/weidai11/cryptopp).

***

In order to use SCons, python and SCons must be installed on your system.
You can use the relevant resources to install Python and SCons.

## building

Open the terminal.

first option: shared library:

`scons`

third option: static library:

`scons static=1`

Outputs are generated in the `bin/[platform]` directory.

## Planned

* [ ] MSVC support
* [ ] release / debug / sanitize options
* [ ] test programs
