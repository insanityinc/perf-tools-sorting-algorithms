# source files.
SRC = sort.c main.c

OBJ = $(SRC:.cpp=.o)

OUT = sort

# include directories
INCLUDES = -I.

# C compiler flags
CCFLAGS = -g -Wall

# compiler
CCC = gcc

.SUFFIXES: .cpp .c


default: $(OUT)

.cpp.o:
	$(CCC) $(CCFLAGS) $(INCLUDES)  -c $< -o $@

.c.o:
	$(CCC) $(CCFLAGS) $(INCLUDES) -c $< -o $@

$(OUT): $(OBJ)
	$(CCC) -o $(OUT) $(CCFLAGS) $(OBJ)

depend:  dep
#
#dep:
#	makedepend -- $(CFLAGS) -- $(INCLUDES) $(SRC)

clean:
	rm -f *.o .a *~ Makefile.bak $(OUT)
