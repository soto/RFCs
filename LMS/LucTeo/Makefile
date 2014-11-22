
PROGRAM=hello_world
DEBUG_FLAGS=
OPT_LEVEL=-O2
INCLUDES=-I/usr/local/include
LIBS=-L/usr/local/lib -lczmq -lzmq
GCC=clang
RUN_ARGS=50000

OPTS=-O2

$(PROGRAM).out:  $(PROGRAM).o
	$(GCC) -o $(PROGRAM).out $(PROGRAM).o $(LIBS) $(OPT_LEVEL) $(DEBUG_FLAGS)

$(PROGRAM).o: $(PROGRAM).c
	$(GCC) -o $(PROGRAM).o $(PROGRAM).c -c $(OPT_LEVEL) $(CPP_FLAGS) $(INCLUDES)

all: $(PROGRAM).out

run: $(PROGRAM).out
	./$(PROGRAM).out $(RUN_ARGS)

clean:
	rm -f *~
	rm -f *.ll
	rm -f *.bc
	rm -f *.o
	rm -f *.out
