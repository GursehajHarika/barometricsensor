# barometricsensor


MS5611 Barometric Pressure (0x76)![barometric pressure senor](https://user-images.githubusercontent.com/43185907/49833042-5935f500-fd66-11e8-84f8-3ecc64b90181.jpg)

picture from [this](https://www.ebay.ca/i/192749049300?chn=ps&dispItem=1) Webpage.



# Introduction 

Have you ever wanted to know what was your height or how high somtihng goes without calulating its speed and figuring out its distance traveled. My senor (Barometric Pressure Senor is what you're looking for. 
This Sensor Is able to read the height of the object or the temperature around it.
here's how this sensor works with a android application. If you wish to work on the appication as well. i would highly recommend you clicking on [this](https://github.com/GursehajHarika/SAG-Droning). 
here's the System diagram on how it will work,
![umlimage](https://user-images.githubusercontent.com/43185907/48031330-cdef9100-e121-11e8-9fc3-03276bc2c449.PNG)


# Parts and Tools 

These are the parts and Tools required to make,

### Please Note :- Some of the parts will take up to a month to be delivered to your door step.

a soldering tool,
![image](https://user-images.githubusercontent.com/43185907/49832105-bda38500-fd63-11e8-91b4-6f54d5e169e2.jpeg)



lead free soldering wire(Recommended) or a soldering wire.

Raspberry Pi 3  - $141.47 [Image1 ](https://raw.githubusercontent.com/GursehajHarika/barometricsensor/master/Project%20receipts/raspberry.png.jpg)
       

Ethernet to USB adapter- $31.53 [Image of the receipt](https://raw.githubusercontent.com/GursehajHarika/barometricsensor/master/Project%20receipts/Adapter.png)   

Barometric Pressure Sensor - $11.99 [Image of sensor ](https://raw.githubusercontent.com/GursehajHarika/barometricsensor/master/Project%20receipts/reciept%20sensor.png)  

And a Parts Kit that i bought from humber but you can get ir from where ever you feel like, as long as it has the same tools.
[image](https://raw.githubusercontent.com/GursehajHarika/barometricsensor/master/Project%20receipts/20181002_175841.jpg)

# Mechanical Assembly

Once you get your [Raspberry Pi 3.](https://www.canakit.com/raspberry-pi-3-model-b-plus.html) and keep your micro-SD card handy, you'll be needing it soon.
Go to Raspberry Pi 's Website and download [Raspbian full desktop verison](https://www.raspberrypi.org/downloads/) and get a [software to format the SD card to NFTS format.](https://www.sdcard.org/downloads/formatter_4/)
Flash your Raspbian OS to your SD Card.
Connect your Raspberry Pi to a Monitor. Grab a Keyboard,a mouse and a HTMI or VGA(Depending on what type of monitor you have.
wait for the [RASPBIAN OS](https://www.raspberrypi.org/downloads/raspbian/) to boot up.



# PCB and Soldering. 

Once you have all the parts ready to use, this is how you should 

![pcbbarometricsensor_bb](https://user-images.githubusercontent.com/43185907/49048095-89e32f80-f1a7-11e8-8fa2-22bcb1d66fbc.png)

And When you design your PCB, Please Make sure that the Grey Part(Actual PCB) has all the wiring inside it.

![pcbbarometricsensor_pcbnew](https://user-images.githubusercontent.com/43185907/48722214-7e18cb80-ebf1-11e8-8b25-dfd06f559e3d.png)

You'll need a [12 Pin Header](https://canada.newark.com/adafruit/2223/40-pin-pi-gpio-stacking-header/dp/31AC4582?gclid=Cj0KCQiA3b3gBRDAARIsAL6D-N9cOFlmcrDGau38Dyun99IYzh_ug67qgDeVlbwTAWUUSCZh_Ob89TsaAukoEALw_wcB&CAGPSPN=pla&CAWELAID=120185770002227709&CAAGID=23354969332&CMP=KNC-GCA-GEN-SHOPPING&CATCI=pla-294680686006) to connect your Sensor to your Raspberry Pi.

