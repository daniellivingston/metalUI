cmake_minimum_required(VERSION 3.14)

project(metalUI
    VERSION   0.1.0
    LANGUAGES Swift)

add_executable(metalUI
    src/App.swift
    src/ContentView.swift)

set_target_properties(metalUI
    PROPERTIES
        MACOSX_BUNDLE    TRUE
        WIN32_EXECUTABLE TRUE
        MACOSX_BUNDLE_GUI_IDENTIFIER
            my.example.com
        MACOSX_BUNDLE_BUNDLE_VERSION
            ${PROJECT_VERSION}
        MACOSX_BUNDLE_SHORT_VERSION_STRING
            ${PROJECT_VERSION_MAJOR}.${PROJECT_VERSION_MINOR}
)

