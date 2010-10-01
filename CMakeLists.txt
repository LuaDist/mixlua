# Copyright (C) 2007-2009 LuaDist.
# Created by Peter Drahoš
# Redistribution and use of this file is allowed according to the terms of the MIT license.
# For details see the COPYRIGHT file distributed with LuaDist.
# Please note that the package source code is licensed under its own license.

PROJECT(mixlua C)
CMAKE_MINIMUM_REQUIRED(VERSION 2.8)
INCLUDE(dist.cmake)

# Build
ADD_LUA_MODULE(mixlua mixlua.c mixlua.def)

# Install all files and documentation
INSTALL (TARGETS mixlua DESTINATION ${INSTALL_CMOD})
INSTALL (FILES README VERSION DESTINATION ${INSTALL_DATA})
INSTALL (FILES test.lua DESTINATION ${INSTALL_TEST})
