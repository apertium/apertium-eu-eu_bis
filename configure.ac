#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.


AC_PREREQ(2.52)

AC_INIT([Apertium Basque-Biscayan Basque], [0.3.1], [sortiz@users.sourceforge.net], [apertium-eu-eu_bis])
AM_INIT_AUTOMAKE
AC_PROG_AWK

PKG_CHECK_MODULES(APERTIUM, apertium >= 3.6.1)
PKG_CHECK_MODULES(LTTOOLBOX, lttoolbox >= 3.5.1)


AC_PATH_PROG(XSLTPROC, xsltproc, no)
if test x$ac_cv_path_XSLTPROC = x
then
  AC_MSG_ERROR([You don't have xsltproc installed.])
fi
if test x$ac_cv_path_XSLTPROC = xno
then
  AC_MSG_ERROR([You don't have xsltproc installed.])
fi

AP_MKINCLUDE

AC_OUTPUT([Makefile])
