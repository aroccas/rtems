
rtems_tests_PROGRAMS = spfatal06
spfatal06_SOURCES = ../spfatal_support/init.c ../spfatal_support/system.h testcase.h

dist_rtems_tests_DATA = spfatal06.scn
dist_rtems_tests_DATA += spfatal06.doc

include $(RTEMS_ROOT)/make/custom/@RTEMS_BSP@.cfg
include $(top_srcdir)/../automake/compile.am
include $(top_srcdir)/../automake/leaf.am


AM_CPPFLAGS += -I$(top_srcdir)/../support/include

LINK_OBJS = $(spfatal06_OBJECTS)
LINK_LIBS = $(spfatal06_LDLIBS)

spfatal06$(EXEEXT): $(spfatal06_OBJECTS) $(spfatal06_DEPENDENCIES)
	@rm -f spfatal06$(EXEEXT)
	$(make-exe)

include $(top_srcdir)/../automake/local.am
