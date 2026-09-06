
ifdef DEBUG
DEBUGFLGS = -g
else
DEBUGFLGS =
endif
LSTFLGS =

LDFLAGS = -lc -e main -arch arm64

all: divexamp mulexamp matrixmult

divexamp: divexamp.s debug.s
	clang $(LDFLAGS) -o divexamp divexamp.s

mulexamp: mulexamp.s debug.s
	clang $(LDFLAGS) -o mulexamp mulexamp.s

matrixmult: matrixmult.s
	clang $(LDFLAGS) -g -o matrixmult matrixmult.s

clean: 
	rm -rf divexamp matrixmult mulexamp