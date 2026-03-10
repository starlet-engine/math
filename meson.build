project('starlet-math', 'cpp',
  version : '1.0.0',
  meson_version : '>=1.1',
  default_options : ['cpp_std=c++20']
)

inc = include_directories('inc')

starlet_math_dep = declare_dependency(
  include_directories : inc
)

if get_option('build_tests')
  gtest_dep = dependency('gtest_main',
    fallback : ['gtest', 'gtest_main_dep']
  )
  subdir('tests')
endif
