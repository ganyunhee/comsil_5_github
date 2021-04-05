cc = g++
cflags = -w -g
objects = main.o array.o rangearray.o
target = main


$(target) : $(objects)
	$(cc) $(cflags) -o $(target) $(objects)

%.o : %.cpp
	$(cc) $(cflags) -c -o $@ $<

main.o array.o rangearray.o : Array.h RangeArray.h

.PHONY : clean

clean :
	rm *.o $(target)
