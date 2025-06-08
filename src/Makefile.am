
NULL=

libexec_PROGRAMS = xfce4-polkit-authentication-agent-1
xfce4_polkit_authentication_agent_1_SOURCES = \
	xfce4-polkit.c \
	xfce4-polkit-listener.c \
	xfce4-polkit-listener.h \
	$(NULL)

xfce4_polkit_authentication_agent_1_CFLAGS = @GLIB_CFLAGS@ \
	@LIBXFCE4UI_CFLAGS@ \
	@POLKIT_AGENT_CFLAGS@


xfce4_polkit_authentication_agent_1_LDADD = @GLIB_LIBS@ \
	@LIBXFCE4UI_LIBS@ \
	@POLKIT_AGENT_LIBS@


#xfce-polkit-listener.o: xfce-polkit-listener.h

