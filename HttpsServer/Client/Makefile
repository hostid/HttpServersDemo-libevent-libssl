# 适用与.h与.c处于同一文件的工程
SRC = $(wildcard *.cpp)
OBJ = $(patsubst %.cpp,%.o,$(notdir ${SRC}))

TARGET = login
CC = g++
CFLAGS = -Wall 
LIB = 

# 调试阶段加-g参数，确定后去掉该参数
${TARGET}:${OBJ}
	$(CC) $(OBJ) -o  $@ $(LIB)
%.o:%.c
	$(CC) $(CFLAGS) -c $< -o $@ 
clean:
	rm *.o ${TARGET}