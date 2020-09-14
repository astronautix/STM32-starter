includes = []
includes += incdir

if meson.is_cross_build()
    source_files += cross_source_files
    includes += cross_includes
    deps += cross_deps
endif

if meson.is_cross_build()
    executable('blink_raw', [files('blink_raw.cpp'), cross_source_files], include_directories : includes,  dependencies : deps)

endif