CFLAGS = -c -Wall
CC = gcc
LIBS =  -lm 

all: main

main: main.o parser.o scanner.o reader.o charcode.o token.o error.o symtab.o debug.o semantics.o
	${CC} main.o parser.o scanner.o reader.o charcode.o token.o error.o symtab.o  debug.o semantics.o -o main

main.o: main.c
	${CC} ${CFLAGS} main.c

scanner.o: scanner.c
	${CC} ${CFLAGS} scanner.c

parser.o: parser.c
	${CC} ${CFLAGS} parser.c

reader.o: reader.c
	${CC} ${CFLAGS} reader.c

charcode.o: charcode.c
	${CC} ${CFLAGS} charcode.c

token.o: token.c
	${CC} ${CFLAGS} token.c

error.o: error.c
	${CC} ${CFLAGS} error.c

symtab.o: symtab.c
	${CC} ${CFLAGS} symtab.c

debug.o: debug.c
	${CC} ${CFLAGS} debug.c

semantics.o: semantics.c
	${CC} ${CFLAGS} semantics.c

clean:
	del /Q *.o *~ *.exe *~