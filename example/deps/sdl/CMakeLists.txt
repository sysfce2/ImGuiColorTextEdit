#	TextEditor - A syntax highlighting text editor for ImGui
#	Copyright (c) 2024-2025 Johan A. Goossens. All rights reserved.
#
#	This work is licensed under the terms of the MIT license.
#	For a copy, see <https://opensource.org/licenses/MIT>.

set(BUILD_SHARED_LIBS OFF CACHE BOOL "" FORCE)

FetchContent_Populate(sdl QUIET GIT_REPOSITORY "https://github.com/libsdl-org/SDL" GIT_TAG "release-3.2.18")
add_subdirectory(${sdl_SOURCE_DIR} ${sdl_BINARY_DIR} EXCLUDE_FROM_ALL)
