SUBDIRS = src

NULL=

desktopdir=$(sysconfdir)/xdg/autostart
desktop_in_files = \
	xfce4-polkit-authentication-agent-1.desktop.in \
	$(NULL)

desktop_DATA = $(desktop_in_files:.desktop.in=.desktop)

EXTRA_DIST = \
	$(desktop_in_files) \
	$(NULL)

xfce4-polkit-authentication-agent-1.desktop: xfce4-polkit-authentication-agent-1.in
	sed -e 's,@xfce_polkit_libexecdir@,$(libexecdir),' $< > $@

clean-local:
	-rm -f xfce4-polkit-authentication-agent-1.desktop
