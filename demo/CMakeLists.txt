set(sts_src sts_util.c 
        sts_transport.c 
        sts_data.c
        sts_process.c
        sts_define.c
        sts_api.c
        main.c)

add_executable(sts_demo ${sts_src})
target_link_libraries(sts_demo curl json-c ssl crypto)
