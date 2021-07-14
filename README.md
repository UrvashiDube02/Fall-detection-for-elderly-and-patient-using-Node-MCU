# Fall-detection-for-elderly-and-patient-using-Node-MCU

![image](https://user-images.githubusercontent.com/87383888/125567049-31f067bc-170a-452d-89de-587f5dcaea00.png)

![image](https://user-images.githubusercontent.com/87383888/125567065-292458bd-233d-469b-852c-6f2a8fb067db.png)

 **ABSTRACT**

Falling down is too risky to many old people. If they fall, we must help them as soon as possible before any accidents happen. The problem is we can't always keep watch on 
their activities. The considerable risk of falls and the substantial increase in the elderly population make the automatic fall detection system very important. Existing fall detection systems using accelerometer have detectors that are often designed based on an empirical acceleration threshold to differentiate falls from normal activities. An optimal detection threshold can be obtained which meets the specified false alarm rate while maximizing the detection probability. So, in this project I have created a prototype of fall detection to solve the problem above. This device will send an alert to your email and a message if fall is detected.
 

**FORMULATION**

To apply the proposed fall-detection algorithm and detect falls, a wearable fall-detection device has been designed and produced In the past decade, the population in the world has been increasingly aging [The elderly, especially those above the age of 65, are exposed to falls owing to the deterioration of their physical functions. When an elder person falls and becomes unconscious or is unable to move his/her body, he/she may succumb to the injuries that caused the fall. Thus, research and development of a system that can automatically detect falls in the elderly or other patients has been actively studied Because of the expansion of the Internet in the 90s, it is now commonly referred to as the Internet of Things (IoT). The pervasive and seamless interaction among objects, sensors, and computing devices is an important concern of the IOT . Smart embedded objects such as a fall-detection sensor with wireless communication will also become an important part of the IoT. The identified fall-detection systems can be classified primarily into two categories: contextaware systems and wearable devices Wearable device-based approaches rely on clothing with embedded sensors to detect the motion and location of the body of the subject. The advantages of wearable devices are the cost efficiency, ease of installation, setup, and operation of the design. In this project , a fall-detection algorithm using 3-axis acceleration is proposed. The fall-feature parameters, calculated from the 3-axis acceleration, are applied to a simple threshold method.


**MATERIALS NEEDED**

Hardware needed : 

1.NodeMCU ESP8266 1.2 MPU6050 triple axis acc gyro NodeMCU ESP8266 

Software needed : 

1. Arduino IDE 
2. IFTTT
3. Other equipments: 3.1.Connecting wires 
2. LED 
3. Switch 
4. Bred board 
5. Lithium ion battery

![image](https://user-images.githubusercontent.com/87383888/125567591-9fc4d76e-aec0-4639-9c6d-74a8f8e27bc6.png)

![image](https://user-images.githubusercontent.com/87383888/125567605-9d0a1b14-3dc9-404f-9fc2-4dea15d1f110.png)

**CIRCUIT DIAGRAM**

![image](https://user-images.githubusercontent.com/87383888/125567640-3a044f14-62cb-4433-ab29-1bdf43550959.png)

**LITERATURE REVIEW**

The purpose of this literature review is to systematically assess the current state of design and implementation of fall detection devices. It also examines the extent to which 
these devices have been tested in the real world as well as the acceptability of these devices to older adults. A wearable device can detect the elderly's falling by acceleration analysis. Then it will get the elderly's geographic position and send fall alarm short message to caregivers. So the elderly who has fallen can get timely help to minimize the negative influence. 

Coordinate and gravity before and after falling:

(a) Before falling. 

(b) After falling.

![image](https://user-images.githubusercontent.com/87383888/125567712-6534cd2a-3907-4a43-8aca-575b5068961d.png)

**PROJECT DESIGN AND METHODOLOGY**

The microcontroller (NodeMCU) is connected to MPU6050 (accelerometer and gyroscope sensor). When the person falls, there is an increase in the acceleration of the sensor, and after it crosses the threshold limit the LED is turned on which changes the channel value in IFTTT. A trigger is setup in such a way that when the channel value changes in IFTTT an SMS is sent to the numbers specified. 

![image](https://user-images.githubusercontent.com/87383888/125567816-7a6a2044-9554-4904-b5dd-0aaea7db911a.png)

**CONNECTIONS**

![image](https://user-images.githubusercontent.com/87383888/125567802-6edc7041-033f-48ba-ac53-4ee31350a532.png)

**CODE**

![image](https://user-images.githubusercontent.com/87383888/125568299-7f9aaddb-98a5-4f2b-b796-80eb46ef607f.png)

![image](https://user-images.githubusercontent.com/87383888/125568323-3bfe3b2b-9c55-4178-90cd-d0c70e0fa9b3.png)

![image](https://user-images.githubusercontent.com/87383888/125568375-279e0e61-9970-4092-a556-adc2e0be493d.png)

![image](https://user-images.githubusercontent.com/87383888/125568418-99fc8762-1508-4ce4-84e7-4e6c50cfbdcf.png)

![image](https://user-images.githubusercontent.com/87383888/125568444-22cf9aac-798d-4aa0-b203-082d2fb51741.png)


**OBSERVATION**

When acceleration is above the threshold limit, the LED turns on and as a result of that an SMS is sent to the specified mobile numbers stating the immediate requirement of attention to the user. Before the acceleration reaches the threshold

![image](https://user-images.githubusercontent.com/87383888/125567907-2ebfa893-1e35-4a29-90a0-15c4fcfcb860.png)

![image](https://user-images.githubusercontent.com/87383888/125567938-da5fa746-384d-450f-8e21-41dd37af3348.png)

After the acceleration crosses the threshold

![image](https://user-images.githubusercontent.com/87383888/125567969-fe084877-a487-4921-8c59-94f63fd8dea7.png)

![image](https://user-images.githubusercontent.com/87383888/125567983-d088a86b-5b21-452b-981e-8d4ab30b82cb.png)

**MESSAGE NOTIFICATION**

![image](https://user-images.githubusercontent.com/87383888/125568052-2947e497-4422-4e82-9360-36f5a186e9b2.png)

![image](https://user-images.githubusercontent.com/87383888/125568071-5fe18b6a-dc53-426a-86b5-ed9ce461b89a.png)

**IFTT CHANNEL GRAPH**

![image](https://user-images.githubusercontent.com/87383888/125568147-aed82c4b-56a9-43c8-9653-15d409810d2b.png)

**CONCLUSION**

A lot of cases where old people and even young ones in general suffer from falling due to various reasons such as heart attack go unnoticed as there isn’t a simple device 
available to them which can detect their fall and send a notification to the people concerned. In today’s society a device like this is really important because most people 
stay away from their elderly due to work and it is practically impossible to get to know if something bad happens at any point as old people are not that well versed with 
technology either. The device serves the purpose of sending an SMS to the users specified. It relies on the use of the MPU6050 sensor consisting of an accelerometer and 
gyroscope which is used to note the acceleration readings. When the acceleration goes above the threshold an SMS is sent to whosever’s number is specified in the IFTTT service


