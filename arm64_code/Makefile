TOOLCHAIN=/home/zzy/bin/gcc-linaro-aarch64-linux-gnu-4.9-2014.09_linux
# SYSROOT=${TOOLCHAIN}/sysroot

CC=${TOOLCHAIN}/bin/aarch64-linux-gnu-gcc
CPP=${TOOLCHAIN}/bin/aarch64-linux-gnu-g++
AS=${TOOLCHAIN}/bin/aarch64-linux-gnu-as
STRIP=${TOOLCHAIN}/bin/aarch64-linux-gnu-strip
CFLAGS=-O3 -fPIE -pie -g3 
#--sysroot=${SYSROOT}

all: hello1 hello2 hello3
hello1: hello1.s
	${CC} ${CFLAGS} -o hello1 hello1.s
hello2: hello2.s
	${CC} ${CFLAGS} -o hello2 hello2.s
hello3: hello3.s
	${CC} ${CFLAGS} -o hello3 hello3.s
	
clean:
	rm -rf hello1 hello2 hello3