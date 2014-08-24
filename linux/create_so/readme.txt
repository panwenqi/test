这个目录是在linux创建so动态库示例程序
myfunction.h 是库的头文件
myfunction.c 是库函数的c文件

test_so.c 是调用so库的c程序,编译出的so文件要么放在 /lib 下， 要么加到环境变量中
