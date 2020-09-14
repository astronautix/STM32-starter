
cross_source_files = []
cross_deps = []
cross_includes = []

add_global_link_arguments(
    '-mcpu=cortex-m4', '-mno-thumb-interwork', '-mfpu=fpv4-sp-d16', '-mfloat-abi=hard',
    '-Lcross-compile/stm32/', '-T'+meson.current_source_dir()+'/stm32f429.ld', 
    language: ['c', 'cpp'])

libopencm3 = subproject('libopencm3')
cross_deps += libopencm3.get_variable('libopencm3_stm32f4_dep')

cross_source_files = files('syscalls.c', 'sysmem.c')
