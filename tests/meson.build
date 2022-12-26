gtest = dependency('gtest')

tests = executable('tests',
    'gtest_main.cpp',
    'test_ideal_gas.cc',
    'test_poly_gas.cc',
    dependencies: [libthermo, gtest],
    cpp_args : '-DLIBTHERMO_USE_XTENSOR'
)

test('unit tests', tests)
