add_subdirectory(determinant)

SET(DGTAL_EXAMPLES_SRC
  examplePreimage
)


FOREACH(FILE ${DGTAL_EXAMPLES_SRC})
  add_executable(${FILE} ${FILE})
  target_link_libraries (${FILE} DGtal DGtalIO )
ENDFOREACH(FILE)



