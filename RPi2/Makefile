CC=gcc
CFLAGS= -c -Wall
LDFLAGS= -lpthread 
SOURCES=RPi2.c WiringPi/wiringPi/wiringPi.c WiringPi/wiringPi/wiringPiI2C.c WiringPi/wiringPi/piHiPri.c 
OBJECTS=$(SOURCES:.c=.o)
EXECUTABLE=RPi3

all: $(SOURCES) $(EXECUTABLE)

$(EXECUTABLE): $(OBJECTS)
	$(CC) $(LDFLAGS) $(OBJECTS) -o $@
	
.c.o:
	$(CC) $(CFLAGS) $< -o $@

clean: 
	rm -rf *.o $(EXECUTABLE)
