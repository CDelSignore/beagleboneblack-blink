#   makefile for Beaglebone
#   ECE-231 Spring 2023
#
#	Date		Author			Revision
#	04/13/23    C. DelSignore   initial code creation

TARGET  := ece231_led_cl
CC      := gcc
#CFLAGS := -I $(INC_DIR)

# /part2/
#   ├── /bin/
#   │    ├── ece231_led_cl.elf
#   │    ├── makefile
#   │    └── test.sh
#   └── /src/
#        ├── ece231_led_cl.c
#        └── any other source files

BIN_DIR := ../bin
SRC_DIR := ../src
# INC_DIR := ../inc
# EXT_DIR := ../ext

# Find all .c files in the src and ext directories
SRC = $(wildcard $(SRC_DIR)/*.c)
# SRC += $(wildcard $(EXT_DIR)/*.c)

begin: $(TARGET).elf

$(TARGET).elf: $(SRC)
	$(CC) -o $(BIN_DIR)/$(TARGET).elf $(SRC)

# Remove all executable files
clean:
	@rm -f $(wildcard *.elf)