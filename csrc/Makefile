MKDIR_P      := mkdir -p
RM           := rm
CC           := cc
CC_FLAGS     := -fPIC -shared -o
SRC_FILES    := ./local_metrics.c

BUILD_D      := build
OUT_LIB      := ${BUILD_D}/liblocal.so

.PHONY: all clean build directories

all: build
directories:
	@${MKDIR_P} ${BUILD_D}

build: directories
	${CC} ${CC_FLAGS} ${OUT_LIB} ${SRC_FILES}

clean:
	rm -rf build/ *~
