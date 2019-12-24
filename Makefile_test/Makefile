# Usage:
# make        # compile all binary
# make clean  # remove ALL binaries and objects

.PHONY = all clean

CC = g++                        # compiler to use

LINKERFLAG = -lm

SRCS := foo.cpp
BINS := foo

all: clean foo run

foo: foo.o
	@echo "Checking.."
	g++ -lm foo.o -o foo

foo.o: foo.cpp
	@echo "Creating object.."
	g++ -c foo.cpp

clean:
	@echo "Cleaning up..."
	rm -rvf foo.o foo

run: foo
	./foo
