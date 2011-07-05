CC      = g++
AR      = ar
SRCDIR	= .
OBJDIR	= .
TARGET  = Tlib.a
DEST	= ./
LIBS	= 
CFLAGS	= -Wall -g -O0
ARFLAGS = rc
LDFLAGS = -L../TLib -L../../externals/libpng -L../../externals/zlib -lTlib -Lpng -Lzlib

SRCS=\
$(SRCDIR)/aes.cpp \
$(SRCDIR)/blowfish.cpp \
$(SRCDIR)/cfg.cpp \
$(SRCDIR)/ipmsg.cpp \
$(SRCDIR)/logmng.cpp \
$(SRCDIR)/mainwin.cpp \
$(SRCDIR)/miscdlg.cpp \
$(SRCDIR)/miscfunc.cpp \
$(SRCDIR)/msgmng.cpp \
$(SRCDIR)/plugin.cpp \
$(SRCDIR)/pubkey.cpp \
$(SRCDIR)/recvdlg.cpp \
$(SRCDIR)/richedit.cpp \
$(SRCDIR)/senddlg.cpp \
$(SRCDIR)/setupdlg.cpp \
$(SRCDIR)/share.cpp \
$(SRCDIR)/version.cpp

OBJS=\
$(OBJDIR)/aes.o \
$(OBJDIR)/blowfish.o \
$(OBJDIR)/cfg.o \
$(OBJDIR)/ipmsg.o \
$(OBJDIR)/logmng.o \
$(OBJDIR)/mainwin.o \
$(OBJDIR)/miscdlg.o \
$(OBJDIR)/miscfunc.o \
$(OBJDIR)/msgmng.o \
$(OBJDIR)/plugin.o \
$(OBJDIR)/pubkey.o \
$(OBJDIR)/recvdlg.o \
$(OBJDIR)/richedit.o \
$(OBJDIR)/senddlg.o \
$(OBJDIR)/setupdlg.o \
$(OBJDIR)/share.o \
$(OBJDIR)/version.o \
$(OBJDIR)/ipmsg.res

all:	$(TARGET)

.cpp.o:
	$(CC) $(CFLAGS) -c $<

ipmsg.res: ipmsg.rc resource.h
	windres $< -O coff -o $@

$(TARGET): $(OBJS)
	$(CC) $(LDFLAGS) $(OBJS) -o $@

clean:
	@rm -f $(OBJS) $(TARGET)
