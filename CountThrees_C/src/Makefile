test: ServerCountThrees.o readInt32BitLE.o directories
	gcc ServerCountThrees.o readInt32BitLE.o -o ServerCountThrees
	cp ServerCountThrees ../build
	cp ../data/threesData.bin ../build
	exit	
ServerCountThrees.o: ServerCountThrees.c readInt32BitLE.h
	gcc -I . -c ServerCountThrees.c
readInt32BitLE.o: readInt32BitLE.c readInt32BitLE.h
	gcc -I . -c readInt32BitLE.c
directories:
	mkdir -p ../build
clean:
	rm -rf *.o
	rm ServerCountThrees
	rm -r ../build
