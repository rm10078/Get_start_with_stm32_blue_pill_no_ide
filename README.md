
# Get start with stm32

Follow all command step to step



## Deployment

#### Step:-1
install st-link and compiler for stm32

```bash
  sudo apt install stlink-tools gcc-arm-none-eabi
```

#### Step:-2
Clone the libopencm3 all library are inside this repo

```bash
  git clone https://github.com/libopencm3/libopencm3-template
```
```bash
  cd libopencm3-template
```
```bash
  git submodule init
```
```bash
  git submodule update
```
```bash
  make
```
#### Step:-3
Make a folder for your project.  <br> inside the folder make two file one is Makefile and other is main.c file.
</br> project link:- https://github.com/rm10078/Get_start_with_stm32_blue_pill_no_ide/tree/main/stm_blink_first

#### Step:-4
After typeing code run make command on your project dir location

```bash
  make
```

#### Step:-5
Check your st-link v2 programmer detected or not
ST-LINK v2
![App Screenshot](https://github.com/rm10078/Get_start_with_stm32_blue_pill_no_ide/blob/main/img/st-link.jpg?raw=true)

```bash
  st-info
```
For check the programmer version
```bash
  st-info --version
```

#### Step:-5
Befor flash the program you need to change the boot jumper. BOOT0 GND TO 3.3
#### PinOut
![App Screenshot](https://github.com/rm10078/Get_start_with_stm32_blue_pill_no_ide/blob/main/img/STM32F103C8T6-Blue-Pill-Pin-Layout.gif?raw=true)

#### Step:-6
If your code have not any error, you can find a .bin file.
</br> For upload code type this command

```bash
  st-flash --reset write <file name.bin> 0x8000000
```

#### Step:-7
After upload the code change the boot jumper <br> to the normal position and press reset button one time.

<br> Now your code is running normaly.
<br> ⚠ do not press reset button without changeing the boot jumper.
<br> If you pree then your inter program are erase. 

### For programming 
follow the Beginning STM32 Book by Warren Gay

# Thank your

