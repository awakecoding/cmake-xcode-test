
set(MODULE_NAME "A")
set(MODULE_PREFIX "A")

set(${MODULE_PREFIX}_SRCS a.c)

add_library(${MODULE_NAME} OBJECT ${${MODULE_PREFIX}_SRCS})

#target_link_libraries(${MODULE_NAME} ${${MODULE_PREFIX}_LIBS})

