cmake_minimum_required(VERSION 2.8.9)

fips_begin_lib(wren-vm)
    fips_include_directories(wren/src/include wren/src/vm wren/src/optional)
    fips_files(
        wren/src/optional/wren_opt_meta.c
        wren/src/optional/wren_opt_random.c)
    fips_src(wren/src/vm)
fips_end_lib()