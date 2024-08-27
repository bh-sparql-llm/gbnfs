PATH=../../../ggerganov/llama.cpp/examples/bin
SRCS := $(wildcard tests/positive/*)
TARGETS := $(notdir $(SRCS:=_test))

all: $(TARGETS)

$(TARGETS): $(STUFF)

%_test: tests/positive/%
	llama-gbnf-validator sparql1.1.gbnf $^
