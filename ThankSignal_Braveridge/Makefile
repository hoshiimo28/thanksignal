# This file was automagically generated by mbed.org. For more information, 
# see http://mbed.org/handbook/Exporting-to-GCC-ARM-Embedded

# cross-platform directory manipulation
ifeq ($(shell echo $$OS),$$OS)
    MAKEDIR = if not exist "$(1)" mkdir "$(1)"
    RM = rmdir /S /Q "$(1)"
else
    MAKEDIR = $(SHELL) -c "mkdir -p \"$(1)\""
    RM = $(SHELL) -c "rm -rf \"$(1)\""
endif

ifeq (,$(filter .build,$(notdir $(CURDIR))))
.SUFFIXES:
OBJDIR := .build
mkfile_path := $(abspath $(lastword $(MAKEFILE_LIST)))
MAKETARGET = $(MAKE) --no-print-directory -C $(OBJDIR) -f $(mkfile_path) \
		SRCDIR=$(CURDIR) $(MAKECMDGOALS)
.PHONY: $(OBJDIR) clean
all:
	+@$(call MAKEDIR,$(OBJDIR))
	+@$(MAKETARGET)
$(OBJDIR): all
Makefile : ;
% :: $(OBJDIR) ; :
clean :
	$(call RM,$(OBJDIR))

else

VPATH = .. 

GCC_BIN = 
PROJECT = ThankSignal_Braveridge
OBJECTS = main.o BLE_API/source/BLE.o BLE_API/source/BLEInstanceBase.o BLE_API/source/DiscoveredCharacteristic.o BLE_API/source/GapScanningParams.o BLE_API/source/services/DFUService.o BLE_API/source/services/UARTService.o BLE_API/source/services/URIBeaconConfigService.o 
SYS_OBJECTS = mbed/TARGET_RZ_A1H/TOOLCHAIN_GCC_ARM/RZ_A1_Init.o mbed/TARGET_RZ_A1H/TOOLCHAIN_GCC_ARM/analogin_api.o mbed/TARGET_RZ_A1H/TOOLCHAIN_GCC_ARM/cache.o mbed/TARGET_RZ_A1H/TOOLCHAIN_GCC_ARM/can_api.o mbed/TARGET_RZ_A1H/TOOLCHAIN_GCC_ARM/cmsis_nvic.o mbed/TARGET_RZ_A1H/TOOLCHAIN_GCC_ARM/ethernet_api.o mbed/TARGET_RZ_A1H/TOOLCHAIN_GCC_ARM/gic.o mbed/TARGET_RZ_A1H/TOOLCHAIN_GCC_ARM/gpio_api.o mbed/TARGET_RZ_A1H/TOOLCHAIN_GCC_ARM/gpio_irq_api.o mbed/TARGET_RZ_A1H/TOOLCHAIN_GCC_ARM/i2c_api.o mbed/TARGET_RZ_A1H/TOOLCHAIN_GCC_ARM/mbed_board.o mbed/TARGET_RZ_A1H/TOOLCHAIN_GCC_ARM/mbed_sf_boot.o mbed/TARGET_RZ_A1H/TOOLCHAIN_GCC_ARM/mmu_Renesas_RZ_A1.o mbed/TARGET_RZ_A1H/TOOLCHAIN_GCC_ARM/nvic_wrapper.o mbed/TARGET_RZ_A1H/TOOLCHAIN_GCC_ARM/pinmap.o mbed/TARGET_RZ_A1H/TOOLCHAIN_GCC_ARM/pl310.o mbed/TARGET_RZ_A1H/TOOLCHAIN_GCC_ARM/port_api.o mbed/TARGET_RZ_A1H/TOOLCHAIN_GCC_ARM/pwmout_api.o mbed/TARGET_RZ_A1H/TOOLCHAIN_GCC_ARM/retarget.o mbed/TARGET_RZ_A1H/TOOLCHAIN_GCC_ARM/rtc_api.o mbed/TARGET_RZ_A1H/TOOLCHAIN_GCC_ARM/rza_io_regrw.o mbed/TARGET_RZ_A1H/TOOLCHAIN_GCC_ARM/serial_api.o mbed/TARGET_RZ_A1H/TOOLCHAIN_GCC_ARM/spi_api.o mbed/TARGET_RZ_A1H/TOOLCHAIN_GCC_ARM/startup_RZ1AH.o mbed/TARGET_RZ_A1H/TOOLCHAIN_GCC_ARM/system_MBRZA1H.o mbed/TARGET_RZ_A1H/TOOLCHAIN_GCC_ARM/us_ticker.o 
INCLUDE_PATHS = -I../. -I../shields -I../BLE_API -I../BLE_API/ble -I../BLE_API/ble/services -I../BLE_API/source -I../BLE_API/source/services -I../nRF51822 -I../mbed/. -I../mbed/TARGET_RZ_A1H -I../mbed/TARGET_RZ_A1H/TARGET_RENESAS -I../mbed/TARGET_RZ_A1H/TARGET_RENESAS/TARGET_RZ_A1H -I../mbed/TARGET_RZ_A1H/TARGET_RENESAS/TARGET_RZ_A1H/device -I../mbed/TARGET_RZ_A1H/TARGET_RENESAS/TARGET_RZ_A1H/device/inc -I../mbed/TARGET_RZ_A1H/TARGET_RENESAS/TARGET_RZ_A1H/device/inc/iobitmasks -I../mbed/TARGET_RZ_A1H/TARGET_RENESAS/TARGET_RZ_A1H/device/inc/iodefines -I../mbed/TARGET_RZ_A1H/TOOLCHAIN_GCC_ARM -I../mbed/drivers -I../mbed/hal -I../mbed/platform 
LIBRARY_PATHS = -L../mbed/TARGET_RZ_A1H/TOOLCHAIN_GCC_ARM 
LIBRARIES = -lmbed 
LINKER_SCRIPT = ../mbed/TARGET_RZ_A1H/TOOLCHAIN_GCC_ARM/RZA1H.ld

