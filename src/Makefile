# Minimal Makefile for CHOICE

all: label.exe

UPX=upx --8086
# if you don't want to use UPX set
#     UPX=-rem (DOS)
#   or
#     UPX=true (Unix)
# if you use UPX: then options are
#     --8086 for 8086 compatibility
#   or
#     --best for smallest

label.exe label.com: label.c
	$(CC) $(CFLAGS)$@ $^ $(LDFLAGS)
	$(UPX) $@

clean:
	$(RM) label.exe
	$(RM) label.com
	$(RM) *.o
	$(RM) *.obj
