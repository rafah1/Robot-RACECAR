# Robot-RACECAR

Robot-RACECAR is an autonomous AI racecar, based on Nvidia a 1/10th scale R/C racing chassis, using a Nvidia Jetson Nano SBC, a single camera input, and a servo controller.  


## References

Robot-RACECAR is based on Nvidia IOT Jetbot resources, and inspired by Nvidia Jetracer:

https://github.com/NVIDIA-AI-IOT/jetbot

https://github.com/NVIDIA-AI-IOT/jetcam

https://github.com/NVIDIA-AI-IOT/jetcard

https://github.com/NVIDIA-AI-IOT/jetracer

https://github.com/NVIDIA-AI-IOT/torch2trt


## Project Presentation
Robot-RACEACAR Presentation Video:

https://youtu.be/KQGQ4Fs-Uek



## 1. Introduction:

R/C Scale car racing is a world-wide popular hobby, but scale cars can also be used as models for education and investigation purposes. The use of scale models allows us to model the real world in a controlled environment to proof and teach concepts, do research, or even take risks that we would never take in real scale.

[Autonomous car racing](https://en.wikipedia.org/wiki/Autonomous_racing#:~:text=Autonomous%20or%20self%2Ddriving%20racing,E%20spin%2Doff%20series%20Roborace.) is an evolving international sport. Scale car racing has become a prime playground for self-driving vehicle experimentation. Multiple organizations use scale racecars in education and experimentation, like MIT, UPenn, AWS, etc. Several groups have started organizing and hosting autonomous scale racecars competitions. Some common vehicle R/C scales are 1/4, 1/5, 1/16, and 1/10, the last being the most popular.

I wanted to prove if I could convert one of my 1/10 scale electric R/C racing cars in a self-driving 1/10 racecar robot, with a Jetson Nano SBC, and a servo motor controller onboard. This autonomous racecar robot would be tested on its ability to drive as fast as possible in a closed course, solving lane detection, obstacle evasion, obstacle avoidance changing lanes changing as outrunning other racecars. Solving these challenges, this self-drive racecar should be able to compete in time-based laps competitions, like the ones hosted by DIY Robocars groups.

 **1.1. Goals of the Project:**
  
 1.1.1. Build a self-driving 1/10 scale electric racecar hardware which is more cost efficient and of better quality, based in an existing R/C chassis with a Nvidia Jetson Nano SBC onboard, as well as purchasing a few parts on amazon to build it. This turns out to be better overall than acquiring a robot kit like the [jetracer-Pro](https://www.waveshare.com/jetracer-pro-ai-kit.htm) from waveshare, or the [AWS deepRacer](https://www.amazon.com/dp/B07JMHRKQG) from amazon.

1.1.2. Develop the software solution to allow the racecar robot to drive, as fast as possible, in a closed course track with multiple lanes.

1.1.3. Solve autonomous navigation challenges in a closed course like: lane detection, obstacle evasion, and obstacle avoidance changing lanes changing as outrunning other racecars.

**1.2. Level of Autonomy**

The robot racecar should be able to be fully autonomous; with a predefined number of laps. The racecar will be placed on the start line, and a start action will trigger the car to complete the circuit in the shortest time possible.

Any human intervention during the race will disqualify the robot racecar. In this sense the racecar is considered to be within autonomy level 5.

Autonomous car racing is quickly becoming a new sport, like the new autonomous Indi-Car racing. Advancements in scale car racing will contribute to this nascent industry.

  1. **Description**

- Robot Racecar Hardware System overview

![](RackMultipart20210512-4-7shque_html_ab00d50affbf0700.gif)

- GPIO Diagram:

![](RackMultipart20210512-4-7shque_html_f95526e0bbfeb7ca.gif)

- Architecture of the application:
 ![](RackMultipart20210512-4-7shque_html_13c169975070f9de.gif)
 
 
 
## Cars

There are two different JetRacer cars that you can build.  They differ primarily in size and speed.  Which one to pick depends on your use case

|  Latrax Rally | Tamiya TT02 |
|--------------|---------------|
| <img src="https://user-images.githubusercontent.com/25759564/67250038-b1c22e00-f41e-11e9-82d2-bbb17526310b.jpg" width=256>  | <img src="https://user-images.githubusercontent.com/25759564/67250039-b1c22e00-f41e-11e9-931f-98c1729550d0.jpg" width=320>  | 
| 1/18th scale |  1/10th scale |
| Moderate Speed  |  High Speed  |
| ~$400 total build cost | ~$600 total build cost |
| Compact and portable |  Large and easy to modify |
| Soldering required |  No soldering required  |
| Base car pre-assembled | Base car assembly required |

If you have any questions, please reach out by [creating an issue](../..//issues).


## Examples

JetRacer comes with a couple examples to get you up and running.  The examples are in the format of Jupyter Notebooks, which are interactive documents which combine text, code, and visualization.  Once you've completed the notebooks, start tweaking them to create your own racing software!

### Example 1 - Basic motion

In this example you'll learn to progam JetRacer programatically from your web browser.  Learn more in the [examples](docs/examples.md) documentation.

<img src="https://user-images.githubusercontent.com/4212806/60383497-68d90a80-9a26-11e9-9a18-778b7d3a3221.gif" height=300/>

### Example 2 - Road following

In this example, you'll teach JetRacer how to follow a road using AI.  After training the neural network using the [interactive training notebook](notebooks/interactive_regression.ipynb), you'll optimize the model using NVIDIA TensorRT and deploy for a live demo. Learn more in the [examples](docs/examples.md).

<img src="https://user-images.githubusercontent.com/4212806/60383389-bd7b8600-9a24-11e9-9f64-926e5edb52cc.gif" height=300/>

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
