all: main tests

main: *.o
	g++ main.o submodule.o -o main

tests: *.o
	g++ tests.o submodule.o -o tests

*.o:
	g++ -c src/*.cpp -Isrc
	g++ -c *.cpp -Isrc

clean:
	rm -f *.o

cleanAll: clean
	rm -f main tests