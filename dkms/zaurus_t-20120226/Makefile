#
# Makefile for USB Network drivers
#

obj-m	+= zaurus_t.o

all:
	make -C /lib/modules/`uname -r`/build M=`pwd`

clean:
	make -C /lib/modules/`uname -r`/build M=`pwd` clean

install:
	install -D -m 755 zaurus_t.ko /lib/modules/`uname -r`/kernel/drivers/net/usb/zaurus_t.ko

