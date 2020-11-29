
# ---- can use a variable to easily change the compiler (ex: gcc --> clang) ----
CC=gcc

# ---- the specific keyword 'all' is the default and you can just type "make" to use this config ----
all: test_c 

#  ---- compile but do not link ----
example_objfile: example.c
	$(CC) -c example.c -o example.o

test_objfile: test.c
	$(CC) -c test.c -o test.o


# ---- compile and link ----
example: example.c
	$(CC) example.c -o example

test_c: test.c
	$(CC) test.c -o test

# ---- deletes all the executables and object files ----
clean:
	rm example test example.o test.o

