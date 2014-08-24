#编译动态库


libmyfunction.so:
	gcc myfunction.c -fPIC -shared -o libmyfunction.so

# -shared该选项指定生成动态连接库（让连接器生成T类型的导出符号表，有时候也生成弱连接W类型的导出符号），不用该标志外部程序无法连接。相当于一个可执行文件
# -fPIC：表示编译为位置独立的代码，不用此选项的话编译后的代码是位置相关的所以动态载入时是通过代码拷贝的方式来满足不同进程的需要，而不能达到真正代码段共享的目的


#====================================
#链接.so
testso:
	gcc test_so.c -o test_so.out  libmyfunction.so
clean:
	rm *.out *.so
