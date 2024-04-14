

<p align="center">
  <img src="./Images/A611cf33089f74830b00823becb2412c8A.webp"
       width="45%" 
       style="border-radius: 30px;"/>
</p>

* STM32 Clone
<p align="center">
  <img src="./Images/chrome_SuSKcdilPA.png"
       width="100%" 
       style="border-radius: 30px;"/>
</p>

<p align="center">
  <img src="./Images/SumatraPDF_4lavNja64r.png"
       width="100%" 
       style="border-radius: 30px;"/>
</p>




<p align="center">
  <img src="./Images/ST LINK Stlink ST-Link V2 Mini STM8 STM32 JTAG.jpg"
       width="100%" 
       style="border-radius: 30px;"/>
</p>

```
openocd -f interface/stlink-v2.cfg -f .\myconfig.cfg -c "init" -c "halt" -c "stm32f1x unlock 0" -c "shutdown"
```

```
st-flash erase
```

```
openocd -f interface/stlink-v2.cfg -f .\myconfig.cfg -c "init" -c "halt" -c "flash write_image erase Unprotected-2-1-Bootloader.bin 0x08000000" -c "shutdown"
```