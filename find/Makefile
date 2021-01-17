include ../common.mk

CFLAGS += -D_GNU_SOURCE

find: find.c function.c ls.c main.c misc.c operator.c option.c getdate.c ../pwcache.o

getdate.c: getdate.y
	yacc $< -o $@

clean: clean-generated

clean-generated:
	$(RM) getdate.c
