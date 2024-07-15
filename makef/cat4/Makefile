CXX = g++
CXXFLAGS = -std=c++17 -Wall -O3
TARGET = myprogram
OBJS = main.o utils.o

all: $(TARGET)

$(TARGET): $(OBJS)
    $(CXX) $(CXXFLAGS) -o $(TARGET) $(OBJS)

%.o: %.cpp
    $(CXX) $(CXXFLAGS) -c $< -o $@

clean:
    rm -f $(TARGET) $(OBJS)
