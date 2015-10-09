#complie .so(share object) file for python

cc = gcc
CFLAG = -wall -o2
INCLUDE = -I/usr/include/pythe

all:example.so

%.o:%.c
	${cc} ${CFLAG} ${INCLUDE} -fpic -c $< -o $@

example_obj = example.o wrap.o
example.so:${example_obj}
	${cc} ${CFLAG} -shared $^ -o $@

.PYONY: clean
clean:
	rm
