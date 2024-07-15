CC = gcc
CFLAGS = -Wall -O2
TARGET = myprogram

all: $(TARGET)

$(TARGET): main.c
    $(CC) $(CFLAGS) -o $(TARGET) main.c

clean:
    rm -f $(TARGET)