############################################################################### 
AS      = $(GCC_BIN)arm-none-eabi-as
CC      = $(GCC_BIN)arm-none-eabi-gcc
CPP     = $(GCC_BIN)arm-none-eabi-g++
LD      = $(GCC_BIN)arm-none-eabi-gcc
OBJCOPY = $(GCC_BIN)arm-none-eabi-objcopy
OBJDUMP = $(GCC_BIN)arm-none-eabi-objdump
SIZE    = $(GCC_BIN)arm-none-eabi-size 


CPU = -mcpu=cortex-a9 -mthumb -mthumb-interwork -marm -march=armv7-a -mfpu=vfpv3 -mfloat-abi=hard -mno-unaligned-access 
CC_FLAGS = $(CPU) -c -g -fno-common -fmessage-length=0 -Wall -Wextra -Wno-unused-parameter -Wno-missing-field-initializers
CC_FLAGS += -fno-exceptions -fno-builtin -ffunction-sections -fdata-sections -fno-delete-null-pointer-checks -fomit-frame-pointer
CC_FLAGS += -MMD -MP

CPPC_FLAGS = -c -Wall -Wextra -Wno-unused-parameter -Wno-missing-field-initializers -fmessage-length=0 -fno-exceptions -fno-builtin -ffunction-sections -fdata-sections -funsigned-char -MMD -fno-delete-null-pointer-checks -fomit-frame-pointer -mcpu=cortex-a9 -mthumb -mthumb-interwork -marm -march=armv7-a -mfpu=vfpv3 -mfloat-abi=hard -mno-unaligned-access -Os -std=gnu++98 -fno-rtti -Wvla -DTARGET_MBRZA1H -DDEVICE_ERROR_PATTERN=1 -DDEVICE_SPI=1 -D__FPU_PRESENT -D__MBED__=1 -DDEVICE_I2CSLAVE=1 -DTARGET_LIKE_MBED -DDEVICE_PORTINOUT=1 -DDEVICE_PORTIN=1 -DDEVICE_RTC=1 -DTOOLCHAIN_object -D__CMSIS_RTOS -D__EVAL -DTOOLCHAIN_GCC -DTARGET_CORTEX_A -DDEVICE_I2C_ASYNCH=1 -DARM_MATH_CA9 -DTARGET_UVISOR_UNSUPPORTED -DDEVICE_ANALOGIN=1 -D__MBED_CMSIS_RTOS_CA9 -DTARGET_LIKE_CORTEX_A9 -DDEVICE_SERIAL=1 -DDEVICE_INTERRUPTIN=1 -DDEVICE_I2C=1 -DDEVICE_PORTOUT=1 -DDEVICE_STDIO_MESSAGES=1 -DFEATURE_IPV4=1 -DDEVICE_SPI_ASYNCH=1 -DTARGET_RENESAS -DTARGET_RELEASE -DDEVICE_SERIAL_FC=1 -DTARGET_A9 -D__CORTEX_A9 -DTARGET_RZ_A1H -DDEVICE_SERIAL_ASYNCH=1 -DTARGET_FF_ARDUINO -DTOOLCHAIN_GCC_ARM -DDEVICE_CAN=1 -DDEVICE_ETHERNET=1 -DDEVICE_SPISLAVE=1 -DMBED_BUILD_TIMESTAMP=1479315285.14 -DDEVICE_PWMOUT=1 -include mbed_config.h -MMD -MP
ASM_FLAGS = -x assembler-with-cpp -D__FPU_PRESENT -DARM_MATH_CA9 -D__MBED_CMSIS_RTOS_CA9 -D__CMSIS_RTOS -D__CORTEX_A9 -D__EVAL -c -Wall -Wextra -Wno-unused-parameter -Wno-missing-field-initializers -fmessage-length=0 -fno-exceptions -fno-builtin -ffunction-sections -fdata-sections -funsigned-char -MMD -fno-delete-null-pointer-checks -fomit-frame-pointer -mcpu=cortex-a9 -mthumb -mthumb-interwork -marm -march=armv7-a -mfpu=vfpv3 -mfloat-abi=hard -mno-unaligned-access -Os
CC_SYMBOLS = -DTARGET_MBRZA1H -DDEVICE_ERROR_PATTERN=1 -DDEVICE_SPI=1 -D__FPU_PRESENT -D__MBED__=1 -DDEVICE_I2CSLAVE=1 -DTARGET_LIKE_MBED -DDEVICE_PORTINOUT=1 -DDEVICE_PORTIN=1 -DDEVICE_RTC=1 -DTOOLCHAIN_object -D__CMSIS_RTOS -D__EVAL -DTOOLCHAIN_GCC -DTARGET_CORTEX_A -DDEVICE_I2C_ASYNCH=1 -DARM_MATH_CA9 -DTARGET_UVISOR_UNSUPPORTED -DDEVICE_ANALOGIN=1 -D__MBED_CMSIS_RTOS_CA9 -DTARGET_LIKE_CORTEX_A9 -DDEVICE_SERIAL=1 -DDEVICE_INTERRUPTIN=1 -DDEVICE_I2C=1 -DDEVICE_PORTOUT=1 -DDEVICE_STDIO_MESSAGES=1 -DFEATURE_IPV4=1 -DDEVICE_SPI_ASYNCH=1 -DTARGET_RENESAS -DTARGET_RELEASE -DDEVICE_SERIAL_FC=1 -DTARGET_A9 -D__CORTEX_A9 -DTARGET_RZ_A1H -DDEVICE_SERIAL_ASYNCH=1 -DTARGET_FF_ARDUINO -DTOOLCHAIN_GCC_ARM -DDEVICE_CAN=1 -DDEVICE_ETHERNET=1 -DDEVICE_SPISLAVE=1 -DMBED_BUILD_TIMESTAMP=1479315285.14 -DDEVICE_PWMOUT=1 

