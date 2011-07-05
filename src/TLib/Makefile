CC      = g++
AR      = ar
SRCDIR	= .
OBJDIR	= .
TARGET  = Tlib.a
DEST	= ./
LIBS	= 
CFLAGS	= -Wall -g -O0
ARFLAGS = rc
LDFLAGS =

SRCS=\
$(SRCDIR)/tapi32ex.cpp \
$(SRCDIR)/tapi32u8.cpp \
$(SRCDIR)/tapi32v.cpp \
$(SRCDIR)/tapp.cpp \
$(SRCDIR)/tdlg.cpp \
$(SRCDIR)/tini.cpp \
$(SRCDIR)/tlist.cpp \
$(SRCDIR)/tmisc.cpp \
$(SRCDIR)/tregist.cpp \
$(SRCDIR)/twin.cpp

OBJS=\
$(OBJDIR)/tapi32ex.o \
$(OBJDIR)/tapi32u8.o \
$(OBJDIR)/tapi32v.o \
$(OBJDIR)/tapp.o \
$(OBJDIR)/tdlg.o \
$(OBJDIR)/tini.o \
$(OBJDIR)/tlist.o \
$(OBJDIR)/tmisc.o \
$(OBJDIR)/tregist.o \
$(OBJDIR)/twin.o

all:	$(TARGET)

.cpp.o:
	$(CC) $(CFLAGS) -c $<

$(TARGET): $(OBJS)
	$(CC) $(LDFLAGS) $(OBJS) -o $@

clean:
	@rm -f $(OBJS) $(TARGET)
