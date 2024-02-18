MCU stm32f411re
Board Nucleo
libopencm3
blink example


Easy "clone and go" repository for a libopencm3 based project.

 1. git clone --recurse-submodules https://github.com/Yra179/libopencm3-stm32f411re-blink.git
 2. cd libopencm3-stm32f411re-blink
 3. make -C libopencm3 # (Only needed once)
 4. make -C blink
 5. make stlink-flash # (connect board and flash)
