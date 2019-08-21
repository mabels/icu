# Copyright (C) 2016 and later: Unicode, Inc. and others.
# License & terms of use: http://www.unicode.org/copyright.html#License
#
# Copyright (c) 2000-2002 IBM, Inc. and others
# sample code makefile

# Usage:
#  - configure, build, install ICU (make install)
#  - make sure "icu-config" (in the ICU installed bin directory) is on
#     the path
#  - do 'make' in this directory

#### definitions
# Name of your target
TARGET=numfmt.js

# All object files (C or C++)
OBJECTS=main.o util.o capi.o

#### rules
# Load in standard makefile definitions
include ../defs.mk

CC=emcc  -s TOTAL_MEMORY=32MB -s WASM=1 -s FORCE_FILESYSTEM=1 -s NODERAWFS=1
CXX=emcc  -s TOTAL_MEMORY=32MB -s WASM=1 -s FORCE_FILESYSTEM=1 -s NODERAWFS=1
CPPFLAGS=-I../../common -I../../i18n
CFLAGS=-I../../common -I../../i18n
CXXFLAGS=-I../../common -I../../i18n -std=c++11
LDFLAGS=-L../../lib

# the actual rules (this is a simple sample)
include ../rules.mk
