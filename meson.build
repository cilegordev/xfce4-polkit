project('xfce4-polkit', 'c', version : '0.3.1')

prefix = get_option('prefix')
libexecdir = join_paths(prefix, get_option('libexecdir'))
sysconfdir = join_paths(prefix, get_option('sysconfdir'))
autostartdir = join_paths(sysconfdir, 'xdg', 'autostart')

deps = [
  dependency('glib-2.0'),
  dependency('libxfce4ui-2'),
  dependency('polkit-agent-1'),
]

sources = files([
  'src/xfce4-polkit.c',
  'src/xfce4-polkit-listener.c',
])

executable('xfce4-polkit-authentication-agent-1', sources,
  dependencies: deps,
  install: true,
  install_dir: libexecdir
)

desktopconf = configuration_data()
desktopconf.set('xfce_polkit_libexecdir', libexecdir)
configure_file(
  input: 'xfce4-polkit-authentication-agent-1.desktop.in',
  output: 'xfce4-polkit-authentication-agent-1.desktop',
  configuration: desktopconf,
  install_dir: autostartdir
)
