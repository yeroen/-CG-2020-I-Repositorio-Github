CMAKE_MINIMUM_REQUIRED(VERSION "3.17.0")

PROJECT(CGproject1)

SET(CGproject1_CGproject1 "CGproject1/main.cpp" "CGproject1/glad.c")

LINK_DIRECTORIES(${CMAKE_SOURCE_DIR}/lib)

INCLUDE_DIRECTORIES("include")

MESSAGE("Se agrego libloteca exitosamente!")

ADD_EXECUTABLE(CGproject1 ${CGproject1_CGproject1})

TARGET_LINK_LIBRARIES(CGproject1 PUBLIC glfw3)
TARGET_LINK_LIBRARIES(CGproject1 PUBLIC opengl32)
