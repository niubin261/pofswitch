cmake_minimum_required(VERSION 3.6)
project(pofswitch2)

set(CMAKE_CXX_STANDARD 11)

set(SOURCE_FILES
        common/pof_basefunc.c
        common/pof_byte_transfer.c
        common/pof_command.c
        common/pof_hmap.c
        common/pof_list.c
        common/pof_log_print.c
        common/pof_memory.c
        common/pof_tree.c
        datapath/pof_action.c
        datapath/pof_datapath.c
        datapath/pof_instruction.c
        include/pof_byte_transfer.h
        include/pof_command.h
        include/pof_common.h
        include/pof_conn.h
        include/pof_datapath.h
        include/pof_global.h
        include/pof_hmap.h
        include/pof_list.h
        include/pof_local_resource.h
        include/pof_log_print.h
        include/pof_memory.h
        include/pof_protocol_header.h
        include/pof_switch_listen.h
        include/pof_tree.h
        include/pof_type.h
        local_resource/pof_counter.c
        local_resource/pof_flow_table.c
        local_resource/pof_group.c
        local_resource/pof_ins_block.c
        local_resource/pof_local_resource.c
        local_resource/pof_meter.c
        local_resource/pof_port.c
        switch_control/pof_config.c
        switch_control/pof_encap.c
        switch_control/pof_parse.c
        switch_control/pof_sctrl.c
        switch_control/pof_switch.c
        switch_control/pof_switch_listen.c)

add_executable(pofswitch2 ${SOURCE_FILES})