
set(MODULE_NAME "C")
set(MODULE_PREFIX "C")

add_subdirectory(A)
add_subdirectory(B)

add_library(${MODULE_NAME} SHARED $<TARGET_OBJECTS:A> $<TARGET_OBJECTS:B>)

set_target_properties(${MODULE_NAME} PROPERTIES LINKER_LANGUAGE C)
set_target_properties(${MODULE_NAME} PROPERTIES PREFIX "lib")

#list(REMOVE_DUPLICATES ${MODULE_PREFIX}_LIBS)
#target_link_libraries(${MODULE_NAME} ${${MODULE_PREFIX}_LIBS})

