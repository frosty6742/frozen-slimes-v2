# Frozen Slimes V2

### Contact: artemis#8615

## Check out the discord: https://discord.gg/vhHEsKjWGV

This project will currently be using a Wemo D1 mini, mpu6050, bmi160 or bno085s, and a TP4056 charger. On my personal slimes I wanted to use a 18650 batteries due to the longer battery life and how easy they are to get. 

This is the second version of the case with a hotswappable 18650, strap slots build into the pcb and a much improved pcb design. 

This will now also support mpu6050s, bmis160s, and BNO085s all on one pcb with toggles. 

Tested:
- mpu6050 = yes
- bmi160 = yes
- BNO085s = no

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
- [Links](#Links)


### Components   
- [TP4056](https://www.amazon.com/HiLetgo-Lithium-Battery-Charging-Protect/dp/B00LTQU2RK/ref=sr_1_3?crid=31BCDZYQGA5IU&keywords=TP4056&qid=1643591253&sprefix=tp4056%2Caps%2C124&sr=8-3)
- [Wemos D1 Mini](https://www.amazon.com/Organizer-ESP8266-Internet-Development-Compatible/dp/B081PX9YFV/ref=sr_1_3?crid=2FMF3NVYGOSPK&keywords=wemos+d1+mini&qid=1643591309&sprefix=wemos+d1+mini%2Caps%2C136&sr=8-3)
- [2in straps] Made these from elastic and velcro
- [IMU docs](https://docs.slimevr.dev/diy/components-guide.html)
    - [MPU6050](https://www.amazon.com/MPU-6050-Accelerometer-Gyroscope-Converter-Compatible/dp/B08TH9NH55/ref=sr_1_6?crid=1W65V3QJ27XN&keywords=mpu+6050&qid=1643591376&sprefix=mpu+6050%2Caps%2C136&sr=8-6)  
    - [BMI160]
- [Switch](https://docs.slimevr.dev/diy/components-guide.htmll)
    - [SS22F32](https://www.aliexpress.com/item/32975535599.html)
- [Battery](https://docs.slimevr.dev/diy/components-guide.html)
    - [18650](https://www.amazon.com/s?k=18650&crid=2H65KICLJGU4U&sprefix=18650%2Caps%2C301&ref=nb_sb_noss_1)
- [1n5817 Diode](https://www.amazon.com/100-Pieces-1N5817-Schottky-Rectifier/dp/B079KDQQPD/ref=sr_1_5?crid=1EPLYISD4R4G3&keywords=1n5817+Diode&qid=1659032765&sprefix=1n5817+diode%2Caps%2C130&sr=8-5)
- [180k Resistor](https://www.amazon.com/EDGELEC-Resistor-Tolerance-Resistance-Optional/dp/B07HDFCNXB/ref=sr_1_3?crid=9MPFJ93KJT6X&keywords=180k+resistor&qid=1659032821&sprefix=180k+%2Caps%2C129&sr=8-3)
- [18650 Battery Solderable Holder]



### Case
Still in work but the tracker will work even without the case.

Live updates of case CAD [here](https://a360.co/42u5nMa).


<img src="https://user-images.githubusercontent.com/98719680/227734265-6dffa7c5-9c2f-498a-8c37-c5e9e4d3c53d.png" alt="PCB" width="600" height="400" />


If you want a case around the extension bmis check out whitneys artcturus cases and extensions: 
[Arcturus Cases](https://github.com/Lixulia/Arcturus)



### PCB 

##Check above for tested and supported mpus

This PCB lets every component be soldered on without any extra wires. This includes the diodes and resistor for battery sense and protected charging. 

To order PCBS go to a website like https://cart.jlcpcb.com/quote upload the gerber file zip file and select quanity and color and order. It should autoselect all the other correct options when you upload the gerber file. 


*if you want to buy pcb packs, fully assembled pcbs or even whole trackers dm me*



<img src="https://github.com/frosty6742/frozen-slimes-v2/blob/main/Pictures/20230212_062153031_iOS.png" alt="PCB" width="600" height="400" /> 

<img src="https://github.com/frosty6742/frozen-slimes-v2/blob/main/Pictures/20230212_062336631_iOS.png" alt="PCB" width="400" height="500" /> 

<img src="https://github.com/frosty6742/frozen-slimes-v2/blob/main/Pictures/20230212_065153234_iOS.png" alt="PCB" width="600" height="400" /> 


![Screenshot 2023-02-10 085738](https://user-images.githubusercontent.com/98719680/227734494-7778ed71-9f84-4e93-b037-b169e9d53451.png)



### Printing 

![227603217-12ec5b41-bc10-43a8-856b-a48b9d3375ae](https://user-images.githubusercontent.com/98719680/227734497-a1913c7c-93c8-40bc-b744-7558b1a9abad.png)

### Assembly 
Steps 
- [ ] Print main tracker case

- [ ] Solder charge board to PCB
- [ ] Solder mpu to PCB 
- [ ] Solder pins from wemo D1 to wemo, set through holes on PCB and solder the pins on the backside of the PCB

- [ ] Add 180K resitor and diodes in the same orientation as the picture 
- [ ] Bridge correct pads to chose imu
- [ ] Solder on battery holder
- [ ] Solder on switch

- [ ] Check connections with multimeter for contunity 

- [ ] Feel free to reach out to me with any questions 

### Flashing firmware 





BMI Specific Instructions:
- [ ] Use this online [firmware flasher](https://slimevr-firmware.bscotch.ca/) with this fork "0forks/v3dev".

- [ ] Orientation: 

![221204855-9bce6008-605c-4c25-83e0-810afc768479](https://user-images.githubusercontent.com/98719680/227734508-38e85ab7-38b9-43e7-b7cb-f7d4d2efbc29.png)


- [ ] [Calibrate](https://github.com/SlimeVR/SlimeVR-Tracker-ESP/tree/beta/bmi-improvements#bmi160) bmis for first use


### Links
Resources:
- [The Docs (SlimeVR Documentation)](https://docs.slimevr.dev/)
- [Github Repository SlimeVR](https://github.com/SlimeVR/)
- [SlimeVR Discord](https://discord.gg/SlimeVR)










### Community Builds
I love seeing everyone building and using my pcbs, send in your photos if you want them featured!


![Screenshot 2023-03-25 110515](https://user-images.githubusercontent.com/98719680/227734529-8239390f-cc73-430a-8573-4deac898a3bc.png)


![227594965-319fff3d-ec7c-4dd1-b06a-6c97975d8db4](https://user-images.githubusercontent.com/98719680/227734523-fe025773-85c6-469c-bbe0-94ca9602a039.png)

