# phony target
.PHONY: all
.PHONY: clean

# compile target
all: server client

# compile flags
CFLAGS 	= -g -Wall
CC 	= gcc

# compile
server: server.o
	$(CC) $(CFLAGS) -o server server.o

client: client.o
	$(CC) $(CFLAGS) -o client client.o

server.o: network_socket.h
client.o: network_socket.h

clean:
	-rm -f *.o  server client
