PRIVDIR := ../priv

OBJ=

all : $(PRIVDIR)/dthread_drv.so

override CFLAGS += -fpic -shared

OBJ := dlib.o dterm.o dthread.o dthread_drv.o

$(PRIVDIR)/dthread_drv.so : $(OBJ)
	$(CC) -shared -fpic $(LDFLAGS) -o $@ $^

lean:
	$(RM) -f $(PRIVDIR)/dthread_drv.so $(OBJ)
