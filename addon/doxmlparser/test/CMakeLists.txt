
include_directories(
	../include
	${PROJECT_SOURCE_DIR}/qtools
)

add_executable(doxmlparser_test
main.cpp
)


target_link_libraries(doxmlparser_test
	doxmlparser
	qtools
        ${COVERAGE_LINKER_FLAGS}
)