LD_FLAGS =-Wl,--gc-sections -Wl,--wrap,main -Wl,--wrap,_malloc_r -Wl,--wrap,_free_r -Wl,--wrap,_realloc_r -Wl,--wrap,_calloc_r -mcpu=cortex-a9 -mthumb -mthumb-interwork -marm -march=armv7-a -mfpu=vfpv3 -mfloat-abi=hard -mno-unaligned-access 
LD_SYS_LIBS = -lstdc++ -lsupc++ -lm -lc -lgcc -lnosys


ifeq ($(DEBUG), 1)
  CC_FLAGS += -DDEBUG -O0
else
  CC_FLAGS += -DNDEBUG -Os
endif


.PHONY: all lst size

all: $(PROJECT).bin $(PROJECT).hex size



.asm.o:
	+@$(call MAKEDIR,$(dir $@))
	$(CC) $(CPU) -c $(ASM_FLAGS) $(CC_SYMBOLS) $(INCLUDE_PATHS) -o $@ $<
.s.o:
	+@$(call MAKEDIR,$(dir $@))
	$(CC) $(CPU) -c $(ASM_FLAGS) $(CC_SYMBOLS) $(INCLUDE_PATHS) -o $@ $<
.S.o:
	+@$(call MAKEDIR,$(dir $@))
	$(CC) $(CPU) -c $(ASM_FLAGS) $(CC_SYMBOLS) $(INCLUDE_PATHS) -o $@ $<

.c.o:
	+@$(call MAKEDIR,$(dir $@))
	$(CC)  $(CC_FLAGS) $(CC_SYMBOLS) $(INCLUDE_PATHS) -o $@ $<

.cpp.o:
	+@$(call MAKEDIR,$(dir $@))
	$(CPP) $(CPPC_FLAGS) $(CC_SYMBOLS) $(INCLUDE_PATHS) -o $@ $<




$(PROJECT).elf: $(OBJECTS) $(SYS_OBJECTS) $(LINKER_SCRIPT)
	$(LD) $(LD_FLAGS) -T$(filter %.ld, $^) $(LIBRARY_PATHS) -o $@ $(filter %.o, $^) -Wl,--start-group $(LIBRARIES) $(LD_SYS_LIBS) -Wl,--end-group

	@echo ""
	@echo "*****"
	@echo "***** You must modify vector checksum value in *.bin and *.hex files."
	@echo "*****"
	@echo ""


$(PROJECT).bin: $(PROJECT).elf
	$(OBJCOPY) -O binary $< $@

$(PROJECT).hex: $(PROJECT).elf
	@$(OBJCOPY) -O ihex $< $@

$(PROJECT).lst: $(PROJECT).elf
	@$(OBJDUMP) -Sdh $< > $@

lst: $(PROJECT).lst

size: $(PROJECT).elf
	$(SIZE) $(PROJECT).elf

DEPS = $(OBJECTS:.o=.d) $(SYS_OBJECTS:.o=.d)
-include $(DEPS)


endif
