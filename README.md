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
### Please Note :- Do not Power On your raspberry Pi before you have plugged in all your I/O Devices.
wait for the [RASPBIAN OS](https://www.raspberrypi.org/downloads/raspbian/) to boot up and initallize itself and you'll be greated with a home Screen that looks like this.
![rpi-home-screen](https://user-images.githubusercontent.com/43185907/49835201-753c9500-fd6c-11e8-8d28-7d7a5e1cb914.png)

Which i got from this [website](http://albumplays.com/raspberry-pi/assisted-installation-raspberry-pi/rpi-home-screen/)




# PCB and Soldering. 

Once you have all the parts ready to use, this is how you should 

![pcbbarometricsensor_bb](https://user-images.githubusercontent.com/43185907/49048095-89e32f80-f1a7-11e8-8fa2-22bcb1d66fbc.png)

And When you design your PCB, Please Make sure that the Grey Part(Actual PCB) has all the wiring inside it.

![pcbbarometricsensor_pcbnew](https://user-images.githubusercontent.com/43185907/48722214-7e18cb80-ebf1-11e8-8b25-dfd06f559e3d.png)

You'll need a [12 Pin Header](https://canada.newark.com/adafruit/2223/40-pin-pi-gpio-stacking-header/dp/31AC4582?gclid=Cj0KCQiA3b3gBRDAARIsAL6D-N9cOFlmcrDGau38Dyun99IYzh_ug67qgDeVlbwTAWUUSCZh_Ob89TsaAukoEALw_wcB&CAGPSPN=pla&CAWELAID=120185770002227709&CAAGID=23354969332&CMP=KNC-GCA-GEN-SHOPPING&CATCI=pla-294680686006) to connect your Sensor to your Raspberry Pi.

Once THE PCB is Designed,lets try [Creating the Case](https://github.com/GursehajHarika/barometricsensor/blob/master/PiGursehajHarika.cdr) for it 

Once the case is completed.
bring your [PCB], Sensor and [Raspberry Pi] fitted inside the case.
and this is how youre final sensor complete with your case and PCB should look like.
![sensorcase2](https://user-images.githubusercontent.com/43185907/48949692-e116a500-ef06-11e8-8675-9b4f8dc0291f.jpeg)

![sensorcase](https://user-images.githubusercontent.com/43185907/48949567-60f03f80-ef06-11e8-90fd-74825a6f81f5.jpeg)

which should be edited on Corel draw as the file that i have was made on Corel Draw.

Once youre case is complete and raspberry pi is connecting to a display we have to work on making the Raspberry Pi Remotly acessable,
Go to youtube and follow this [tutorial](https://www.youtube.com/watch?v=WAFaw2Mbnko)
after you're done with the tutorial your Raspberry Pi should work with remote desktop and now you don't need a keyboard and a mouse or even a monitor just to run your Raspberry Pi.

Now open Terminal and Type in 
i2c detect -y 1 and you shuould see 0x76.
if not please look at your PCB.
 
Now Create a [Python Code](https://github.com/GursehajHarika/barometricsensor/blob/master/ms5611.py) and that code will run and you'll be able to get some readings from it which should look somtihng like this.

![sensorreadings](https://user-images.githubusercontent.com/43185907/48626353-a5686200-e97f-11e8-95df-3de6a83a0182.jpeg)

and in order to run it,

type in " sudo python YOUR_FILE_NAME.py "

and you should be good to go.

### Bonus

if you wish to add another sensor, i would recommend looking at [Arman Velani's 3-axis accelormeter](https://github.com/ArmanVelani/3-AxisAccelerometer) and go through his read me and if you are able to make his sensor too and try to put it on your sensor, it will look somthing like this.

![barometricpressureand3axissensorstacked](https://user-images.githubusercontent.com/43185907/48626118-07749780-e97f-11e8-9f47-7c04b9b4464c.jpeg)


# Unit and Production Testing

If i were to make a 1000 or 10,000 of these sensors and have more than one 
i would try to fit both 
