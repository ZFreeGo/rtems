## Process this file with autoconf to produce a configure script.

AC_PREREQ([2.69])
AC_INIT([rtems-c-src-lib-libbsp-mips-hurricane],[_RTEMS_VERSION],[https://devel.rtems.org/newticket])
AC_CONFIG_SRCDIR([make/custom/hurricane.cfg])
RTEMS_TOP(../../../../../..)

RTEMS_CANONICAL_TARGET_CPU
AM_INIT_AUTOMAKE([no-define nostdinc foreign 1.12.2])

RTEMS_BSP_CONFIGURE

RTEMS_PROG_CC_FOR_TARGET
RTEMS_CANONICALIZE_TOOLS
RTEMS_PROG_CCAS

RTEMS_BSPOPTS_SET([BSP_HAS_USC320],[*],[1])
RTEMS_BSPOPTS_HELP([BSP_HAS_USC320],
[This BSP has a V3 USC320 system controller chip.])

RTEMS_BSPOPTS_SET([BSP_HAS_RM52xx],[*],[1])
RTEMS_BSPOPTS_HELP([BSP_HAS_RM52xx],
[This BSP has a RM52xx compatible CPU.])

RTEMS_BSP_CLEANUP_OPTIONS

# Explicitly list all Makefiles here
AC_CONFIG_FILES([Makefile])
AC_OUTPUT
