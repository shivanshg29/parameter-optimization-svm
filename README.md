# SVM Parameter Optimization using Random Search (Iris Dataset)

This project implements a simple **random search algorithm** to optimize the hyperparameters of a **Support Vector Machine (SVM)** for classifying the UCI Iris dataset. The goal is to **maximize accuracy** by tuning the following parameters:

## 🔧 Parameters Optimized
- **nu**: Random float in [0, 1]
- **epsilon**: Random float in [0, 1]
- **kernel**: Random selection from ['rbfdot', 'polydot', 'vanilladot', 'tanhdot', 'laplacedot', 'anovadot']

## 🧠 Algorithm Flow :
1. Initialize `BestFitness = 0`, `BestParameter = None`
2. Generate random parameters
3. Train SVM and compute fitness (accuracy)
4. If accuracy > BestFitness, update BestFitness and BestParameter
5. Repeat until stopping condition (e.g. max iterations)
6. Return best parameters and accuracy

## 📈 Output
- Best parameter set found
- Corresponding accuracy
- Accuracy graph saved as PNG
- Result table saved as CSV

## 🖼️ Graph
![Accuracy Plot](./svm_iris_classification_convergence.png)
