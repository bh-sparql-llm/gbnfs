# gbnfs/sparql1.1

SPARQL 1.1 GBNF (whatever that is) grammar for Llama.

The tests dir contains positive tests for the grammar. You can verify them with llama-gbnf-validator:

``` bash
git clone {git@github.com:,}ggerganov/llama.cpp --depth=1
cd ggerganov/llama.cpp/examples/
make llama-gbnf-validator # creates bin/llama-gbnf-validator
```

Now come back to this directory and tweak the PATH set in the top of the Makefile to reflect the path to `llama-gbnf-validator`. (It works out of the box if the two repos are arranged like:
```
- ggerganov/llama.cpp
- bh-sparql-llm/gbnfs
```
You can then run the Makefile to test each file in `tests/` against the grammar.
