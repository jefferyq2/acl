base_path = ../../..
include ../../Makefile.in
#Path for SunOS
ifeq ($(findstring SunOS, $(UNIXNAME)), SunOS)
	EXTLIBS = -liconv
endif
ifeq ($(findstring FreeBSD, $(UNIXNAME)), FreeBSD)
	EXTLIBS = -L/usr/local/lib -liconv
endif
ifeq ($(findstring Darwin, $(UNIXNAME)), Darwin)
	EXTLIBS += -L/usr/lib -liconv
endif

PROG = server
EXTLIBS += -L../../../lib/linux64 -ldl -lz
