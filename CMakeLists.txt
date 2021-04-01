cmake_minimum_required(VERSION 3.15)

project(L431_LED LANGUAGES C CXX ASM)

find_bsp(ID com.sysprogs.project_importers.stm32.cubemx
	SOURCE_PROJECT L431_LED.ioc)

add_bsp_based_executable(NAME L431_LED
	GENERATE_BIN
	GENERATE_MAP)
