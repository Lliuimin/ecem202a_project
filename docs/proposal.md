# Project Proposal

## 1. Motivation & Objective

More than 80% of information that human brain processes is visual. Therefore, visually impaired people face a great challenge of sensing the outside world, especially when they need to move through an unknown environment. The goal of this project is to build an low-cost, robust and user-friendly obstacle avoidance system, with Arduino Nano 33 BLE Sense, Raspberry Pi 3, Ultrasound module, IR camera, eSense earable compute platform, aid of a smartphone and other minor parts, to detect and warn obstacles for the visually impaired users, which improves their outdoor mobility, and quality of life.

## 2. State of the Art & Its Limitations

The most useful assistance for visually impaired people has been the guide dogs, which need to be trained at a high cost to navigate blind people through obstacles, and have physical needs to be taken care of. And in China, there are tens of millions of blind people with a total of two hundred guide dogs bred in ten years, and now less than one hundred are in service. Those who cannot afford a guide dog usually employ a white cane, which can only detect obstacles near to the ground.
With the development of electronics industry, a wide range of devices were invented to aid visually impaired people in their indoor and outdoor activities. Earliest inventions employ cheap ultrasonic and sonar sensors, which are still welcomed in today's designs, and lasers to detect the distance of obstacles. However, due to the difficulties in calibration, manual scanning and reflective error exclusion[1], those sensors are mostly used alongside more accurate detectors as auxiliary equipment.
Modern obstacle avoidance systems are embedded into wearable or portable devices. Examples of the former are Eyeronman[2] smart vest that uses vibration to translate sensor data to tactile information, and Project Guideline[3] belt that uses camera to sense and sound tone to provide feedback. The latter is mostly realized in the form of smart canes, including Augmented Cane [4] which employs a comprehensive set of modules including LIDAR, camera, GPS and IMU, whose data can be feedback to user with grounded kinesthetic omni-wheel, audio and push button, and WeWalk[5] which has ultrasonic above-ground obstacle detection, automatic voice feedback and smartphone application-aided navigation and transportation assistant.
The most obvious limitation of modern devices is high cost, mainly due to the employment of complicated sensors and high-standard algorithms. Also, a smart cane need to be held at all time, which limits the hand mobility of its user.

## 3. Novelty & Rationale

Our obstacle detection system utilizes relatively simple sensors (IR camera, ultrasonic sensors, Earable gyroscope) and control units (Arduino Nano 33 BLE Sense, Raspberry Pi) to achieve high accuracy and wide range  of obstacle detection, with fast, user-friendly voice feedback (Earable earphones). Current structure is: the IR camera, which is placed on the head of user, detects a wide range of obstacles, whose data is sent and processed by Raspberry Pi (RBPi), who classifies the obstacles and judges if any obstacle is too near and its distance to the user needs to be further measured. RBPi then sends data back to the controlling Arduino Nano 33 BLE Sense (Arduino). If the obstacles are near enough to the user, the ultrasonic sensors will measure the exact distance, and send data to its Arduino to be processed and then sent to the controlling Arduino. If there is indeed an obstacle that needs to be avoided, the controlling Arduino will communicate with Earable smartphone application via Bluetooth, which then communicates with Earable earphone to vocally remind the user of the obstacle.

## 4. Potential Impact

We intend to make a prototype of low-cost, high-accuracy obstacle detecting and warning system.  It will provide a new possibility of the choice and combination of sensors, controllers and smart phone applications, and a new way of user-device interaction to the industry of obstacle avoidance for visually impaired people. It allows blind people to improve their outdoor safe mobility, therefore quality of life, with relatively low cost.

## 5. Challenges

The first challenge of this project is the accuracy of ultrasonic sensors, which, being a cheap module, can sometimes be inaccurate due to reflection, and thus need to be calibrated with algorithms. The second challenge is to maintain the robustness of the system, for it has many components, especially camera recognition will take up a lot of computing time. All these parts need to work in accordance, being able to tolerate perturbations and interruptions.


## 6. Requirements for Success

What skills and resources are necessary to perform the project?
    • Arduino & Ultrasound
    • Raspberry Pi & IR camera
    • Earable & App development
The resources needed for this projects are listed below:
    • Devices
        ○ Arduino Nano 33 BLE Sense
        ○ Raspberry Pi 3
        ○ IR camera
        ○ Ultrasonic sensors
        ○ Earable earphones
        ○ Smartphone
        ○ Other auxiliary parts
    • Software
        ○ Arduino IDE
                ○ Android studio
        ○ Earable smartphone application
    • Background research materials
        ○ Various IEEE papers
        ○ Arduino and Raspberry Pi tutorials
The skills needed are:
    • Arduino and Raspberry Pi programming
    • Android application development (Java)
    • GitHub
    • Hardware usage, connection and debugging
    • Teamworking
    • Time management

## 7. Metrics of Success

A successful obstacle detecting and warning system must have the following properties: fast and accurate obstacle detecting, proper classification and judgement of obstacles, in-time and clear warning, easy operation and robustness. They can be qualified as:
    • The speed with which the system response to obstacle (in seconds)
    • The rate of successful obstacle detection (%), while the obstacles' type, distance, moving speed vary
    • The speed with which a user walks under the assistance of our system
    To measure those metrics, various tests and trials can be conducted.

## 8. Execution Plan

1. Obstacle detection and reminder 
2. Obstacle image recognition
3. Development of Earable application on Arduino smart phone
4. Programming the controller Arduino and communication between parts
Partitioning: 
Task 1 is to be done by Ruoye Wang, task 2,3 are to be done by Jinchen Wu, and task 4 is done together.

## 9. Related Work

### 9.a. Papers

List the key papers that you have identified relating to your project idea, and describe how they related to your project. Provide references (with full citation in the References section below).

### 9.b. Datasets

List datasets that you have identified and plan to use. Provide references (with full citation in the References section below).

### 9.c. Software

List softwate that you have identified and plan to use. Provide references (with full citation in the References section below).

## 10. References

[1] Hossain, E., Khan, M.R., Muhida, R. and Ali, A. (2011) ‘State of the art review on walking support system for visually impaired people’, Int. J. Biomechatronics and Biomedical Robotics, Vol. 1, No. 4, pp.232–251.
[2] https://tactilenavigationtools.com/#:~:text=The%20Eyeronman%2C%20is%20a%20hands,user's%20through%20superior%20situation%20awareness.
[3] Project Guideline: Can Technology Help A Blind Runner Navigate?
[4] P. Slade, A. Tambe, M. J. Kochenderfer, Multimodal sensing and intuitive steering assistance improve navigation and mobility for people with impaired vision. Sci. Robot. 6, eabg6594 (2021
[5] https://wewalk.io/en/


