IF (NODEJS_COMPILE)

	## INSTALL ##

	# Install script
	INSTALL (FILES ${CMAKE_CURRENT_SOURCE_DIR}/run.js DESTINATION share/jderobot/webtools/cameraviewjs COMPONENT webtools )

	# Install public
	INSTALL (DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/public DESTINATION share/jderobot/webtools/cameraviewjs COMPONENT webtools PATTERN .svn EXCLUDE)


ENDIF()