# AnoLSTM-TCP
AnoLSTM-A Deep Learning Approach for Test Cases Prioritization


# Abstract
In a continuous integration environment, code is often merged into the mainline codebase. As a result, regression testing is essential for ensuring that modifications to the primary codebase do not adversely affect the performance of the software's current characteristics. Test case prioritization (TCP) is a regression-based approach for reordering test cases in a test suite to enhance fault detection performance and shorten test case execution time. In this study, we put forward the AnoLSTM-TCP (Anomaly-Based Long Short-Term Memory Test Case Prioritisation) method to prioritize test cases. Our strategy leverages historical test case data, including features such as duration, execution of the test cases, and list of previous test results to automatically learn patterns and prioritize test cases effectively. Our proposed method goal is to increase the rate at which faults are discovered in test cases. For our experiment, we use an industrial dataset from ABB Robotics Norway (IOFROL and Paint Control). The evaluation metric we used to analyze the effectiveness of our model is APFD values. We compare our novel work with previous works of Random, ROCKET, RETECS, Deepgini, DeepOrder, and HyLSTMTCP. Finally, our experimental results show that AnoLSTM-TCP significantly achieves higher APFD values of 0.85, and 0.90 on IOFROL, and Paint Control datasets which are higher than existing approaches.

# Datasets
https://bitbucket.org/HelgeS/retecs/src/master/DATA/

# Repository Structure

AnoLSTM-TCP 
│ 
├── final_iofrol.py 
├── final_paint_control.py 
├── requirements.txt 
├── README.md 
└── datasets/

# Running the Code

# Install Dependencies
 pip install -r requirements.txt
 
# Run IOF/ROL Experiment
python final_iofrol.py

# Run Paint Control Experiment
python final_paint_control.py

# Citation
If you use this work, please cite:

