# See LICENSE for license details.
HLD_ROOT ?= ../../../../

DEBUG_FLAGS=-O3

USER_DEFS ?= -DSC_ACC -fopenmp
# -DGRAPHGEN
SOURCES=sc_main.cpp 
TARGET=ga_acc

SC_DIR ?= /p/hdk/rtl/cad/x86-64_linux26/accellera/systemc/2.3.0
SC_LIB ?= /p/hdk/rtl/cad/x86-64_linux26/accellera/systemc/2.3.0/release/linux_64/gcc_4.5.2/libsystemc.a

CFLAGS=${USER_DEFS} -g -I.. -I${HLD_ROOT}/pagerank-hybrid/gapbs/src/ -Wno-unknown-pragmas
LDFLAGS=-fopenmp
include $(HLD_ROOT)/common/Makefile.inc
