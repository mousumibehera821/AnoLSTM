# AnoLSTM
AnoLSTM-A Deep Learning Approach for Test Cases Prioritization


# Abstract
In a continuous integration environment, code is often merged into the mainline codebase. As a result, regression testing is essential for ensuring that modifications to the primary codebase do not adversely affect the performance of the software's current characteristics. Test case prioritization (TCP) is a regression-based approach for reordering test cases in a test suite to enhance fault detection performance and shorten test case execution time. In this study, we put forward the AnoLSTM-TCP (Anomaly-Based Long Short-Term Memory Test Case Prioritisation) method to prioritize test cases. Our strategy leverages historical test case data, including features such as duration, execution of the test cases, and list of previous test results to automatically learn patterns and prioritize test cases effectively. Our proposed method goal is to increase the rate at which faults are discovered in test cases. For our experiment, we use an industrial dataset from ABB Robotics Norway (IOFROL and Paint Control). The evaluation metric we used to analyze the effectiveness of our model is APFD values. We compare our novel work with previous works of Random, ROCKET, RETECS, Deepgini, DeepOrder, and HyLSTMTCP. Finally, our experimental results show that AnoLSTM-TCP significantly achieves higher APFD values of 0.85, and 0.90 on IOFROL, and Paint Control datasets which are higher than existing approaches.

Experiments were conducted on two industrial datasets from ABB Robotics Norway:

| Dataset | 
|----------|
| IOF/ROL | 
| Paint Control | 

The proposed approach achieved APFD scores of:

| Dataset | APFD |
|----------|------|
| IOF/ROL | 0.85 |
| Paint Control | 0.90 |

These results outperform several existing approaches, including Random, ROCKET, RETECS, DeepGini, DeepOrder, LSTMTCP, and HyLSTMTCP.

# Datasets
The datasets used in this work are publicly available at: 

https://bitbucket.org/HelgeS/retecs/src/master/DATA/

# Repository Structure

AnoLSTM-TCP 
│ 
├── final_iofrol.py 
├── final_paint_control.py 
├── requirements.txt 
├── README.md 

# Running the Code

# Install Dependencies
 pip install -r requirements.txt

# Running the Experiments

# IOF/ROL Dataset

python final_iofrol.py

# Paint Control Dataset

python final_paint_control.py

## Paper
Published in Procedia Computer Science (2025)
DOI: https://doi.org/10.1016/j.procs.2025.04.431

# Citation
If you use this work, please cite:
@article{choudhury2025anolstm,
  title={AnoLSTM-A deep learning approach for test cases prioritization},
  author={Choudhury, Tapas Kumar and Behera, Mousumi and Dash, Sanjit Kumar and Pani, Subhendu Kumar and Mishra, Jibitesh},
  journal={Procedia Computer Science},
  volume={258},
  pages={1793--1803},
  year={2025},
  publisher={Elsevier}
}
