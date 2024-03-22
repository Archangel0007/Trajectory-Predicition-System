# Trajectory-Tracking-System

The primary objective of this project is to develop a comprehensive system for the accurate prediction of vehicle trajectories, with a particular focus on motorcycles, within a road environment. This undertaking encompasses three key components:

-><b>Vehicle Detection:<b/> <br>
Implementing advanced computer vision algorithms to identify and locate vehicles, specifically motorcycles, within video or image data streams. For this purpose I have chosen YOLOV8, whose source files can be found at https://github.com/ultralytics/ultralytics

-><b>Vehicle Tracking:<b/> <br>
Utilizing sophisticated tracking techniques to monitor and maintain the continuous identification and monitoring of vehicles as they move through the road scene.I have chosen DeepSort for this purpose. The required depedencies can be found at https://github.com/nwojke/deep_sort

-><b>Vehicle Trajectory Prediction:<b/> <br>
Employing predictive modeling methodologies to forecast the future paths and movements of vehicles, particularly motorcycles, based on their historical trajectories and current contextual data. I have Employed CNN-GRU and CNN-LSTM for this substep.<br><br> We give in the bounding boxes for 8 continuous frames of the tracked object, and the model predicts the next coordinate of the object based on these bounding box values. the Trained Models can be found in the Models Section of this repository. The code for training these models can be found at the Dataset and Training folder of the repository.



## Tech-Stack
<div><img src="https://camo.githubusercontent.com/d9170200b3894f1bb39610409a2b6bd82fa4e31f81156291b2040e6dfea09bf3/68747470733a2f2f63646e2e6a7364656c6976722e6e65742f67682f64657669636f6e732f64657669636f6e2f69636f6e732f7079746f7263682f7079746f7263682d6f726967696e616c2e737667" height="40px" width="40px">
<img src="https://camo.githubusercontent.com/26775c5884b7e016cd32a1ed450980e1d404c81b19077f7702f5e3e7c746dc5d/68747470733a2f2f63646e2e6a7364656c6976722e6e65742f67682f64657669636f6e732f64657669636f6e2f69636f6e732f74656e736f72666c6f772f74656e736f72666c6f772d6f726967696e616c2e737667" height="40px" width="40px">
<img src="https://camo.githubusercontent.com/5603e24b61199730db8d47721aeb6b7e6e0517ee6f43bb6762552a4d625607c9/68747470733a2f2f63646e2e6a7364656c6976722e6e65742f67682f64657669636f6e732f64657669636f6e2f69636f6e732f707974686f6e2f707974686f6e2d6f726967696e616c2e737667" height="40px" width="40px">
<img src="https://camo.githubusercontent.com/25d07ba4220a3fcadb4af12394d157494ec298dec4ecd86321961427ea18c9e8/68747470733a2f2f63646e2e6a7364656c6976722e6e65742f67682f64657669636f6e732f64657669636f6e2f69636f6e732f7673636f64652f7673636f64652d6f726967696e616c2e737667" height="40px" width="40px">
<img src="https://camo.githubusercontent.com/a7788e074a00b2faa78a3d5d74a643522dcbb5d7267a96a3648f2b772d95702f/68747470733a2f2f63646e2e6a7364656c6976722e6e65742f67682f64657669636f6e732f64657669636f6e2f69636f6e732f616e61636f6e64612f616e61636f6e64612d6f726967696e616c2e737667" height="40px" width="40px">
<img src="https://camo.githubusercontent.com/baf28e1c345391854671f1d2c7d53012b92341cac2bf3e94789ba92c76770d7d/68747470733a2f2f63646e2e6a7364656c6976722e6e65742f67682f64657669636f6e732f64657669636f6e2f69636f6e732f6f70656e63762f6f70656e63762d6f726967696e616c2e737667" height="40px" width="40px">
<div/>

## Demo

https://github.com/Archangel0007/Trajectory-Tracking-System/assets/113388386/5dc8706b-3553-4aea-87bc-1c6184a2370a

You can see in the small demo. The center of every bounding boxes is the current state, the model is trying to predict the center point in the next state.
