idf_component_register(
    SRCS
        "decoder/src/ir_decode.c"
        "decoder/src/ir_utils.c"
        "decoder/src/ir_tv_control.c"
        "decoder/src/ir_ac_apply.c"
        "decoder/src/ir_ac_build_frame.c"
        "decoder/src/ir_ac_parse_parameter.c"
        "decoder/src/ir_ac_parse_forbidden_info.c"
        "decoder/src/ir_ac_parse_frame_info.c"
        "decoder/src/ir_ac_control.c"
        "decoder/src/ir_ac_binary_parse.c"
    INCLUDE_DIRS
        "decoder/src/include"
)

target_compile_options(${COMPONENT_LIB} PRIVATE -Wno-error -Wno-type-limits -Wno-sign-compare)
