project('strnatcmp', 'cpp', version: 'snapshot')

libstrnatcmp = static_library('strnatcmp',
  'strnatcmp.cpp',
  install: true,
  install_dir: join_paths(get_option('prefix'), get_option('includedir'), 'strnatcmp')
)

strnatcmp = declare_dependency(
  link_with: libstrnatcmp,
  include_directories: include_directories('.')
)

#For the test
executable('natsort', 
    'natsort.cpp',
    dependencies: strnatcmp,
)