AC_INIT([xfce4-polkit], [0.3.1])
AM_INIT_AUTOMAKE([foreign])
AC_PROG_CC

PKG_CHECK_MODULES([GLIB], [glib-2.0])
PKG_CHECK_MODULES([LIBXFCE4UI], [libxfce4ui-2])
PKG_CHECK_MODULES([POLKIT_AGENT], [polkit-agent-1])

AC_CONFIG_FILES([
	Makefile
	src/Makefile
])

AC_OUTPUT
