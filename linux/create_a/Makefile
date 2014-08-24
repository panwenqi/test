#编译静态库 .a

libmyfunction.a:
	gcc -c myfunction.c
	ar rcs libmyfunction.a myfunction.o
	rm *.o

#调用静态库
test_a.out:
	gcc test_a.c -o test_a.out -L./ libmyfunction.a

clean:
	rm *.out *.a
