JAVAC = javac
JVM = java
JFLAGS = -g
TARGET = MyApp
SOURCES = $(wildcard *.java)
CLASSES = $(SOURCES:.java=.class)

all: $(TARGET)

$(TARGET): $(CLASSES)

%.class: %.java
    $(JAVAC) $(JFLAGS) $<

run: $(TARGET)
    $(JVM) $(TARGET)

clean:
    rm -f $(CLASSES)
