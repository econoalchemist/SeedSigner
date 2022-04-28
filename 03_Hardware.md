# Hardware
This section demonstrates how to assemble the SeedSigner kit components into the final product and also provides details on what each component is and alternative places to purchase these components in case you do not want to purchase the whole kit from one vendor. Best practice is to test that your components power on and the SeedSigner software works prior to assembly. The enclosure and or components can be damaged if you attempt disassembly. 

## Enclosure
The enclosure included in the kit is an open-face design, alternative designs are available from vendors linked below. The enclosure is 3D printed, you can even [download the file](https://github.com/SeedSigner/seedsigner/tree/main/enclosures/open_pill) and print one yourself. 

The enclosure outter dimensions are 80mm x 35mm x 26mm and there are a number of retention bumps, support ledges, and journals to fit the components snugly inside.  
![](assets/hardware00.jpg)

The enclosure also features openings for the camera lense, microUSB ports, HDMI port, and MicroSD card port.
![](assets/hardware01.jpg)

If you do not want to get the complete kit, you can buy a stand alone enclosure of various designs from the following vendors:

- Worlwide delivery available from [BTC Hardware Solutions](https://btc-hardware-solutions.square.site/product/orange_pill/5?cs=true&cst=custom)
- Worldwide delivery available from [Robotechy](https://robotechy.com/collections/frontpage/products/seedsigner-3d-printed-pill-case)
- EU/UK delivery available from [GoBrrr](https://www.gobrrr.me/product/seedsigner-lilpill-case/?v=7516fd43adaa), [DIYNodes](https://diynodes.com/product/seedsigner-3d-printed-orange-pill-case/), & [AnchorHodl](https://anchorhodl.com/product/retro-pill-case-for-seedsigner)

## Raspberry Pi Camera & Cable
The camera is a 5MP OV5647 Sensor, 30 FPS, 2592x1944 resolution video camera module designed for a range of RaspberryPis. The working voltage is 1.7vdc ~ 3vdc. This module measures 25mm x 24mm x 9mm. The camera ships with a protective film over the lense, be sure to remove this prior to assembly.
![](assets/hardware03.jpg)

![](assets/hardware04.jpg)

You want the `HBV-Raspberry-160FPC` golden ribbon cable for the RaspberryPi Zero. This cable has 16-flat-pin connector side measuring 16mm, a 22-flat-pin connector side measuring 11mm, and the overall length is 160mm.
![](assets/hardware05.jpg)

If you do not want to get the complete kit, you can buy a stand alone camera & cable from the following vendors:

- EU/UK delivery available from [GoBrrr](https://www.gobrrr.me/product/ov5647-pi-cam/?v=7516fd43adaa)
- North America delivery available from [Amazon](https://www.amazon.com/dp/B07RXKZ1KN?th=1)
- Philippines delivery available from [TechHaven](https://www.lazada.com.ph/products/raspberry-pi-camera-i2659578273-s12654014174.html?spm=a2o4l.seller.list.4.111a346bP5V0no&mp=1&freeshipping=1)

## RaspberryPi Zero v1.3
The RaspberryPi Zero is the smallest single board computer RaspberryPi manufactures. The v1.3 computer features a 1Ghz single-core CPU, 512MB of RAM, mini-HDMI port, one microUSB port for power only, one microUSB port for data transfer, a HAT-compatible 40-pin header, composit video & reset headers, a microSD card slot, and a CSI camera connector. The full hardware specification can be found [here](https://www.raspberrypi.com/documentation/computers/raspberry-pi.html). 

![](assets/hardware07.jpg)

The RaspberryPi Zero measures 66mm x 31mm x 11mm. 
![](assets/hardware08.jpg)

If you do not want to get the complete kit, you can buy a stand alone RaspberryPi Zero from the following vendors:

- EU/UK delivery available from [GoBrrr](https://www.gobrrr.me/product/pizero-wh/?v=7516fd43adaa)
- EU delivery available from [BricoGeek](https://tienda.bricogeek.com/placas-raspberry-pi/1358-raspberry-pi-zero-v1-3.html) or [Reichelt](https://www.reichelt.com/ch/en/raspberry-pi-zero-v-1-3-1-ghz-512-mb-ram-rasp-pi-zero-p256439.html)
- North American delivery available from [Adafruit](https://www.adafruit.com/product/2885)
- Philippines delivery available from [TechHaven](https://www.lazada.com.ph/products/raspberry-pi-zero-version-13-i2659573158-s12653906040.html?spm=a2o4l.seller.list.1.111a346bP5V0no&mp=1&freeshipping=1)

## WaveShare LCD HAT Display
The WaveShare LCD Hardware-Attached-on-Top (HAT) is a 65mm x 30mm module that attached to the 40-pin connector on the RaspberryPi Zero. This module features a 240x240 resolution, RGB display measuring 39mm diagonal. The embedded controls use a joystick and three pushbuttons. Operating voltage is 3.3vdc. More specifications can be found [here](https://www.waveshare.com/wiki/1.3inch_LCD_HAT).

![](assets/hardware09.jpg)

![](assets/hardware10.jpg)

If you do not want to get the complete kit, you can buy a stand alone WaveShare LCD HAT Display from the following vendors:

- EU/UK delivery available from [GoBrrr](https://www.gobrrr.me/product/waveshare-lcd-display/?v=7516fd43adaa)
- EU delivery available from [Welectron](https://www.welectron.com/Waveshare-14972-13inch-LCD-HAT_1)
- North America delivery available from [WaveShare](https://www.waveshare.com/1.3inch-lcd-hat.htm)
- Worldwide delivery available from [AliExpress](https://www.aliexpress.com/item/32952472064.html)
- Philippines delivery available from [TechHaven](https://www.lazada.com.ph/products/waveshare-14972-13inch-lcd-hat-i2659455966-s12653987690.html?spm=a2o4l.seller.list.7.111a346bP5V0no&mp=1&freeshipping=1)

## Assembly
Prior to attempting assembly, ensure that you have tested that everything works by connecting the camera and display to the RaspberryPi Zero, inserting the MicroSD card with the SeedSigner image loaded, and powering on the device by connecting a microUSB cable to the power input port.  
