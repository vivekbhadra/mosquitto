# Building for Titan  
sc docker run sky-q-in-life 'make clean; make CC="$SKY_ONE_COMMON_TOOLCHAIN_BASE"/bin/arm-linux-gcc CXX="$SKY_ONE_COMMON_TOOLCHAIN_BASE"/bin/arm-linux-g++ AR="$SKY_ONE_COMMON_TOOLCHAIN_BASE"/bin/arm-linux-ar LD="$SKY_ONE_COMMON_TOOLCHAIN_BASE"/bin/arm-linux-ld'

# Building for Hub 4 
sc docker run bcm502l07 'make clean; make CC=/opt/toolchains/crosstools-arm-gcc-5.3-linux-4.1-glibc-2.22-binutils-2.25/usr/bin/arm-linux-gcc CXX=/opt/toolchains/crosstools-arm-gcc-5.3-linux-4.1-glibc-2.22-binutils-2.25/usr/bin/arm-linux-g++ AR=/opt/toolchains/crosstools-arm-gcc-5.3-linux-4.1-glibc-2.22-binutils-2.25/usr/bin/arm-linux-ar LD=/opt/toolchains/crosstools-arm-gcc-5.3-linux-4.1-glibc-2.22-binutils-2.25/usr/bin/arm-linux-ld'

# Building for RDK
sc docker run ada-sdk 'make clean; make CC=/opt/toolchains/crosstools-aarch64-gcc-10.3-linux-4.19-glibc-2.32-binutils-2.36.1/bin/aarch64-linux-gcc CXX=/opt/toolchains/crosstools-aarch64-gcc-10.3-linux-4.19-glibc-2.32-binutils-2.36.1/bin/aarch64-linux-g++ AR=/opt/toolchains/crosstools-aarch64-gcc-10.3-linux-4.19-glibc-2.32-binutils-2.36.1/bin/aarch64-linux-ar LD=/opt/toolchains/crosstools-aarch64-gcc-10.3-linux-4.19-glibc-2.32-binutils-2.36.1/bin/aarch64-linux-ld'

# Building for Xwing
sc docker run sky-q-in-life 'make clean; make CC="$ST_COMMON_TOOLCHAIN_BASE"/bin/armv7-linux-gcc CXX="$ST_COMMON_TOOLCHAIN_BASE"/bin/armv7-linux-g++ AR="$ST_COMMON_TOOLCHAIN_BASE"bin/armv7-linux-ar LD="$ST_COMMON_TOOLCHAIN_BASE"/bin/armv7-linux-ld'

