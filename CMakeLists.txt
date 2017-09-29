cmake_minimum_required(VERSION 3.8)
project(libmbus)

set(CMAKE_CXX_STANDARD 11)

set(SOURCE_FILES
        bin/mbus-serial-request-data-multi-reply.c
        bin/mbus-serial-request-data.c
        bin/mbus-serial-scan-secondary.c
        bin/mbus-serial-scan.c
        bin/mbus-serial-select-secondary.c
        bin/mbus-serial-switch-baudrate.c
        bin/mbus-tcp-application-reset.c
        bin/mbus-tcp-raw-send.c
        bin/mbus-tcp-request-data-multi-reply.c
        bin/mbus-tcp-request-data.c
        bin/mbus-tcp-scan-secondary.c
        bin/mbus-tcp-scan.c
        bin/mbus-tcp-select-secondary.c
        libltdl/libltdl/lt__alloc.h
        libltdl/libltdl/lt__argz_.h
        libltdl/libltdl/lt__dirent.h
        libltdl/libltdl/lt__glibc.h
        libltdl/libltdl/lt__private.h
        libltdl/libltdl/lt__strl.h
        libltdl/libltdl/lt_dlloader.h
        libltdl/libltdl/lt_error.h
        libltdl/libltdl/lt_system.h
        libltdl/libltdl/slist.h
        libltdl/loaders/dld_link.c
        libltdl/loaders/dlopen.c
        libltdl/loaders/dyld.c
        libltdl/loaders/load_add_on.c
        libltdl/loaders/loadlibrary.c
        libltdl/loaders/preopen.c
        libltdl/loaders/shl_load.c
        libltdl/lt__alloc.c
        libltdl/lt__argz.c
        libltdl/lt__dirent.c
        libltdl/lt__strl.c
        libltdl/lt_dlloader.c
        libltdl/lt_error.c
        libltdl/ltdl.c
        libltdl/ltdl.h
        libltdl/slist.c
        mbus/mbus-protocol-aux.c
        mbus/mbus-protocol-aux.h
        mbus/mbus-protocol.c
        mbus/mbus-protocol.h
        mbus/mbus-serial.c
        mbus/mbus-serial.h
        mbus/mbus-tcp.c
        mbus/mbus-tcp.h
        mbus/mbus.c
        mbus/mbus.h
        test/mbus_parse.c
        test/mbus_parse_hex.c
        config.h)

include_directories(.)

add_executable(libmbus ${SOURCE_FILES})