
build: main.o libhello_lib.a
	g++ -o sayHello main.o -L. -lhello_lib

libhello_lib.a: hello_lib.o 
	ar cr libhello_lib.a hello_lib.o 

main.o hello_lib.o:
	g++ -c *.cpp

clean:
	rm -f *.o *.a sayHello