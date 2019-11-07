CROSS_COMPILE ?= arm-linux-

CC = $(CROSS_COMPILE)gcc
CFLAGS = -Wall -Wextra -Wfatal-errors -I ../include

VPATH = ../src

EXAMPLES += pcm-readi
EXAMPLES += pcm-writei

.PHONY: all
all: $(EXAMPLES)

pcm-readi: pcm-readi.c -ltinyalsa

pcm-writei: pcm-writei.c -ltinyalsa

.PHONY: clean
clean:
	rm -f $(EXAMPLES)

