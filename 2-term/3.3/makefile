TARGET_1 = http-proxy
SRCS_1 = picohttpparser.c map.c pqueue.c http-proxy.c main.c

CC=gcc
RM=rm
CFLAGS= -g -w
LIBS=-lpthread
INCLUDE_DIR="."

all: ${TARGET_1}

${TARGET_1}: picohttpparser.h map.h pqueue.h http-proxy.h ${SRCS_1}
	${CC} ${CFLAGS} -I${INCLUDE_DIR} ${SRCS_1} ${LIBS} -o ${TARGET_1}

clean:
	${RM} -f *.o ${TARGET_1}
