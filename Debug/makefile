################################################################################
# Automatically-generated file. Do not edit!
################################################################################

-include ../makefile.init

RM := rm -rf

# All of the sources participating in the build are defined here
-include sources.mk
-include example/src/subdir.mk
-include subdir.mk
-include objects.mk

ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
endif

-include ../makefile.defs

# Add inputs and outputs from these tool invocations to the build variables 

# All Target
all: usbd_lib_cdc_AZ_az.axf

# Tool invocations
usbd_lib_cdc_AZ_az.axf: $(OBJS) $(USER_OBJS)
	@echo 'Building target: $@'
	@echo 'Invoking: MCU Linker'
	arm-none-eabi-gcc -nostdlib -L"C:\Users\user\Documents\MCUXpressoIDE_10.0.2_411\workspace\lpc_chip_40xx\Debug" -L"C:\Users\user\Documents\MCUXpressoIDE_10.0.2_411\workspace\lpc_board_ea_devkit_4088\Debug" -L"C:\Users\user\Documents\MCUXpressoIDE_10.0.2_411\workspace\lpc_chip_40xx\libs" -Xlinker -Map="usbd_lib_cdc_AZ_az.map" -Xlinker --gc-sections -mcpu=cortex-m4 -mfpu=fpv4-sp-d16 -mfloat-abi=softfp -mthumb -T "usbd_lib_cdc_Debug.ld" -o "usbd_lib_cdc_AZ_az.axf" $(OBJS) $(USER_OBJS) $(LIBS)
	@echo 'Finished building target: $@'
	@echo ' '
	$(MAKE) --no-print-directory post-build

# Other Targets
clean:
	-$(RM) $(EXECUTABLES)$(OBJS)$(C_DEPS) usbd_lib_cdc_AZ_az.axf
	-@echo ' '

post-build:
	-@echo 'Performing post-build steps'
	-arm-none-eabi-size "usbd_lib_cdc_AZ_az.axf"; # arm-none-eabi-objcopy -v -O binary "usbd_lib_cdc_AZ_az.axf" "usbd_lib_cdc_AZ_az.bin" ; # checksum -p LPC4088 -d "usbd_lib_cdc_AZ_az.bin";
	-@echo ' '

.PHONY: all clean dependents
.SECONDARY: post-build

-include ../makefile.targets
