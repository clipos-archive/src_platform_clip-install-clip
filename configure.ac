# SPDX-License-Identifier: LGPL-2.1-or-later
# Copyright © 2007-2018 ANSSI. All Rights Reserved.
AC_INIT([clip-install-clip],[2.3.11],[clipos@ssi.gouv.fr])
AM_INIT_AUTOMAKE([-Wall -Werror foreign])
AC_PROG_CC
AC_ARG_ENABLE([corerm],
[  --enable-corerm      only for CLIP client],
[case "${enableval}" in
  yes) corerm=true ;;
  no) corerm=false ;;
  *) AC_MSG_ERROR([bad value ${enableval} for --enable-corerm]) ;;
esac],[corerm=false])
AM_CONDITIONAL([CORERM], [test x$corerm = xtrue])
AC_CONFIG_HEADERS([config.h])
AC_CONFIG_FILES([Makefile scripts/Makefile man/man8/Makefile etc/init.d/Makefile lib/Makefile etc/admin/clip_install/Makefile etc/admin/clip_install/apt.conf.d/Makefile etc/clip_update/clip_install/Makefile])
AC_OUTPUT
