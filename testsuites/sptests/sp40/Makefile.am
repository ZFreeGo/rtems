
rtems_tests_PROGRAMS = sp40
sp40_SOURCES = init.c

dist_rtems_tests_DATA = sp40.scn
dist_rtems_tests_DATA += sp40.doc

include $(RTEMS_ROOT)/make/custom/@RTEMS_BSP@.cfg
include $(top_srcdir)/../automake/compile.am
include $(top_srcdir)/../automake/leaf.am


AM_CPPFLAGS += -I$(top_srcdir)/../support/include

LINK_OBJS = $(sp40_OBJECTS)
LINK_LIBS = $(sp40_LDLIBS)

sp40$(EXEEXT): $(sp40_OBJECTS) $(sp40_DEPENDENCIES)
	@rm -f sp40$(EXEEXT)
	$(make-exe)

include $(top_srcdir)/../automake/local.am
