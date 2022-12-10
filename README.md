# RGB-Matrix-LED-Mario-Bros.-Clock
Super Mario is my childhood memory, when I saw JnthasMario Bros. Clock project, I immediately decided to make one

![github](https://github.com/James-workshop/RGB-Matrix-LED-Mario-Bros.-Clock/blob/main/IMG/10.jpg "Mario-Bros.-Clock")

Here is a record of my production process.

# Hardware
* Custom PCB x 1
* LED panel (HUB75； RGB 64 X 64；P3）
* ESP32 Dev Board 
* Dupont wire Female To Female(for prototype or test circuit)
* 2.54mm Double Row Female Header 2x8pin
* 2.54mm Single Row Female Header 15pin X2
* 2.54mm Single Row Straight Male Header 3pin
* Jumper Cap
* 220K Ohm resistance
* 10K Ohm resistance
* 220uF 25V Capacitor
* 1N5822
* KF8500 PCB screw block
* KF301 PCB screw block
* DC Jack Adapter
* Power Supply 5v 3A or more


![github](https://github.com/James-workshop/RGB-Matrix-LED-Mario-Bros.-Clock/blob/main/Schematic_LED%20Matrix_2022-12-08.png "Schematic")
<BR><BR><BR><BR>
# PCB
I made a PCB at JLCPCB.com, which makes it very easy to make!

![github](https://github.com/James-workshop/RGB-Matrix-LED-Mario-Bros.-Clock/blob/main/IMG/EasyEDA.png "EasyEDA")

![github](https://github.com/James-workshop/RGB-Matrix-LED-Mario-Bros.-Clock/blob/main/IMG/3D_F.png "3DPCB")

### ![github](https://jlcpcb.com/client/svg/nv_logo.svg "JLCPCB") Make hardware development easier, Higher Quality & Lower Cost
### New registered users offer , **[Order here ](https://jlcpcb.com/?from=James)**
### You can use my Gerber file to place an order at JLCPCB.com

![github](https://github.com/James-workshop/RGB-Matrix-LED-Mario-Bros.-Clock/blob/main/IMG/21.jpg "PCB")
<BR><BR><BR>
# PCB Assembly
  
![github](https://github.com/James-workshop/RGB-Matrix-LED-Mario-Bros.-Clock/blob/main/IMG/23.jpg "PCBA")
  
Just solder according to the schematic diagram, and then assemble the PCB on the LED paneland connect the power

<BR><BR><BR>
# Firmware
Thanks Brian & Jnthas for that, we can use the Clockwise.page to upload firmware without having to install anything and without making any effort as it is already compiled. Just plug the ESP32 into the USB port and click Flash to flash.

## Configuring WiFi
The first time you run it, you need to configure the WiFi, for that connect to the "Clockwise-Wifi" access point with the password 12345678 via your smartphone or laptop, click "Configure WiFi" and select your AP, put in your password and your timezone and save. Then the clock can connect to an NTP server to get the correct time. It is important to use a 2.4GHz WiFi, it will not work on 5G.

## About Timezone
WiFi Manager is responsible for collecting the timezone parameter used in the clock to show the time correctly. When instantiating the NTP client, the default time is in UTC, we need to inform the correct timezone during the Wifi setup process. All the available timezone names is listed here, e.g. America/New_York, Asia/Dubai, Europe/Paris, and so on.
In my case, I type "Asia/Hong_Kong" in the timezone field on WiFi Manager not work. In the end I need typed Asia/Macau to work  
  
## For a more detail, please watch my video
<a href="https://youtu.be/MCjrmfSF1EU">https://youtu.be/MCjrmfSF1EU</a>
  ![github](https://github.com/James-workshop/RGB-Matrix-LED-Mario-Bros.-Clock/blob/main/IMG/Mario%20brother%20Clock%20I.jpg "Youtube Cover Photo")
<BR><BR>
<a href="https://youtu.be/UVlxxYB1LpE">https://youtu.be/UVlxxYB1LpE</a>
  ![github](https://github.com/James-workshop/RGB-Matrix-LED-Mario-Bros.-Clock/blob/main/IMG/Mario%20Brother%20Clock%20II.jpg "Youtube Cover Photo")
    
    
