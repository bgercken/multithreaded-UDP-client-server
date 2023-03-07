CC=g++
all: client.o client_func.o packet.o
	$(CC) client.o client_func.o packet.o -o client
client.o:
	$(CC) -c client.c -o client.o
client_func.o:
	$(CC) -c client_func.c -o client_func.o
packet.o:
	$(CC) -c packet.c -o packet.o
