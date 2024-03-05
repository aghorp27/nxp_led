################################################################################
# Automatically-generated file. Do not edit!
################################################################################

-include ../makefile.init

RM := rm -rf

# All of the sources participating in the build are defined here
-include sources.mk
-include src/subdir.mk
-include generate/src/subdir.mk
-include board/subdir.mk
-include RTD/src/subdir.mk
-include Project_Settings/Startup_Code/subdir.mk
-include subdir.mk
-include objects.mk

ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
endif

-include ../makefile.defs

# Add inputs and outputs from these tool invocations to the build variables 
SECONDARY_FLASH += \
led_M7_0.hex \

SECONDARY_SIZE += \
led_M7_0.siz \


# All Target
all: led_M7_0.elf secondary-outputs

dependents:
	-cd C:/Users/eya12/workspaceS32DS.3.5/led/led_M7_1/Debug_FLASH && $(MAKE) clean all

# Tool invocations
led_M7_0.elf: $(OBJS) C:/Users/eya12/workspaceS32DS.3.5/led/led_M7_0/Project_Settings/Linker_Files/linker_flash_c0_s32k322.ld $(USER_OBJS) C:/Users/eya12/workspaceS32DS.3.5/led/led_M7_1/Debug_FLASH/led_M7_1.elf
	@echo 'Building target: $@'
	@echo 'Invoking: Standard S32DS C Linker'
	arm-none-eabi-gcc -o "led_M7_0.elf" "@led_M7_0.args"  $(USER_OBJS)
	@echo 'Finished building target: $@'
	@echo ' '

led_M7_0.hex: led_M7_0.elf
	@echo 'Invoking: Standard S32DS Create Flash Image'
	arm-none-eabi-objcopy -O ihex led_M7_0.elf  "led_M7_0.hex"
	@echo 'Finished building: $@'
	@echo ' '

led_M7_0.siz: led_M7_0.elf
	@echo 'Invoking: Standard S32DS Print Size'
	arm-none-eabi-size --format=berkeley led_M7_0.elf
	@echo 'Finished building: $@'
	@echo ' '

# Other Targets
clean:
	-$(RM) ./*
	-@echo ' '

secondary-outputs: $(SECONDARY_FLASH) $(SECONDARY_SIZE)

.PHONY: all clean dependents
C:/Users/eya12/workspaceS32DS.3.5/led/led_M7_1/Debug_FLASH/led_M7_1.elf:

-include ../makefile.targets
