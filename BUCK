load('//:buckaroo_macros.bzl', 'buckaroo_deps')

cxx_library(
  name = 'vorbis',
  header_namespace = '',
  exported_headers = subdir_glob([
    ('include', 'vorbis/**/*.h'),
  ]),
  headers = subdir_glob([
    ('lib', '**/*.h'),
  ]),
  srcs = glob([
    'lib/**/*.c',
  ],
  excludes = glob([
    'lib/psytune.c',
    'lib/barkmel.c',
  ])),
  deps = buckaroo_deps(),
  visibility = [
    'PUBLIC',
  ],
)
