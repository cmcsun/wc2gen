EXE = wc2gen
PREFIX =


CC = $(PREFIX)gcc
AS = $(CC)
LD = $(CC)
AR = $(PREFIX)ar rcs
STRIP = $(PREFIX)strip
CP = cp -fp
RM = rm -f

CFLAGS = -O2
ASFLAGS =
LDFLAGS = 
ARFLAGS =


OBJS = wc2gen.o getopt.o


all: $(EXE)

.c.o:
	$(CC) $(CFLAGS) -c -o $@ $<

.S.o:
	$(AS) $(ASFLAGS) -c -o $@ $<

$(EXE): $(OBJS)
	$(LD) $(LDFLAGS) $(OBJS) -o $@

.PHONY: clean


clean:
	-$(RM) $(EXE)
	-$(RM) *.o




