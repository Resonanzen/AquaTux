SRCS:=$(wildcard *.c)
OBJ:=$(patsubst %.c,%.o,$(SRCS))
EXES:=$(patsubst %.c,%.out,$(SRCS))

include ../Makefile.in
include Makefile.deps

%.out: %.o $(LIB)
	$(CC) -o $@ $< $(CXXFLAGS)

.PHONY: $(PHONY_TARGETS)
