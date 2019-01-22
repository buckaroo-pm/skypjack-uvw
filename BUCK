load('//:buckaroo_macros.bzl', 'buckaroo_deps_from_package')
load('//:subdir_glob.bzl', 'subdir_glob')

prebuilt_cxx_library(
  name = 'uvw',
  header_only = True,
  header_namespace = '',
  exported_headers = subdir_glob([
    ('src', '**/*.hpp'),
  ]),
  deps = buckaroo_deps_from_package('github.com/buckaroo-pm/libuv'),
  visibility = [
    'PUBLIC',
  ],
)
