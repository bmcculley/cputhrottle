CC = /usr/bin/g++
CCFLAGS = -g
LDFLAGS =

CCFLAGS += -Wall -std=c++11

.cc.o:
	$(CC) -c $(CCFLAGS) $<

OBJS1 = cputhrottle.o manip.o
LIBS1 =
BINARY1 = cputhrottle
OBJS2 = test.o
LIBS2 =
BINARY2 = test

$(BINARY1): $(OBJS1)
	$(CC) $(LDFLAGS) -o $(BINARY1) $(OBJS1) $(LIBS1)

$(BINARY2): $(OBJS2)
	$(CC) $(LDFLAGS) -o $(BINARY2) $(OBJS2) $(LIBS)

all: $(BINARY1) $(BINARY2)

clean:
	rm -f *.o core $(BINARY1) $(BINARY2)
