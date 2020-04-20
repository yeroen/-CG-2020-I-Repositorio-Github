CMAKE_MINIMUM_REQUIRED(VERSION "3.1")

PROJECT(CGproject2Triangulo)

SET(CGproject2Triangulo_CGproject2Triangulo "CGproject2Triangulo/main.cpp" "CGproject2Triangulo/glad.c")

LINK_DIRECTORIES(${CMAKE_SOURCE_DIR}/lib)

INCLUDE_DIRECTORIES("include")

MESSAGE("Se agrego libloteca exitosamente!")

ADD_EXECUTABLE(CGproject2Triangulo ${CGproject2Triangulo_CGproject2Triangulo})

TARGET_LINK_LIBRARIES(CGproject1 PUBLIC glfw3)
TARGET_LINK_LIBRARIES(CGproject1 PUBLIC opengl32)
