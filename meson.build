project('strnatcmp', 'cpp', version: 'snapshot')

incdir = include_directories('include')
strnat_sources = ['src/strnatcmp.cpp']

libstrnatcmp = library('strnatcmp',
  strnat_sources,
  install: true,
  install_dir: '/usr/lib',
  include_directories: incdir
)

natsort_dep = declare_dependency(
  link_with: libstrnatcmp,
  include_directories: incdir
)