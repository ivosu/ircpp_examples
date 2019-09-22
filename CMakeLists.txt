cmake_minimum_required(VERSION 3.0)
project(ircpp_example CXX)

set(CMAKE_CXX_STANDARD 17)

add_subdirectory(ircpp)

add_executable(twitch_bot src/twitch_bot.cpp)
target_link_libraries(twitch_bot ircpp)
