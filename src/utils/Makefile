
CC = gcc
CFLAGS = -Wall -Wstrict-prototypes -Werror

all: lpcchksum genhdr

genhdr: genhdr.o
	$(CC) $(CFLAGS) $^ --output $@

lpcchksum: lpcchksum.o
	$(CC) $(CFLAGS) $^ --output $@

%.o: %.c
	$(CC) -c $(CFLAGS) $< -o $@

clean:
	rm -f genhdr.o genhdr
	rm -f lpcchksum.o lpcchksum

