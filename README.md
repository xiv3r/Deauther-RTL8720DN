# Deauther RTL8720DN
2G/5Ghz Deauther firmware for RTL8720DN BW16 MCU


<img src="https://github.com/xiv3r/RT8720DN-Deauther/blob/main/rtl7820dn.png">

# Installation (windows)
- First [Download](https://github.com/xiv3r/Deauther-RTL8720DN/raw/refs/heads/main/CH341SER.EXE) and Install the CH340G driver for RTL8720DN

- [Download](https://github.com/xiv3r/Deauther-RTL8720DN/releases/download/RTL8720DN/RTL8720DN-Deauther.zip) and unzip the Firmware and Flasher

- Open the flasher and import the firmware then flash

- Connect to the WiFi=`Ereshkigal` Password=`masukangin`

- Open the browser [http://192.168.1.1](http://192.168.1.1)

- Then you can start the attack

# Linux
```
sudo apt update && sudo apt install esptool -y
```
```
git clone https://github.com/xiv3r/Deauther-RTL8720DN
cd Deauther-RTL8720DN
```
- Install the ch340g driver
```
cd Linux_Driv3r
```
```
make
```
```
sudo make load
```
```
sudo make install
```
- Flash the firmware
```
cd Deauther-RTL8720DN
```
```
esptool -b 115200 0x0 RTL8720DN.bin
```
- Connect to the WiFi=`Ereshkigal` Password=`masukangin`

- Open the browser [http://192.168.1.1](http://192.168.1.1)

- Then you can start the attack


Credit: [Ereshkigal](https://github.com/Arifmaulanaazis/Ereshkigal)
