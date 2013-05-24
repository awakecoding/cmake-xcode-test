
set(MODULE_NAME "B")
set(MODULE_PREFIX "B")

set(${MODULE_PREFIX}_SRCS b.c)

add_library(${MODULE_NAME} OBJECT ${${MODULE_PREFIX}_SRCS})

#target_link_libraries(${MODULE_NAME} ${${MODULE_PREFIX}_LIBS})


