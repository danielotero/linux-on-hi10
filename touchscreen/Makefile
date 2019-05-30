obj-m += silead-test.o

build:
	make -C /lib/modules/$(shell uname -r)/build M=$(PWD) modules

clean:
	make -C /lib/modules/$(shell uname -r)/build M=$(PWD) clean

remove:
	-sudo rmmod silead-test

install:
	sudo insmod silead-test.ko

test: build remove install
