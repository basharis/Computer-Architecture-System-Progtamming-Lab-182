PROG = my_elf

CC = gcc
LD = gcc

LDFLAGS = -g -Wall
CCFLAGS = -g -Wall -c -m64

OBJS = task2.o

# All Targets
all: $(PROG)

# Tool invocations
# Executable "main" depends on the files...

$(PROG): $(OBJS)
	$(LD) $(LDFLAGS) $(OBJS) -o $(PROG)

# Depends on the source and header files

task2.o: task2.c task2.h
	$(CC) $(CCFLAGS) task2.c -o task2.o
	
#tell make that "clean" is not a file name!
.PHONY: clean

#Clean the build directory
clean:
	rm -f *.o $(PROG)
