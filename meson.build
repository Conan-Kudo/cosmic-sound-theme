project('COSMIC-Sounds',
        version: '1.2.0',
        meson_version: '>= 0.45',
        license : 'CC-BY-SA-4.0',
        default_options: ['prefix=/usr'])


theme_dir = join_paths(get_option('prefix'), 'share', 'sounds', 'COSMIC')

conf_data = configuration_data()
conf_data.set('ThemeName', 'COSMIC')

configure_file(input : 'src/index.theme.in',
              output : 'index.theme',
              configuration : conf_data,
              install_dir: theme_dir)

install_subdir('src/stereo', install_dir: theme_dir)
