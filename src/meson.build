plug_files = files(
    'Plug.vala',
    'Widgets/Sidebar.vala',
    'Widgets/SettingsOption.vala',
    'Widgets/SettingsHeader.vala',
    'Widgets/MainView.vala',
    'Widgets/Footer.vala',
    'Widgets/AppSettingsView.vala',
    'Widgets/AppList.vala',
    'Widgets/AppEntry.vala',
    'Backend/NotifySettings.vala',
    'Backend/NotifyManager.vala',
    'Backend/App.vala'
)

switchboard_dep = dependency('switchboard-2.0')

shared_module(
    meson.project_name(),
    plug_files,
    plug_resources,
    dependencies: [
        dependency('glib-2.0'),
        dependency('gio-2.0'),
        dependency('gobject-2.0'),
        dependency('granite'),
        dependency('gtk+-3.0'),
        switchboard_dep
    ],
    install: true,
    install_dir : join_paths(switchboard_dep.get_pkgconfig_variable('plugsdir'), 'personal')
)
