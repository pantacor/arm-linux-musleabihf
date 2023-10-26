armv6-eabihf--musl--stable-2023.08-1

This is a toolchain provided by the https://toolchains.bootlin.com/
service. This toolchain was built using Buildroot.

The complete source code for all components of the toolchain can be
found at http://toolchains.bootlin.com/downloads/releases/sources/.

The complete license text of all components of the toolchain can be
found at http://toolchains.bootlin.com/downloads/releases/licenses/.

This toolchain is based on:

    gcc                  version     12.3.0
    binutils             version       2.40
    gdb                  version       12.1
    musl                 version      1.2.4

For those who would like to reproduce the toolchain, you can just
follow these steps:

    git clone https://github.com/bootlin/buildroot-toolchains.git buildroot
    cd buildroot
    git checkout toolchains.bootlin.com-2023.08.1

    curl http://toolchains.bootlin.com/downloads/releases/toolchains/armv6-eabihf/build_fragments/armv6-eabihf--musl--stable-2023.08-1.defconfig > .config
    make olddefconfig
    make
    make sdk
