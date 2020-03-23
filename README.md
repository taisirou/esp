# esp-32 AT Command Pin Configuration
ATコマンド用のピンを間違えた人用

RX:IO16
TX:IO17

https://github.com/espressif/esp-at

--flash_mode dio --flash_freq 40m --flash_size detect 
0x1000 bootloader/bootloader.bin 
0x20000 at_customize.bin 
0x30000 customized_partitions/factory_param.bin 
0xf000 phy_init_data.bin 
0x100000 esp-at.bin 
0x8000 partitions_at.bin
