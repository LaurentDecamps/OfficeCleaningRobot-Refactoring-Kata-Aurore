set(SRC_LIB_NAME src)
set(SOURCES sample.cpp
        RobotCleaner.h
        RobotCleanerMain.h
        OfficeCleaner01/OrientationClasses.h
        OfficeCleaner01/RobotCleanerParser.h
        OfficeCleaner01/RobotCleaner.h
        OfficeCleaner01/Program.h)
add_library(${SRC_LIB_NAME} ${SOURCES})
target_sources(${SRC_LIB_NAME} PRIVATE ${SOURCES})
target_include_directories(${SRC_LIB_NAME} PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
