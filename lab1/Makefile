TARGET = flip flip.man
CC = gcc
CFLAGS = -g -Wall -DBSD 
#–DNDEBUG giving issues

all:	$(TARGET)

$(TARGET): flip.o
	$(CC) $(CFLAGS) -o $@ flip.o
	
flip.o:		flip.c flip.h

flip:		flip.o
	$(CC) $(CFLAGS) –o $@ flip.o

flip.man:	
	nroff -man flip.1 > flip.man
	
clean:
	rm -rf *.o $(TARGET)