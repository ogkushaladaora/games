# Build file for OOP Project

.PHONY: all
all: full

#main:
#	g++ -std=c++11 -c main.cpp point.hpp point.cpp
#	g++ main.o -o main.x -lsfml-graphics -lsfml-window -lsfml-system

full: main.o point.o
	g++ main.o point.o -o main -lsfml-graphics -lsfml-window -lsfml-system

main.o: main.cpp
	g++ -std=c++11 -c main.cpp

point.o: point.cpp point.hpp
	g++ -std=c++ -c point.cpp point.hpp

.PHONY: run
run: runmain

runmain:
	./main.exe

.PHONY: clean
clean :
	@rm -f main.x main.o