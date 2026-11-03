<a href="https://github.com/NotAScratch/Autonomous-Mapping-and-Navigation">
  <img src="assets/aqua-abyss/banner.svg" width="100%" alt="Samir Sen: robotics, machine learning and embedded systems. An animated LiDAR scan sweeps a room." />
</a>

<p align="center">
  <a href="https://notascratch.github.io/Samir-Sen/"><img src="https://img.shields.io/badge/Portfolio-060c1a?style=for-the-badge&logo=googlechrome&logoColor=2fd8b0" alt="Portfolio" /></a>
  <a href="https://x.com/samirsen66"><img src="https://img.shields.io/badge/@samirsen66-060c1a?style=for-the-badge&logo=x&logoColor=white" alt="X / Twitter" /></a>
  <a href="https://github.com/NotAScratch?tab=followers"><img src="https://img.shields.io/github/followers/NotAScratch?style=for-the-badge&logo=github&label=Followers&labelColor=060c1a&color=f9b9cc" alt="GitHub followers" /></a>
</p>

<img src="assets/aqua-abyss/intro.svg" width="100%" alt="I build things that sense, decide and move. Right now that means a Jetson-powered robot that I'm teaching to map a room. I write the SLAM stack myself, starting from the raw LiDAR bytes, then benchmark it against the production tools. Alongside it runs a Gazebo digital twin, so the same code is tested in simulation before it touches the hardware. Every project here is written as an open research log." />

## Featured research

<p align="center">
  <a href="https://github.com/NotAScratch/Autonomous-Mapping-and-Navigation"><img src="assets/aqua-abyss/card-slam.svg" width="49%" alt="Autonomous Mapping and Navigation: SLAM from scratch on a real wheeled robot" /></a>
  <a href="https://github.com/NotAScratch/rosmaster-r2-sim"><img src="assets/aqua-abyss/card-sim.svg" width="49%" alt="Rosmaster R2 Sim: Gazebo digital twin with 16/16 parity checks passing" /></a>
  <a href="https://github.com/NotAScratch/Monkey-Deterrence"><img src="assets/aqua-abyss/card-bandar.svg" width="49%" alt="Bandar Sentinel: edge-AI monkey detection and non-lethal deterrence" /></a>
  <a href="https://github.com/NotAScratch/AQI-Monitor"><img src="assets/aqua-abyss/card-aqi.svg" width="49%" alt="AQI Monitor: ESP32 PM2.5 monitor streaming to ThingsBoard" /></a>
</p>

## Lab status

<img src="assets/aqua-abyss/lab-status.svg" width="100%" alt="Research roadmap: the real robot is on phase 1 of 12 (talking to hardware); the simulation twin has finished phase 4 (parity) and is moving to SLAM and Nav2." />

<details>
<summary><b>Recent findings</b></summary>
<br />

- **Don't trust device names.** `/dev/rplidar` and `RPLIDAR_TYPE` pointed to a Slamtec RPLidar. Tracing the vendor launch files showed the sensor is actually a **YDLIDAR 4ROS** at 512000 baud. I now decode its packet protocol with my own code.
- **The real EKF runs unchanged in simulation.** It matches within 0.9% on distance and 2.8% on turning.
- **A bug the twin surfaced:** the robot's shipped EKF config fuses two absolute yaw sources, which makes `/odom` zig-zag.

</details>

## More from the lab

