CC=g++

all: server.o thread.o server_func.o packet.o
	$(CC) server.o thread.o server_func.o packet.o -lpthread -o server
server_func.o:
	$(CC) -c server_func.c -o server_func.o
packet.o:
	$(CC) -c packet.c -o packet.o
thread.o: server_func.o packet.o
	$(CC) -c thread.c -o thread.o
server.o: thread.o server_func.o packet.o
	$(CC) -lpthread -c server.c -o server.o

