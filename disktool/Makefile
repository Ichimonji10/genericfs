#
# FILE        : Makefile
# AUTHOR      : (C) Copyright 2011 by Peter C. Chapin
# SUBJECT     : Makefile for the disktool project.
#

CFLAGS= -Wall -g -I../driver
OBJS  = createdir.o    \
	disktool.o     \
	initialize.o   \
	showfreemaps.o \
	showinode.o    \
	showblock.o    \
	showfile.o     \
	showrootdir.o  \
	tool.o         \
	util.o         \
	createfile.o   \
	verify.o
LDLIBS = -lncurses

all:	disktool

# Dependency lists for the various object files.
COMMON_DEPS = tool.h ../driver/genericfs.h

createdir.o:	createdir.c $(COMMON_DEPS)

createfile.o:   createfile.c $(COMMON_DEPS)

disktool.o:	disktool.c $(COMMON_DEPS)

initialize.o:	initialize.c $(COMMON_DEPS)

showfreemaps.o:	showfreemaps.c $(COMMON_DEPS)

showinode.o:	showinode.c $(COMMON_DEPS)

showblock.o:	showblock.c $(COMMON_DEPS)

showfile.o:	showfile.c $(COMMON_DEPS)

showrootdir.o:	showrootdir.c $(COMMON_DEPS)

tool.o:		tool.c $(COMMON_DEPS)

util.o:		util.c $(COMMON_DEPS)

verify.o:	verify.c $(COMMON_DEPS)

# Executable depends on the object files.
disktool:	$(OBJS)

# Clean up the mess.
clean:
	rm -rf disktool *.o *~ core
