
# makefile to build a program

# program depends on components: name and main 
myname:      main.o name.o 
	g++ -g  main.o name.o -o myname

# name.cpp has it's own header file
name.o:        name.cpp name.h
	g++ -c -g  name.cpp

# main.cpp also uses the header file name.h
main.o:	       main.cpp name.h
	g++ -c -g main.cpp

backup:
	tar -czvf ddkeen.assignment4_1.tar.gz main.cpp Makefile name.cpp name.h readme

clean:
	/bin/rm -f myname *.o

