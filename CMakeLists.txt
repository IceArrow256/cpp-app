cmake_minimum_required(VERSION 3.20)

project(cpp-app VERSION 0.1.0)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

add_executable(cpp-app)

target_sources(cpp-app PRIVATE
              ${CMAKE_CURRENT_SOURCE_DIR}/src/main.cpp
	      )

target_include_directories(cpp-app PRIVATE
                          ${CMAKE_CURRENT_SOURCE_DIR}/include
			  )
