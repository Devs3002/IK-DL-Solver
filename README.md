# Inverse Kinematics Calculation Using Deep Learning

This project aims to find the inverse kinematics solution for a PUMA560 robotic arm using a deep neural network (DNN) trained with vanilla flavoring. While a closed-form solution already exists for the PUMA-560, we explore the use of DNNs to demonstrate that they can be employed to find the inverse kinematic solution for a robotic arm.

## Dataset and Code Structure

This repository consists of two sets of codes:

1. **Data Generation using Conventional Methods**: This section includes a MATLAB code that computes the inverse solution for a 6R robot using the piper solution for inverse kinematics. The code writes the generated data into a CSV file. Please note that the solutions provided by the MATLAB code can be singular, and if no inverse kinematic solution exists, it will not be added to the CSV file. The data generated using this code will be used to train the DNN model.

2. **Data Generation using Forward Kinematics with Joint Restraints**: This section contains code for generating data using forward kinematics with joint restraints. 

## Usage

To use this project, follow the steps below:

1. Clone the repository:

```bash
git clone https://github.com/Devs3002/IK-DL-Solver.git
```

2. Navigate to the project directory


3. Set up the dataset:

   - Run the MATLAB code (`iPUMA.m`) to generate the inverse kinematics data using conventional methods.
   - Provide additional instructions if necessary for the data generation using forward kinematics with joint restraints.

4. Train the DNN model:

   - Specify the location of the generated CSV file in the DNN training code (`train.py` or any relevant file).
   - Describe any dependencies or configurations required for training the DNN model.
   - Provide instructions on how to run the training code and any relevant parameters that can be adjusted.

5. Evaluate and test the trained model:

   - Explain the process of evaluating the trained DNN model, including any metrics used for assessment.
   - Provide instructions for testing the model on new data or specific use cases, if applicable.

## Contributing

Contributions to this project are welcome! If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request. Describe the problem or enhancement you'd like to address, and we'll review it together.


## Acknowledgments

- Dr. Ekta Singla from IIT Ropar for assigning this project as a course project.
- Thanh Q. Nguyen1, Khien B. Pham2, Duong Thi Kim Chi3 for their research paper "Modeling Robotic Arm with Six-Degree-of-Freedom Through Forward Kinematics Calculation Based on Deep Learning," which served as an inspiration for this project.
- Advait Chandorkar, my teammate, for assisting with the code development.

