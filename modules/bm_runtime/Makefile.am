AM_CPPFLAGS += \
-I$(top_srcdir)/modules/bm_sim/include \
-I$(top_builddir)/thrift_src/gen-cpp

if P4THRIFT
  AM_CPPFLAGS += -DP4THRIFT 
endif

AM_CXXFLAGS = $(PICKY_CXXFLAGS)
AM_CFLAGS = $(PICKY_CFLAGS)
noinst_LTLIBRARIES = libbmruntime.la

common_source = \
src/server.cpp \
src/Standard_server.ipp \
src/SimplePre_server.ipp \
src/SimplePreLAG_server.ipp

common_include = \
include/bm_runtime/bm_runtime.h

libbmruntime_la_SOURCES = $(common_source) $(common_include)
