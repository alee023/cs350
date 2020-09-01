TARGET = flip flip.man
CC = gcc
CFLAGS = -Wall -DBSD 
#–DNDEBUG giving issues

all:	$(TARGET)

flip:		flip.o
	$(CC) $(CFLAGS) –o $@ flip.o
	
flip.o:		flip.c flip.h
	
clean:
	rm -rf *.o $(TARGET)