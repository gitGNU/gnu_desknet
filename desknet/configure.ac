#                          -*- Autoconf -*-

# Copying and distribution of this file, with or without modification,
# are permitted in any medium without royalty provided the copyright
# notice and this notice are preserved.  This file is offered as-is,
# without any warranty.
# Process this file with autoconf to produce a configure script.

AC_PREREQ(2.61)
AC_INIT(dnet, 0.1, juanslayton@dslextreme.com)
AM_INIT_AUTOMAKE

AC_CONFIG_SRCDIR([src/dnet.c])
AC_CONFIG_HEADER([config.h])

# Checks for programs.
AC_PROG_CC
AC_PROG_INSTALL

# Checks for libraries.
# FIXME: Replace `main' with a function in `-lSDL2':
AC_CHECK_LIB([SDL2], [SDL_init()])
# FIXME: Replace `main' with a function in `-lSDL2_ttf':
AC_CHECK_LIB([SDL2_ttf], [main])

# FIXME: Replace `main' with a function in `-lrt':
AC_CHECK_LIB([rt], [main])


# Checks for header files.
AC_HEADER_STDC
AC_CHECK_HEADERS([fcntl.h stdlib.h string.h sys/ioctl.h unistd.h])

# Checks for typedefs, structures, and compiler characteristics.
AC_TYPE_SIZE_T
AC_HEADER_TIME

# Checks for library functions.
AC_PROG_GCC_TRADITIONAL
AC_FUNC_SELECT_ARGTYPES
AC_CHECK_FUNCS([select])

AC_CONFIG_FILES([Makefile
                 src/Makefile])
AC_OUTPUT
