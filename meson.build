project('STM32-Starter', ['c', 'cpp'], default_options : ['cpp_std=gnu++17', 'c_std=gnu11'])
source_files = []
incdir = []
deps = []

if meson.is_cross_build()
    subdir('cross-compile')
endif

subdir('src')


