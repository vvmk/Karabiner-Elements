all: main.o
	$(MAKE) -C ../../src/lib/libkrbn
	c++ -framework CoreFoundation -framework CoreServices -framework SystemConfiguration -framework IOKit -L../../src/lib/libkrbn/build/Release -lkrbn main.o

run: all
	./a.out

include ../Makefile.rules
