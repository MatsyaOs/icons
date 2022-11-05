cmake_minimum_required(VERSION 3.5)
project(matsya-icons)

include(FeatureSummary)

install(DIRECTORY Matsya DESTINATION ${CMAKE_INSTALL_PREFIX}/share/icons)
install(DIRECTORY Matsya-dark DESTINATION ${CMAKE_INSTALL_PREFIX}/share/icons) 
