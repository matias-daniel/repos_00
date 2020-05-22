SOURCES := $(wildcard *.cpp)
OBJECTS := $(subst .cpp,.o,$(SOURCES))
INCLUDE := -I.
CC      := g++

main: ${OBJECTS}
	$(CC) -o $@ $^

%.o: %.cpp
	$(CC) -o $@ -c $^ $(INCLUDE)

info:
	$(info $(SOURCES))
	$(info $(OBJECTS))

clean:
	rm -f main *.o

run: main
	./main.exe
