﻿# Makefile generated by CMakefileGenerator.cs (v1.2)
# *DO NOT EDIT*

cmake_minimum_required (VERSION 2.6)
project (UE4)

# CMake Flags
set(CMAKE_CXX_STANDARD 14)
set(CMAKE_CXX_USE_RESPONSE_FILE_FOR_OBJECTS 1 CACHE BOOL "" FORCE)
set(CMAKE_CXX_USE_RESPONSE_FILE_FOR_INCLUDES 1 CACHE BOOL "" FORCE)

# Standard Includes
include("C:/Unreal Engine/unreal_projects/My_3rd_Person/Intermediate/ProjectFiles/cmake-includes.cmake")
include("C:/Unreal Engine/unreal_projects/My_3rd_Person/Intermediate/ProjectFiles/cmake-definitions.cmake")
include("C:/Unreal Engine/unreal_projects/My_3rd_Person/Intermediate/ProjectFiles/cmake-headers-ue4.cmake")
include("C:/Unreal Engine/unreal_projects/My_3rd_Person/Intermediate/ProjectFiles/cmake-headers-project.cmake")
include("C:/Unreal Engine/unreal_projects/My_3rd_Person/Intermediate/ProjectFiles/cmake-sources-engine.cmake")
include("C:/Unreal Engine/unreal_projects/My_3rd_Person/Intermediate/ProjectFiles/cmake-sources-project.cmake")
include("C:/Unreal Engine/unreal_projects/My_3rd_Person/Intermediate/ProjectFiles/cmake-csharp-engine.cmake")
include("C:/Unreal Engine/unreal_projects/My_3rd_Person/Intermediate/ProjectFiles/cmake-csharp-project.cmake")

# Optional Shader Include
include("C:/Unreal Engine/unreal_projects/My_3rd_Person/Intermediate/ProjectFiles/cmake-shaders-engine.cmake")
set_source_files_properties(${ENGINE_SHADER_FILES} PROPERTIES HEADER_FILE_ONLY TRUE)
include("C:/Unreal Engine/unreal_projects/My_3rd_Person/Intermediate/ProjectFiles/cmake-shaders-project.cmake")
set_source_files_properties(${PROJECT_SHADER_FILES} PROPERTIES HEADER_FILE_ONLY TRUE)
source_group("Shader Files" REGULAR_EXPRESSION .*.usf)

# Optional Config Include
include("C:/Unreal Engine/unreal_projects/My_3rd_Person/Intermediate/ProjectFiles/cmake-config-engine.cmake")
set_source_files_properties(${ENGINE_CONFIG_FILES} PROPERTIES HEADER_FILE_ONLY TRUE)
include("C:/Unreal Engine/unreal_projects/My_3rd_Person/Intermediate/ProjectFiles/cmake-config-project.cmake")
set_source_files_properties(${PROJECT_CONFIG_FILES} PROPERTIES HEADER_FILE_ONLY TRUE)
source_group("Config Files" REGULAR_EXPRESSION .*.ini)

add_custom_target(UE4Editor-Win64-DebugGame call "C:/Unreal Engine/UE_4.26/Engine/Build/BatchFiles/Build.bat" UE4Editor Win64 DebugGame  -game -progress -buildscw VERBATIM)
add_custom_target(UE4Editor-Win64-Shipping call "C:/Unreal Engine/UE_4.26/Engine/Build/BatchFiles/Build.bat" UE4Editor Win64 Shipping  -game -progress -buildscw VERBATIM)
add_custom_target(UE4Editor call "C:/Unreal Engine/UE_4.26/Engine/Build/BatchFiles/Build.bat" UE4Editor Win64 Development  -game -progress -buildscw VERBATIM)

add_custom_target(UE4Game-Win64-DebugGame call "C:/Unreal Engine/UE_4.26/Engine/Build/BatchFiles/Build.bat" UE4Game Win64 DebugGame  -game -progress -buildscw VERBATIM)
add_custom_target(UE4Game-Win64-Shipping call "C:/Unreal Engine/UE_4.26/Engine/Build/BatchFiles/Build.bat" UE4Game Win64 Shipping  -game -progress -buildscw VERBATIM)
add_custom_target(UE4Game call "C:/Unreal Engine/UE_4.26/Engine/Build/BatchFiles/Build.bat" UE4Game Win64 Development  -game -progress -buildscw VERBATIM)

add_custom_target(My_3rd_Person-Win64-DebugGame call "C:/Unreal Engine/UE_4.26/Engine/Build/BatchFiles/Build.bat" My_3rd_Person Win64 DebugGame "-project=C:/Unreal Engine/unreal_projects/My_3rd_Person/My_3rd_Person.uproject" -game -progress -buildscw VERBATIM)
add_custom_target(My_3rd_Person-Win64-Shipping call "C:/Unreal Engine/UE_4.26/Engine/Build/BatchFiles/Build.bat" My_3rd_Person Win64 Shipping "-project=C:/Unreal Engine/unreal_projects/My_3rd_Person/My_3rd_Person.uproject" -game -progress -buildscw VERBATIM)
add_custom_target(My_3rd_Person call "C:/Unreal Engine/UE_4.26/Engine/Build/BatchFiles/Build.bat" My_3rd_Person Win64 Development "-project=C:/Unreal Engine/unreal_projects/My_3rd_Person/My_3rd_Person.uproject" -game -progress -buildscw VERBATIM)

add_custom_target(My_3rd_PersonEditor-Win64-DebugGame call "C:/Unreal Engine/UE_4.26/Engine/Build/BatchFiles/Build.bat" My_3rd_PersonEditor Win64 DebugGame "-project=C:/Unreal Engine/unreal_projects/My_3rd_Person/My_3rd_Person.uproject" -game -progress -buildscw VERBATIM)
add_custom_target(My_3rd_PersonEditor-Win64-Shipping call "C:/Unreal Engine/UE_4.26/Engine/Build/BatchFiles/Build.bat" My_3rd_PersonEditor Win64 Shipping "-project=C:/Unreal Engine/unreal_projects/My_3rd_Person/My_3rd_Person.uproject" -game -progress -buildscw VERBATIM)
add_custom_target(My_3rd_PersonEditor call "C:/Unreal Engine/UE_4.26/Engine/Build/BatchFiles/Build.bat" My_3rd_PersonEditor Win64 Development "-project=C:/Unreal Engine/unreal_projects/My_3rd_Person/My_3rd_Person.uproject" -game -progress -buildscw VERBATIM)

add_executable(FakeTarget ${ENGINE_HEADER_FILES} ${ENGINE_SOURCE_FILES} ${ENGINE_CSHARP_FILES} ${ENGINE_SHADER_FILES} ${ENGINE_CONFIG_FILES} ${PROJECT_HEADER_FILES} ${PROJECT_SOURCE_FILES} ${PROJECT_CSHARP_FILES} ${PROJECT_SHADER_FILES} ${PROJECT_CONFIG_FILES})
