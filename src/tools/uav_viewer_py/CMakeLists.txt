

## INSTALL ##

# Install .py
FILE(GLOB_RECURSE HEADERS_FILES ${CMAKE_CURRENT_SOURCE_DIR}/*py)
FOREACH(header ${HEADERS_FILES})
	INSTALL(FILES ${header} DESTINATION share/jderobot/python/uav_viewer_py/ COMPONENT tools)
ENDFOREACH(header)

# Install gui
INSTALL (DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/gui DESTINATION share/jderobot/python/uav_viewer_py COMPONENT tools PATTERN .svn EXCLUDE)


