# Hack-O-Uplift
Breast Cancer Detection
Breast cancer is a type of cancer that forms in the cells of the breasts.
Symptoms of breast cancer include a lump in the breast, bloody discharge from the nipple and changes in the shape or texture of the nipple or breast<br>
Breast cancer most often begins with cells in the milk-producing ducts.
The tumor formed may be malignant or benign. Early detection of malignant tumors can be live saving. <br>
We have a dataset of images of breast tumors of varying magnification.
We use computer vision to identify whether a tumor is malignant or benign, hence finding the likelihood of cancer developing.<br>
Our objective is to train the machine to help identify the tumor with a reasonable level of accuracy. We are using CNNs to achieve so. 
It could be helpful for oncologists in the future, as it could act as a second opinion which is always advantageous.The machine helps you detect tumors faster, and also helps us bypass human error. Also, it could be helpful in detection breast cancer in populations where cancer awareness is low, like in rural areas with lesser access to medical services. <br>
-Libraries used: OpenCV, TensorFlow, SciKit, Numpy, Pandas, MatPlotlib etc.<br>
-Dataset from: https://web.inf.ufpr.br/vri/databases/breast-cancer-histopathological-database-breakhis Breast Cancer Histopathological Database (BreakHis) <br>
-YouTube Video link: <br>
About the CNN model:

Model: "sequential_1"
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
_________________________________________________________________
densenet201 (Functional)     (None, 7, 7, 1920)        18321984  
_________________________________________________________________
global_average_pooling2d_1 ( (None, 1920)              0         
_________________________________________________________________
dropout_1 (Dropout)          (None, 1920)              0         
_________________________________________________________________
batch_normalization_1 (Batch (None, 1920)              7680      
_________________________________________________________________
dense_1 (Dense)              (None, 2)                 3842      
_________________________________________________________________
Total params: 18,333,506
Trainable params: 18,100,610
Non-trainable params: 232,896
_________________________________________________________________

-Model: Densenet201 <br>
-Optimizer: Adam <br>
-Activation: Softmax <br>
-Accuracy: Around 95% <br>
![2021-09-05 (2)](https://user-images.githubusercontent.com/79798013/132110171-64799982-e089-488c-9181-2e9502376d79.png)


