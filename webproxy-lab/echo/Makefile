# Makefile for echo program 

CC = gcc
CFLAGS = -g -Wall
LDFLAGS = -lpthread

all: client server

client.o: echoclient.c ../csapp.h
	$(CC) $(CFLAGS) -c echoclient.c -o client.o

server.o: echoserveri.c ../csapp.h
	$(CC) $(CFLAGS) -c echoserveri.c -o server.o

client: client.o ../csapp.o
	$(CC) $(CFLAGS) client.o ../csapp.o -o client 

server: server.o ../csapp.o
	$(CC) $(CFLAGS) server.o ../csapp.o -o server 

clean:
	rm -f *~ *.o client server

