CC = gcc
CFLAGS = -Wall -Wextra -pedantic -std=c11
SRCS = main.c addition.c subtraction.c multiplication.c division.c
OBJS = $(SRCS:.c=.o)
TARGET = calculator

all: $(TARGET)

$(TARGET): $(OBJS)
	$(CC) $(CFLAGS) -o $(TARGET) $(OBJS)

%.o: %.c operations.h
	$(CC) $(CFLAGS) -c $< -o $@

clean:
	rm -f $(OBJS) $(TARGET)

.PHONY: all clean

