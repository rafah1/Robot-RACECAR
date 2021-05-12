# Robot-RACECAR

Robot-RACECAR is an autonomous AI racecar, based on:
* 1/10th scale R/C racing chassis
* Nvidia Jetson Nano SBC
* single camera input
* servo controller 


## References

Robot-RACECAR is based on Nvidia IOT Jetbot resources:

https://github.com/NVIDIA-AI-IOT/jetbot

https://github.com/NVIDIA-AI-IOT/jetcam

https://github.com/NVIDIA-AI-IOT/jetcard

https://github.com/NVIDIA-AI-IOT/jetracer

https://github.com/NVIDIA-AI-IOT/torch2trt


## Project Presentation
Robot-RACEACAR Project Presentation Video:

https://youtu.be/KQGQ4Fs-Uek



## 1. Introduction:

R/C Scale car racing is a world-wide popular hobby, but scale cars can also be used as models for education and investigation purposes. The use of scale models allows us to model the real world in a controlled environment to proof and teach concepts, do research, or even take risks that we would never take in real scale.

[Autonomous car racing](https://en.wikipedia.org/wiki/Autonomous_racing#:~:text=Autonomous%20or%20self%2Ddriving%20racing,E%20spin%2Doff%20series%20Roborace.) is an evolving international sport. Scale car racing has become a prime playground for self-driving vehicle experimentation. Multiple organizations use scale racecars in education and experimentation, like [MIT](https://racecar.mit.edu/), [UPenn](https://f1tenth.org/), [AWS](https://aws.amazon.com/deepracer/), etc. Several groups have started organizing and hosting autonomous scale racecars competitions. Some common vehicle R/C scales are 1/4, 1/5, 1/16, and 1/10, the last being the most popular.

I wanted to prove if I could convert one of my 1/10 scale electric R/C racing cars in a self-driving 1/10 racecar robot, with a Jetson Nano SBC, and a servo motor controller onboard. This autonomous racecar robot would be tested on its ability to drive as fast as possible in a closed course, solving lane detection, obstacle evasion, obstacle avoidance changing lanes changing as outrunning other racecars. Solving these challenges, this self-drive racecar should be able to compete in time-based laps competitions, like the ones hosted by [DIY Robocars groups](https://diyrobocars.com/).

**1.1. Goals of the Project:**
  
 1.1.1. Build a self-driving 1/10 scale electric racecar hardware which is more cost efficient and of better quality, based in an existing R/C chassis with a Nvidia Jetson Nano SBC onboard, as well as purchasing a few parts on amazon to build it. This turns out to be better overall than acquiring a robot kit like the [jetracer-Pro](https://www.waveshare.com/jetracer-pro-ai-kit.htm) from waveshare, or the [AWS deepRacer](https://www.amazon.com/dp/B07JMHRKQG) from amazon.

1.1.2. Develop the software solution to allow the racecar robot to drive, as fast as possible, in a closed course track with multiple lanes.

1.1.3. Solve autonomous navigation challenges in a closed course like: lane detection, obstacle evasion, and obstacle avoidance changing lanes changing as outrunning other racecars.

**1.2. Level of Autonomy**

The robot racecar should be able to be fully autonomous; with a predefined number of laps. The racecar will be placed on the start line, and a start action will trigger the car to complete the circuit in the shortest time possible.

Any human intervention during the race will disqualify the robot racecar. In this sense the racecar is considered to be within autonomy level 5.

Autonomous car racing is quickly becoming a new sport, like the [Roborace Alpha](https://en.wikipedia.org/wiki/Roborace), or the new [Indy Autonomous Challenge](https://www.indyautonomouschallenge.com/). Advancements in scale car racing will contribute to this nascent industry.

**1.3 Description**

- Robot Racecar Hardware System overview

<img src="https://github.com/rafah1/Robot-RACECAR/blob/main/Final%20Project%20Robot%20RACECAR%20Presentation%20Slides/Slide18.jpeg" height=300/>

- GPIO Diagram:

<img src="https://github.com/rafah1/Robot-RACECAR/blob/main/Final%20Project%20Robot%20RACECAR%20Presentation%20Slides/Slide13.jpeg" height=300/>

- Architecture of the application:
<img src="https://github.com/rafah1/Robot-RACECAR/blob/main/Final%20Project%20Robot%20RACECAR%20Presentation%20Slides/Slide11.jpeg" height=300/>
 
 
 
## Cars

**4.3 Hardware needed:**

4.3.1 Racecar Proof of Concept Bill of Materials:

| **Part** | **Quantity** | **Cost** | **Store / URL** |
| --- | --- | --- | --- |
| Vintage Tamiya RC Car | 1 | N/A | Tamiya TA02 chassis with 2 servos or servo/ESC combo or equivalent |
| Jetson Nano | 1 | $89.00 | [Microcenter Nvidia](https://developer.nvidia.com/buy-jetson) |
| Micro SD Card 128GB | 1 | $19.99 | [Amazon](https://www.amazon.com/SanDisk-128GB-MicroSDXC-Memory-Adapter/dp/B08GYKNCCP/ref=sr_1_3?crid=3THXX9QW3YBHV&amp;dchild=1&amp;keywords=sandisk+micro+sd+card&amp;qid=1615155574&amp;s=electronics&amp;sprefix=sands%2Celectronics%2C170&amp;sr=1-3) |
| USB Battery 20000mAh with display | 1 | $13.99 | [Amazon](https://www.amazon.com/24000mAh-Portable-External-Charging-Smartphones/dp/B07LFS3MQZ/ref=sr_1_3?dchild=1&amp;keywords=20000+battery+pack&amp;qid=1615156869&amp;sr=8-3) |
| USB A -\&gt; 2.1mm Barrel Cable | 1 | $7.00 | [Amazon](https://amzn.to/2SMmu8A) |
| RC battery pack | 1 | $39.99 | [Amazon](https://amzn.to/31330PW) |
| RC battery charger | 1 | $20.99 | [Amazon](https://amzn.to/2GHi3ay) |
| PWM Servo Motor Driver | 1 | $6.99 | [Amazon](https://amzn.to/317xYqr) |
| Micro USB cable | 1 | $1.00 | [Dollar Store](https://www.dollartree.com/e-circuit-micro-usb-cables-39-in/259578) |
| Double-sided tape | 1 | $1.00 | [Dollar Store](https://www.dollartree.com/crafters-square-doubled-sided-tape-33ft/281210) |
| Foam Board | 1 | $1.00 | [Dollar Store](https://www.dollartree.com/readi-board-white-foam-boards/809955) |

4.3.2 Robot Racecar 1.0 Bill of Materials:

<img src="https://github.com/rafah1/Robot-RACECAR/blob/main/Picture1.png" height=300/>
<img src="https://github.com/rafah1/Robot-RACECAR/blob/main/Picture2.png" height=300/>

(This bill of materials is inspired on the [Nvidia jetracer](https://github.com/NVIDIA-AI-IOT/jetracer/blob/master/docs/tamiya/bill_of_materials.md), with modifications which reduce the cost and also improves some components)
All components are mounted to the wooden tray using the nylon standofs kit (the tray can be easily perforated). For the wiring you can check [here](https://github.com/NVIDIA-AI-IOT/jetracer/blob/master/docs/tamiya/hardware_setup.md)

| **Part** | **Quantity** | **Cost** | **Store / URL** |
| --- | --- | --- | --- |
| 1/10 Tamiya RC Car based on TT02 Chassis w/ESC and brushed motor | 1 | $100 - 130 | [amain](https://www.amainhobbies.com/search?s=tt02+electric) |
| Hi torque metal servo | 1 | $16.66 | [Amazon](https://www.amazon.com/gp/product/B01MU7TQV8/ref=ppx_yo_dt_b_asin_title_o04_s00?ie=UTF8&amp;psc=1) |
| Jetson Nano | 1 | $89.00 | [Microcenter Nvidia](https://developer.nvidia.com/buy-jetson) |
| Micro SD Card 128GB | 1 | $19.99 | [Amazon](https://www.amazon.com/SanDisk-128GB-MicroSDXC-Memory-Adapter/dp/B08GYKNCCP/ref=sr_1_3?crid=3THXX9QW3YBHV&amp;dchild=1&amp;keywords=sandisk+micro+sd+card&amp;qid=1615155574&amp;s=electronics&amp;sprefix=sands%2Celectronics%2C170&amp;sr=1-3) |
| Wi-Fi card w/6DBi antennas | 1 | $26.90 | [Amazon](https://www.amazon.com/gp/product/B07X2NLL85/ref=ppx_yo_dt_b_asin_title_o05_s02?ie=UTF8&amp;psc=1) |
| Camera 160 Degree Wide Angle | 1 | $29.80 | [Amazon](https://www.amazon.com/gp/product/B07T43K7LC/ref=ppx_yo_dt_b_asin_title_o05_s02?ie=UTF8&amp;psc=1) |
| USB Battery 20000mAh with display | 1 | $13.99 | [Amazon](https://www.amazon.com/24000mAh-Portable-External-Charging-Smartphones/dp/B07LFS3MQZ/ref=sr_1_3?dchild=1&amp;keywords=20000+battery+pack&amp;qid=1615156869&amp;sr=8-3) |
| USB A -\&gt; 2.1mm Barrel Cable | 1 | $7.00 | [Amazon](https://amzn.to/2SMmu8A) |
| Battery Strap Pack | 1 | $7.99 | [Amazon](https://www.amazon.com/gp/product/B01CJG5JV2/ref=ppx_yo_dt_b_asin_title_o04_s00?ie=UTF8&amp;psc=1) |
| RC battery pack | 1 | $39.99 | [Amazon](https://amzn.to/31330PW) |
| RC battery charger | 1 | $20.99 | [Amazon](https://amzn.to/2GHi3ay) |
| PWM Servo Motor Driver | 1 | $6.99 | [Amazon](https://amzn.to/317xYqr) |
| Micro USB cable | 1 | $1.00 | [Dollar Store](https://www.dollartree.com/e-circuit-micro-usb-cables-39-in/259578) |
| Wooden tray / Foam board | 1 | $1.00 | [Dollar Store](https://www.dollartree.com/crafters-square-wooden-tray/296724) |
| Nylon Hex Standoffs and Nuts Kit | 1 | $12.99 | [Amazon](https://www.amazon.com/gp/product/B015S27EG2/ref=ppx_yo_dt_b_asin_title_o05_s00?ie=UTF8&amp;psc=1) |
| Jumper Wire Pack | 1 | $6.98 | [Amazon](https://www.amazon.com/gp/product/B01EV70C78/ref=ppx_yo_dt_b_asin_title_o06_s00?ie=UTF8&amp;psc=1) |
| M3 Universal Screw Pack | 1 | $12.94 | [Amazon](https://amzn.to/2LNGt6q) |
| RC 3-Channel Receiver (optional) | 1 | $10.99 | [Amazon](https://www.amazon.com/Flysky-FS-GR3E-Receiver-FS-GT2B-FS-GT3B/dp/B087ZKFGK7/ref=sr_1_21?dchild=1&amp;keywords=Flysky+RC+GR3E&amp;qid=1615159397&amp;s=toys-and-games&amp;sr=1-21) |
| RC 3-Channel Transmitter (optional) | 1 | $53.00 | [Amazon](https://www.amazon.com/FLYSKY-FS-GT3C-fsgt3c-2-4GHz-Transmitter/dp/B00B3NWVR8/ref=sr_1_19?dchild=1&amp;keywords=Flysky+RC+GR3E&amp;qid=1615159397&amp;s=toys-and-games&amp;sr=1-19) |
| RC Servo Multiplexer (optional) | 1 | $7.95 | [Amazon](https://www.amazon.com/gp/product/B00V3XMLEG/ref=ppx_yo_dt_b_asin_title_o02_s00?ie=UTF8&amp;psc=1) |
| Servo Extension Cable Pack (optional) | 1 | $7.99 | [Amazon](https://amzn.to/2SMnkSM) |




## Algorithms

This is where all the magic happens!

You will find under the notebooks project directory, a series of Jupyter notbooks with the code for the different experiments:

    interactive_regression1.ipynb
    interactive_regression1_ALEXNET.ipynb
    interactive_regression1_RESNET34.ipynb
    road_following1.ipynb
    road_following2.ipynb
    road_followin3.ipynb
    road_following1_ALEXNET.ipynb
    road_following1_RESNET34.ipynb


## Setup

To get started with JetRacer, follow these steps

1. Order parts from the bill of materials

    - [Latrax version](docs/latrax/bill_of_materials.md) 
    - [Tamiya version](docs/tamiya/bill_of_materials.md) 

2. Follow the hardware setup

    - [Latrax version](docs/latrax/hardware_setup.md) 
    - [Tamiya version](docs/tamiya/hardware_setup.md) 

3. Follow the [software setup](docs/software_setup.md)
4. Run through the [examples](docs/examples.md)

## See also

* [JetBot](http://github.com/NVIDIA-AI-IOT/jetbot) - An educational AI robot based on NVIDIA Jetson Nano

* [JetCam](http://github.com/NVIDIA-AI-IOT/jetcam) - An easy to use Python camera interface for NVIDIA Jetson
* [JetCard](http://github.com/NVIDIA-AI-IOT/jetcard) - An SD card image for web programming AI projects with NVIDIA Jetson Nano
* [torch2trt](http://github.com/NVIDIA-AI-IOT/torch2trt) - An easy to use PyTorch to TensorRT converter
