CC = gcc
CFLAGS = -g -Wall -DBSD -DNDEBUG

all:	flip flip.man

flip.o:		flip.c flip.h

flip:		flip.o
	$(CC) $(CFLAGS) -o $@ flip.o

flip.man:	
	nroff -man flip.1 > flip.man
	
clean:
	rm -rf *.o flip