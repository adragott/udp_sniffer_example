CC=gcc
CFLAGS= -std=gnu11 -O3 -Wall -Wunused $(INC)
INC= -I../inc/
DEPS=

OBJS= udp_client udp_server udp_sniffer

all: clean $(OBJECT) $(EXECUTABLE)
	$(CC) $(CFLAGS) ../src/udp_client.c -o udp_client $(DEPS)
	$(CC) $(CFLAGS) ../src/udp_server.c -o udp_server $(DEPS)
	$(CC) $(CFLAGS) ../src/udp_sniffer.c -o udp_sniffer $(DEPS)
	@chmod +x *
clean:
	-rm -f udp*
