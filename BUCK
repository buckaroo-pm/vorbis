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
  ])),
  compiler_flags = [
    '-std=c11',
  ],
  deps = [
    'buckaroo.github.buckaroo-pm.xiph-ogg//:ogg', 
  ], 
  visibility = [
    'PUBLIC',
  ],
)
