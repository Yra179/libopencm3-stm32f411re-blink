PROJECT = awesomesauce
BUILD_DIR = bin

CFILES = blink.c

# TODO - you will need to edit these two lines!
DEVICE=stm32f411ret6
#OOCD_FILE = board/stm32f4discovery.cfg

# You shouldn't have to edit anything below here.
VPATH += $(SHARED_DIR)
INCLUDES += $(patsubst %,-I%, . $(SHARED_DIR))
OPENCM3_DIR=../libopencm3

include $(OPENCM3_DIR)/mk/genlink-config.mk
include ../rules.mk
include $(OPENCM3_DIR)/mk/genlink-rules.mk

STFLASH		= $(shell which st-flash)

stlink-flash:
	@printf "  FLASH  $<\n"
	$(STFLASH) write awesomesauce.bin 0x8000000
