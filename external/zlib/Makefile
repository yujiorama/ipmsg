CC      = gcc
AR      = ar
SRCDIR	= .
OBJDIR	= .
TARGET  = libzlib.a
DEST	= ./
LIBS	= 
CFLAGS	= -Wall -g -O0
LDFLAGS =
ARFLAGS = rc

SRCS=\
$(SRCDIR)/adler32.c  \
$(SRCDIR)/compress.c  \
$(SRCDIR)/crc32.c  \
$(SRCDIR)/deflate.c  \
$(SRCDIR)/gzio.c  \
$(SRCDIR)/infback.c  \
$(SRCDIR)/inffast.c  \
$(SRCDIR)/inflate.c  \
$(SRCDIR)/inftrees.c  \
$(SRCDIR)/trees.c  \
$(SRCDIR)/uncompr.c  \
$(SRCDIR)/zutil.c

OBJS=\
$(OBJDIR)/adler32.o  \
$(OBJDIR)/compress.o  \
$(OBJDIR)/crc32.o  \
$(OBJDIR)/deflate.o  \
$(OBJDIR)/gzio.o  \
$(OBJDIR)/infback.o  \
$(OBJDIR)/inffast.o  \
$(OBJDIR)/inflate.o  \
$(OBJDIR)/inftrees.o  \
$(OBJDIR)/trees.o  \
$(OBJDIR)/uncompr.o  \
$(OBJDIR)/zutil.o

all:	$(TARGET)

.c.o:
	$(CC) $(CFLAGS) -c $<

$(TARGET): $(OBJS)
	$(AR) $(ARFLAGS) $@ $(OBJS)

clean:
	@rm -f $(OBJS) $(TARGET)
