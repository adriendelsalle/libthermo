project('libthermo', 'cpp', 
        default_options : ['cpp_std=c++17'])

xtensor = dependency('xtensor')

libthermo = declare_dependency(
    include_directories: include_directories('.'),
    dependencies: xtensor
)

install_headers(
    'libthermo/thermo.hpp',
    'libthermo/exceptions.hpp',
    'libthermo/ideal_gas.hpp',
    'libthermo/poly_gas.hpp',
    'libthermo/math_utils.hpp',
    'libthermo/type_traits.hpp',
    'libthermo/version.hpp',
    'libthermo/detail/ideal_gas_xt_impl.hpp',
    'libthermo/detail/poly_gas_xt_impl.hpp',
    'libthermo/detail/polyval.hpp',
    preserve_path: true
)

subdir('tests')
