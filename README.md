# Frozen Slimes V2

### Contact: artemis8615

## Check out the [Discord](https://discord.gg/vhHEsKjWGV)

This project will currently be using a Wemo D1 mini, mpu6050, bmi160 or bno085s, and a TP4056 charger. On my personal slimes I wanted to use a 18650 batteries due to the longer battery life and how easy they are to get. 

This is the second version of the case with a hotswappable 18650, strap slots build into the pcb and a much improved pcb design. 

This will now also support mpu6050s, bmis160s, and BNO085s all on one pcb with toggles. 

Tested:
- mpu6050 = yes
- bmi160 = yes
- BNO085s = yes

Tested Extensions:
- mpu6050 = yes
- bmi160 = yes
- BNO085s = no



[Offical Component Guide](https://docs.slimevr.dev/diy/components-guide.html)


## Index
- [Components](#Components)
- [Case](#Case)
- [PCB](#PCB)
- [Printing](#Printing)
- [Assembly](#Assembly)
- [Flashing Firmware](#Flashing-firmware)
- [Links](#Links)
- [Community Builds](#Community-Builds)


### Components   
- [TP4056](https://www.amazon.com/HiLetgo-Lithium-Battery-Charging-Protect/dp/B00LTQU2RK/ref=sr_1_3?crid=31BCDZYQGA5IU&keywords=TP4056&qid=1643591253&sprefix=tp4056%2Caps%2C124&sr=8-3)
- [Wemos D1 Mini](https://www.amazon.com/Organizer-ESP8266-Internet-Development-Compatible/dp/B081PX9YFV/ref=sr_1_3?crid=2FMF3NVYGOSPK&keywords=wemos+d1+mini&qid=1643591309&sprefix=wemos+d1+mini%2Caps%2C136&sr=8-3)
- [2in straps](https://www.amazon.com/gp/product/B0C42S3HQC/ref=ox_sc_act_title_1?smid=A29WFRG6NP7W74&psc=1)
- [IMU docs](https://docs.slimevr.dev/diy/components-guide.html)
    - [MPU6050](https://www.amazon.com/MPU-6050-Accelerometer-Gyroscope-Converter-Compatible/dp/B08TH9NH55/ref=sr_1_6?crid=1W65V3QJ27XN&keywords=mpu+6050&qid=1643591376&sprefix=mpu+6050%2Caps%2C136&sr=8-6)  
    - [BMI160](https://www.amazon.com/UMLIFE-GY-BMI160-Accelerometer-Gyroscope-Acceleration/dp/B09BQTP8SN/ref=sr_1_4?keywords=bmi160&qid=1687315590&sr=8-4)
- [Switch](https://docs.slimevr.dev/diy/components-guide.htmll)
    - [SS22F32](https://www.aliexpress.com/item/32975535599.html)
- [Battery](https://docs.slimevr.dev/diy/components-guide.html)
    - [18650](https://www.amazon.com/s?k=18650&crid=2H65KICLJGU4U&sprefix=18650%2Caps%2C301&ref=nb_sb_noss_1)
- [1n5817 Diode](https://www.amazon.com/100-Pieces-1N5817-Schottky-Rectifier/dp/B079KDQQPD/ref=sr_1_5?crid=1EPLYISD4R4G3&keywords=1n5817+Diode&qid=1659032765&sprefix=1n5817+diode%2Caps%2C130&sr=8-5)
- [180k Resistor](https://www.amazon.com/EDGELEC-Resistor-Tolerance-Resistance-Optional/dp/B07HDFCNXB/ref=sr_1_3?crid=9MPFJ93KJT6X&keywords=180k+resistor&qid=1659032821&sprefix=180k+%2Caps%2C129&sr=8-3)
- [18650 Battery Solderable Holder](https://www.amazon.com/dp/B09N76T4GL?ref=nb_sb_ss_w_as-reorder-t1_k5_1_6&amp=&crid=9IYBEM7L1PYO&amp=&sprefix=18650+)






### PCB 

#### Check above for tested and supported mpus

This PCB lets every component be soldered on without any extra wires. This includes the diodes and resistor for battery sense and protected charging. 

To order PCBS go to a website like https://cart.jlcpcb.com/quote upload the gerber file zip file and select quanity and color and order. It should autoselect all the other correct options when you upload the gerber file. 


*if you want to buy pcb packs, fully assembled pcbs or even whole trackers dm me*



<img src="https://github.com/frosty6742/frozen-slimes-v2/blob/main/Pictures/20230212_062153031_iOS.png" alt="PCB" width="600" height="400" /> 

<img src="https://github.com/frosty6742/frozen-slimes-v2/blob/main/Pictures/20230212_062336631_iOS.png" alt="PCB" width="400" height="500" /> 

<img src="https://github.com/frosty6742/frozen-slimes-v2/blob/main/Pictures/20230212_065153234_iOS.png" alt="PCB" width="600" height="400" /> 


![Screenshot 2023-02-10 085738](https://user-images.githubusercontent.com/98719680/227734494-7778ed71-9f84-4e93-b037-b169e9d53451.png)

### Case
CAD [here](https://a360.co/42u5nMa).

<img src="https://github.com/frosty6742/frozen-slimes-v2/blob/main/Pictures/Screenshot%202023-06-21%20091806.png" alt="PCB" width="600" height="400" />

There are some varisous versions of the cases:

**Electronics Cover** - This is the part that slides over the top of the tracker to protect the electronics
- [ ] ECover.stl (This option has the switch soldered to the switch pads)  
- [ ] ECoverTopSwitch.stl (This option has the switch mounted on the top of the tracker)  

<br />

**Bottom Cover** - This is the part that hooks under the tracker to protect the connections
- [ ] BottomCover.stl (This is the standard choice, use it if you are directly soldering the switch on)  
- [ ] BottomCoverThick.stl (This is a thicker version of the one above, its more rigid but the trackers are bigger)
<br />

- [ ] BottomCoverTopSwitch.stl (Use this if you are mounitng the switch on top of the tracker, if you are using the ECoverTopSwitch.stl)  
- [ ] BottomCoverTopSwitchThick.stl (This is a thicker version of the one above, its more rigid but the trackers are bigger)  

<br />



To install the top cover remove the battery holder and slide it on from the battery side of the pcb to the imu side of the case, resolder on the battery holder. 


<img src="https://github.com/frosty6742/frozen-slimes-v2/blob/main/Pictures/IMG_1064.jpg" alt="PCB" width="533" height="400" /> 


If you want a case around the extension bmis check out whitneys artcturus cases and extensions: 
[Arcturus Cases](https://github.com/Lixulia/Arcturus)
 <br />
 
### Printing 
![image](https://github.com/frosty6742/frozen-slimes-v2/assets/98719680/6f6b50f8-9b07-4e87-9ddf-3a423ee4f30b)
Print in this orientation with NO SUPPORTS. 
20% infill is good.


### Assembly 
Steps 
- [ ] Print main tracker case

- [ ] Solder charge board to PCB
- [ ] Solder mpu to PCB 
- [ ] Solder pins from wemo D1 to wemo, set through holes on PCB and solder the pins on the backside of the PCB

- [ ] Add 180K resitor and diodes in the same orientation as the picture 
- [ ] Bridge correct pads to chose imu (no bridge for mpu6050)
- [ ] Solder on battery holder
- [ ] Solder on switch

- [ ] Check connections with multimeter for contunity 

- [ ] Feel free to reach out to me with any questions 

### Flashing firmware 

Make sure to install the slime vr server with drivers first. 
If the slime vr drivers arent working for you:
- [ ] Uninstall the drivers from device manager 
- [ ] Extract and install [this CH340 driver](https://www.wemos.cc/en/latest/ch340_driver.html)
- [ ] Flash the trackers 



BMI Specific Instructions:
- [ ] Use this online [firmware flasher](https://slimevr-firmware.bscotch.ca/) with this fork "0forks/v3dev".

- [ ] Orientation: 

![221204855-9bce6008-605c-4c25-83e0-810afc768479](https://user-images.githubusercontent.com/98719680/227734508-38e85ab7-38b9-43e7-b7cb-f7d4d2efbc29.png)


- [ ] [Calibrate](https://github.com/SlimeVR/SlimeVR-Tracker-ESP?files=1#bmi160) bmis for first use


### Links
Resources:
- [The Docs (SlimeVR Documentation)](https://docs.slimevr.dev/)
- [Github Repository SlimeVR](https://github.com/SlimeVR/)
- [SlimeVR Discord](https://discord.gg/SlimeVR)










### Community Builds
I love seeing everyone building and using my pcbs, send in your photos if you want them featured!

![227595175-0b3c58bc-bebe-40f4-a213-303ace0f15fe](https://user-images.githubusercontent.com/98719680/227734562-431fad07-ec83-4c5a-b0dc-b85b5ef90da1.png)

![Screenshot 2023-03-25 110515](https://user-images.githubusercontent.com/98719680/227734529-8239390f-cc73-430a-8573-4deac898a3bc.png)


![227594965-319fff3d-ec7c-4dd1-b06a-6c97975d8db4](https://user-images.githubusercontent.com/98719680/227734523-fe025773-85c6-469c-bbe0-94ca9602a039.png)

![IMG_20230514_153835964](https://github.com/frosty6742/frozen-slimes-v2/assets/98719680/b7d99d02-0ce7-43bd-830b-89857c67099f)

![image](https://github.com/frosty6742/frozen-slimes-v2/assets/98719680/22d0171f-0c6f-494a-b239-06caf8cf1ce0)


