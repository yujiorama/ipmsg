CC      = gcc
AR      = ar
SRCDIR	= .
OBJDIR	= .
TARGET  = libpng.a
DEST	= ./
LIBS	= 
CFLAGS	= -Wall -g -O0
ARFLAGS = rc

SRCS=\
$(SRCDIR)/png.c \
$(SRCDIR)/pngerror.c \
$(SRCDIR)/pngget.c \
$(SRCDIR)/pngmem.c \
$(SRCDIR)/pngpread.c \
$(SRCDIR)/pngread.c \
$(SRCDIR)/pngrio.c \
$(SRCDIR)/pngrtran.c \
$(SRCDIR)/pngrutil.c \
$(SRCDIR)/pngset.c \
$(SRCDIR)/pngtest.c \
$(SRCDIR)/pngtrans.c \
$(SRCDIR)/pngwio.c \
$(SRCDIR)/pngwrite.c \
$(SRCDIR)/pngwtran.c \
$(SRCDIR)/pngwutil.c

OBJS=\
$(OBJDIR)/png.o \
$(OBJDIR)/pngerror.o \
$(OBJDIR)/pngget.o \
$(OBJDIR)/pngmem.o \
$(OBJDIR)/pngpread.o \
$(OBJDIR)/pngread.o \
$(OBJDIR)/pngrio.o \
$(OBJDIR)/pngrtran.o \
$(OBJDIR)/pngrutil.o \
$(OBJDIR)/pngset.o \
$(OBJDIR)/pngtest.o \
$(OBJDIR)/pngtrans.o \
$(OBJDIR)/pngwio.o \
$(OBJDIR)/pngwrite.o \
$(OBJDIR)/pngwtran.o \
$(OBJDIR)/pngwutil.o

all:	$(TARGET)

.c.o:
	$(CC) $(CFLAGS) -c $<

$(TARGET): $(OBJS)
	$(AR) $(ARFLAGS) $@ $(OBJS)

clean:
	@rm -f $(OBJS) $(TARGET)
