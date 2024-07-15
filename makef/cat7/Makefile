CC = gcc
AS = nasm
CFLAGS = -Wall -O2
ASFLAGS = -f elf64
TARGET = myprogram
OBJS = main.o asmfunc.o

all: $(TARGET)

$(TARGET): $(OBJS)
    $(CC) $(CFLAGS) -o $(TARGET) $(OBJS)

asmfunc.o: asmfunc.asm
    $(AS) $(ASFLAGS) asmfunc.asm -o asmfunc.o

clean:
    rm -f $(TARGET) $(OBJS)
