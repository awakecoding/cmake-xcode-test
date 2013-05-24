
set(MODULE_NAME "APP")
set(MODULE_PREFIX "APP")

set(${MODULE_PREFIX}_SRCS app.c)

add_executable(${MODULE_NAME} ${${MODULE_PREFIX}_SRCS})

target_link_libraries(${MODULE_NAME} C)

