# wot-project-part1-EdgeDevice-sAncoramTamborrino
wot-project-part1-samueleancora created by GitHub Classroom

AN EDGE COMPUTING SOLUTION FOR DRIVER'S SAFETY

The aim of the project is to guarantee and monitor driver's life signals as well as inspect the environment inside the vehicle and manage it. To do so, the Edge Computing paradigm has been chosen to satisfy requirements in speed of elaboration and low delay. The system is composed of three main components: the edge, the server and the frontend.

The first component consists of a Raspeberry Pi 4 and the sensors, together with the code inside this repository.

The second component consists of the server, which is in charge to use machine learning to create a model based on data sent by the edge and to store them in a NoSQL database, MongoDB. Its repository can be reach at this address:https://github.com/UniSalento-IDALab-IoTCourse-2021-2022/wot-project-part2-Server-sAncoramTamborrino

The third component consists of the frontend page, where an external user can access to the digital twins of both driver and car, and get notified of occurred events. Its repository can be reach at this address:https://github.com/UniSalento-IDALab-IoTCourse-2021-2022/wot-project-part3-FrontEnd-sAncoramTamborrino

To give a better understanding of the architecture of the system, the following picture is attached.


![iotarch](https://user-images.githubusercontent.com/106089600/202003221-f3a556e3-e22e-4b43-8f91-3e7255d2c3a8.png)

The purpose of this component is to gather data from sensors and to build a dataframe which will be fed to the already trained model with machine learning to inspect the current situation and give a feedback to the server. Indeed, the edge will send to the server either the data from sensors either the outcome of the prediction according to the model.

To make the system work in the proper way in locale all the components must be in the same working directory with the following structure.
<img width="325" alt="Schermata 2022-10-25 alle 20 10 26" src="https://user-images.githubusercontent.com/106089600/205873399-49d2b136-8573-44a6-8a59-faf015b740b4.png">
