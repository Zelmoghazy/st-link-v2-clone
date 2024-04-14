```
openocd -f interface/stlink-v2.cfg -f .\myconfig.cfg -c "init" -c "halt" -c "stm32f1x unlock 0" -c "shutdown"
```

```
st-flash erase
```

```
openocd -f interface/stlink-v2.cfg -f .\myconfig.cfg -c "init" -c "halt" -c "flash write_image erase Unprotected-2-1-Bootloader.bin 0x08000000" -c "shutdown"
```