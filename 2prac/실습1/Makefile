cc = gcc
objects = dog.o blackcow.o turtle.o main.o

animal.exe : dog.o blackcow.o turtle.o main.o
	$(cc) -o animal.exe dog.o blackcow.o turtle.o main.o

dog.o : dog.c
	$(cc) -c -o dog.o dog.c

blackcow.o : blackcow.c
	$(cc) -c -o blackcow.o blackcow.c

turtle.o : turtle.c
	$(cc) -c -o turtle.o turtle.c

main.o : main.c
	$(cc) -c -o main.o main.c

.PHONY : clean

clean :
	rm -f $(objects) animal.exe
	# -f --> to force clean process in case files do not exist due to unsuccessful build
