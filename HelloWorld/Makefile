SRC := src
BIN := bin

RM := rm -vf
TARGET := $(shell find . -type f -not -name "*.rs" -and -not -name "Makefile" -and -not -name ".git")

all: helloworld

helloworld:
	mkdir -p $(BIN)
	rustc $(SRC)/helloworld.rs -o $(BIN)/helloworld

run: helloworld
	$(BIN)/helloworld

clean: 
	$(RM) bin/*