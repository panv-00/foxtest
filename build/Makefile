CPP=g++
CFLAGS=-Wall -O3 -g `pkg-config fox --cflags --libs`

VPATH=../src

OBJECTS= \

default: $(OBJECTS)
	$(CPP) -o ../foxtest ../src/foxtest.cpp \
		$(OBJECTS) \
		$(CFLAGS)

%.o: %.cpp %.h
	$(CPP) -c $< -o $*.o $(CFLAGS)
