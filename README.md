# Radial Basis Function Simulator

## Overview
This project implements a **Radial Basis Function (RBF)** simulator using Python. It includes data preprocessing, k-means clustering, RBF transformation, and visualization of decision boundaries, along with a Tkinter-based GUI for user interaction. The project also provides insight into training models using RBF for classification tasks and evaluating their performance through confusion matrices and decision boundary visualizations.

---

## Features

### Core Functionality
1. **K-Means Clustering**
   - Performs clustering on the Iris dataset to determine cluster centers.
   - Visualizes clusters and centroids in a 3D scatter plot.

2. **Radial Basis Function Transformation**
   - Converts input data into a higher-dimensional feature space using RBF.
   - Exponential transformation of Euclidean distances to cluster centers.

3. **Model Training and Prediction**
   - Implements a custom perceptron-based training algorithm for multi-class classification.
   - Evaluates performance using confusion matrices.

4. **Visualization of Decision Boundaries**
   - Plots 2D decision boundaries for the transformed data.

### GUI with Tkinter
- **User Interaction**:
  - Inputs number of RBF centers and standard deviations.
  - Displays and manages data points and basis functions.
- **Visualization**:
  - Displays random points and plots.
  - Shows computed RBF centers.

---

## Dependencies
- Python 3.x
- Required Libraries:
  - `numpy`
  - `matplotlib`
  - `sklearn`
  - `tkinter`

Install dependencies using pip:
```bash
pip install numpy matplotlib scikit-learn
```

---

## How to Run

### 1. Run the Core RBF Simulator
Execute the script containing the RBF model and clustering:
```bash
python rbf_model.py
```
### 2. Launch the Tkinter GUI
Run the GUI script:
```bash
python rbf_gui.py
```
The GUI allows user interaction for visualizing RBF centers and training data.

### 3. Example Workflow
1. Load the Iris dataset.
2. Perform k-means clustering to generate cluster centers.
3. Transform data into higher dimensions using RBF.
4. Train and test the model using perceptron-based learning.
5. Visualize decision boundaries.

---

## File Descriptions

1. **rbf_model.py**
   - Contains the core implementation of RBF transformation, k-means clustering, training, and visualization.
   - Key methods:
     - `train_model(label: int)`: Trains the perceptron for a specific class.
     - `predict_model(test_data: np.ndarray)`: Predicts classes and evaluates performance.
     - `plot_decision_boundaries()`: Visualizes decision boundaries.

2. **rbf_gui.py**
   - Implements the Tkinter-based GUI for interacting with the RBF simulator.
   - Key components:
     - `data_points`: Input field for custom data points.
     - `basis_function`: Displays computed RBF centers.
     - `training_points`: Lists training points in a table.
     - `Parameters`: Accepts number of centers and standard deviation as user input.

---

## Outputs
1. **3D Visualization**:
   - Visualizes clusters and centroids in the feature space.

2. **Decision Boundaries**:
   - Displays 2D decision boundaries for the classifier.

3. **GUI Outputs**:
   - Displays computed centers and visualizes RBF transformations.

---

## Future Enhancements
- Implement support for additional datasets.
- Add options for other clustering algorithms (e.g., DBSCAN, Agglomerative).
- Extend GUI for more visualization options.
- Introduce export functionality for models and data.

---

## Acknowledgments
Special thanks to contributors and references for their open-source implementations and guidance.

---

## License
This project is licensed under the MIT License. Feel free to modify and use it as needed.

