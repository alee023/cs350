TARGET = flip flip.man
CC = gcc
CFLAGS = -Wall -DBSD –DNDEBUG

all:	$(TARGET)

flip:		flip.o
	$(CC) $(CFLAGS) –o $@ flip.o
	
flip.o:		flip.c flip.h
	$(CC) $(CFLAGS) –c flip.c
	
clean:
rm -rf *.o $(TARGET)