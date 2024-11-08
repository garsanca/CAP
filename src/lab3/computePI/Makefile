
MPICC=mpiicx
CC=icx
CFLAGS=-O2 -lm

all:
	$(CC)    -o piserial piserial.c $(CFLAGS)
	$(MPICC) -o piparallel piparallel.c $(CFLAGS)

run:
	mpirun -np 2 ./piparallel 10000

clean:
	rm -f piserial piparallel
