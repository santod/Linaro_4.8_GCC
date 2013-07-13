Linaro_4.8_GCC
==============

NuK3RN3L Toolchain


Prebuilt Toolchain Binaries

Prebuilt toolchains for various GCC versions and Linaro milestone releases are provided at https://android-build.linaro.org/ , builds titled ~linaro-android/toolchain-*. Previews of upcoming releases can be found in builds titled ~linaro-android/toolchain-4.7-bzr

(Older prototype builds of the Android toolchain can be found at http://people.linaro.org/~jserv/toolchain/)

To build Android Platform with Linaro Toolchain:

    Extracte toolchain tarball to some directory (/tmp/android-toolchain-eabi is assumed below)
    Change directory to Android toplevel directory and build: 

$ make TARGET_TOOLS_PREFIX=/tmp/android-toolchain-eabi/bin/arm-linux-androideabi- TARGET_PRODUCT=pandaboard systemtarball userdatatarball boottarball

(pandaboard is just an example, replace it with the board you're building for) 
