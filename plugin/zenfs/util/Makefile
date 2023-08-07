# ZenFS utility makefile

TARGET = zenfs

CC=g++
CPPFLAGS = $(shell pkg-config --cflags rocksdb) -I/home/jinyoung/rocksdb2
LIBS = $(shell pkg-config --static --libs rocksdb) -lzbd

all: $(TARGET)

$(TARGET): $(TARGET).cc
	$(CC) $(CPPFLAGS)  -o $(TARGET) $< $(LIBS)

clean:
	$(RM) $(TARGET)

