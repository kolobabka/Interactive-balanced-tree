cmake_minimum_required (VERSION 3.16)

project ("Interactive balanced tree" VERSION 1.0.0)

set (EXEC_FILE "start")

set (HEADERS

	headers/tree.h
)

set (SOURCES 

	sources/main.c
	sources/tree.c
	sources/menu.c
)

add_executable (${EXEC_FILE} ${SOURCES})

target_include_directories (${EXEC_FILE} PRIVATE headers)