<p>
<a href="https://github.com/NotAScratch/FYP_Object_detection"><img src="assets/aqua-abyss/row-fyp.svg" width="100%" alt="FYP_Object_detection: SSD MobileNet V3 object detection with a Python API and Spring Boot web app" /></a>
<a href="https://github.com/NotAScratch/Real-Time-Object-Detection-and-Distance-Measurement-with-Computer-Vision"><img src="assets/aqua-abyss/row-distance.svg" width="100%" alt="Real-Time Object Detection and Distance: detects objects in live video and estimates their distance" /></a>
<a href="https://github.com/NotAScratch/Neural-Networks"><img src="assets/aqua-abyss/row-nn.svg" width="100%" alt="Neural-Networks: LSTM and TensorFlow/Keras experiments" /></a>
<a href="https://github.com/NotAScratch/Natural-Language-Processing"><img src="assets/aqua-abyss/row-nlp.svg" width="100%" alt="Natural-Language-Processing: sentiment analysis, word clouds and ensemble learning" /></a>
<a href="https://github.com/NotAScratch/AI"><img src="assets/aqua-abyss/row-ai.svg" width="100%" alt="AI: BFS vs DFS, KNN, SVM and disease prediction" /></a>
<a href="https://github.com/NotAScratch/Weather-Prediction"><img src="assets/aqua-abyss/row-weather.svg" width="100%" alt="Weather-Prediction: end-to-end regression on weather data" /></a>
<a href="https://github.com/NotAScratch/House-Price-Prediction"><img src="assets/aqua-abyss/row-house.svg" width="100%" alt="House-Price-Prediction: predicts house prices from location, size and amenities" /></a>
<a href="https://github.com/NotAScratch/Learning-Pyspark"><img src="assets/aqua-abyss/row-spark.svg" width="100%" alt="Learning-Pyspark: distributed data processing with Spark" /></a>
<a href="https://github.com/NotAScratch/ESP-32-DHT-11-gsm-module-live-humidity-and-temprature-monitoring"><img src="assets/aqua-abyss/row-esp32.svg" width="100%" alt="ESP-32 Climate Monitor: live temperature and humidity over cloud and GSM" /></a>
<a href="https://github.com/NotAScratch/Arduino-BT-CAR"><img src="assets/aqua-abyss/row-btcar.svg" width="100%" alt="Arduino-BT-CAR: a Bluetooth-controlled rover" /></a>
</p>

## Also in the works

<sub>Private or early-stage. More when they're ready.</sub>

- 🦾 **A second robot platform:** bringing up a larger, more agile robot base
- 🛒 **Retail robotics:** an interactive in-store robot built to catch shoppers' attention
- 🎯 **Vision-based tracking:** following moving targets in real time
- 🌾 **Agri-tech:** digital tools for farms and the supply chains around them
- 🏠 **A property platform** for the local market
- 📱 **An offline-first mobile app** for exam preparation
- 💼 **A job-matching platform**

## Toolbox

**Robotics** &nbsp;
<img src="https://img.shields.io/badge/ROS_2-22314E?style=flat-square&logo=ros&logoColor=white" alt="ROS 2" />
<img src="https://img.shields.io/badge/Gazebo-F58113?style=flat-square&logo=gazebo&logoColor=white" alt="Gazebo" />
<img src="https://img.shields.io/badge/Jetson-76B900?style=flat-square&logo=nvidia&logoColor=white" alt="NVIDIA Jetson" />
<img src="https://img.shields.io/badge/SLAM_·_EKF_·_Nav2-060c1a?style=flat-square" alt="SLAM, EKF, Nav2" />

**AI / ML** &nbsp;
<img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" alt="PyTorch" />
<img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white" alt="TensorFlow" />
<img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white" alt="OpenCV" />
<img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white" alt="scikit-learn" />
<img src="https://img.shields.io/badge/Spark-E25A1C?style=flat-square&logo=apachespark&logoColor=white" alt="Apache Spark" />
<img src="https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white" alt="Jupyter" />

**Embedded** &nbsp;
<img src="https://img.shields.io/badge/ESP32-E7352C?style=flat-square&logo=espressif&logoColor=white" alt="ESP32" />
<img src="https://img.shields.io/badge/Arduino-00878F?style=flat-square&logo=arduino&logoColor=white" alt="Arduino" />
<img src="https://img.shields.io/badge/PlatformIO-F5822A?style=flat-square&logo=platformio&logoColor=white" alt="PlatformIO" />
<img src="https://img.shields.io/badge/MQTT-660066?style=flat-square&logo=mqtt&logoColor=white" alt="MQTT" />

**Languages & backend** &nbsp;
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python" />
<img src="https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white" alt="C++" />
<img src="https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white" alt="Java" />
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript" />
<img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white" alt="Spring Boot" />
<img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black" alt="Linux" />

---

<p align="center">
  <sub>Off the keyboard: ♟️ chess · 🃏 poker · 🎣 fishing · ⚽ football</sub><br />
  <sub><i>Curious by default. Building to find out.</i></sub>
</p>
