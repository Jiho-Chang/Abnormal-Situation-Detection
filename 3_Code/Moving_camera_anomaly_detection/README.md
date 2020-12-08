# Anomaly Detection using Inpainting

The inpainting model used in our approach is extended using an autoencoder. The network takes an input with a cut-out center area and attempts to reconstruct the missing region [1]. The usage of this model for anomaly detection is explored in this paper [2].

[1] Pathak, Deepak, Philipp Krahenbuhl, Jeff Donahue, Trevor Darrell, and Alexei A. Efros. "Context encoders: Feature learning by inpainting." In Proceedings of the IEEE conference on computer vision and pattern recognition, pp. 2536-2544. 2016.

[2] Zaheer, Muhammad Zaigham, Marcella Astrid, Seung-Ik Lee, and Ho Chul Shin. "Ensemble grid formation to detect potential anomalous regions using context encoders." In 2018 18th International Conference on Control, Automation and Systems (ICCAS), pp. 661-665. IEEE, 2018.

### Description
![PedAbnormal](./ped_ab_description.jpg)

model_anomaly: The anomaly detection model is defined here. The model is trained based one-class classification scheme, built on top of an autoencoder architecture. Later, abnormal situations are detected through the thresholding of reconstruction errors.

ped_node: Modules for communication between the anomaly detection module and the server. Receives monitoring image and bounding box information and sends abnormal scores to the server.

### Requirements
- ROS-Kinetic
- Python==3.5.3
- Tensorflow==2.2.0
- numpy==1.16.1
- matplotlib==2.2.2
- scikit-learn==0.20.2
- tqdm==4.41.1
- Opencv-python==3.4.0.12

### Dataset
- Models are trained with our specific dataset. Please contact us.

### Contributor
* [✉️](mailto:jh_lee@etri.re.kr) __이진하__ (in Ha, Lee)
#
![](https://www.etri.re.kr/images/kor/sub5/signature08.png)
