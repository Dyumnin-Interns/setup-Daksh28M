SIM ?= icarus
TOPLEVEL_LANG ?= verilog
VERILOG_SOURCES += $(PWD)/../hdl/dut.v
VERILOG_SOURCES += $(PWD)/wrappers/dut_test.v
TOPLEVEL = dut_test
MODULE = dut_test
all: setup

setup:
	rm -rf sim_build
	$(MAKE) sim MODULE=$(MODULE) TOPLEVEL=$(TOPLEVEL)

include $(shell cocotb-config --makefiles)/Makefile.sim
