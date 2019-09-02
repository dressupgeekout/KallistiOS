
# Makefile stolen from the kmgenc program.

CFLAGS = -O2 -Wall -DINLINE=inline -I/usr/pkg/include
LDFLAGS = -s -lpng16 -ljpeg -lm -lz -L/usr/pkg/lib

all: dcbumpgen

dcbumpgen: dcbumpgen.o get_image.o get_image_jpg.o get_image_png.o readpng.o
	$(CC) -o $@ $+ $(LDFLAGS)

clean:
	rm -f dcbumpgen *.o

