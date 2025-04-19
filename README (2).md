# SVM Optimization Experiment

## Overview
This repository contains an implementation of a Support Vector Machine (SVM) optimization experiment for multi-class classification. The experiment uses a synthetic dataset to evaluate SVM performance across multiple samples with different parameters.

## Features
- Generation of synthetic multi-class dataset with 10000 samples and 10 features
- Automated SVM hyperparameter optimization
- Multiple sample evaluation (10 different train/test splits)
- Comprehensive visualization of results
- Detailed performance metrics and convergence analysis

## Dataset
The experiment uses a synthetic dataset with the following properties:
- 10000 samples
- 10 features (8 informative, 4 redundant)
- 8 classes with equal distribution
- Standardized preprocessing

## Methodology
1. A synthetic multi-class dataset is generated using scikit-learn's `make_classification`
2. Basic exploratory data analysis is performed (class distribution, feature statistics, correlations)
3. The dataset is split into 10 different train/test samples (70%/30% split)
4. For each sample, SVM optimization is performed with various kernel configurations:
   - Linear kernel with different C values (0.1, 1.0, 10.0)
   - RBF kernel with different C values and gamma parameters
5. Accuracy is tracked across iterations to generate convergence history
6. Results are compiled and visualized

## Visualizations
The experiment generates several visualizations:
- Convergence graph for the best-performing SVM
- Class distribution visualization
- Feature correlation heatmap

## Dependencies
- Python 3.x
- NumPy
- pandas
- scikit-learn
- Matplotlib
- seaborn

## Usage
```python
# Clone the repository
git clone https://github.com/yourusername/svm-optimization-experiment.git
cd svm-optimization-experiment

# Install dependencies
pip install -r requirements.txt

# Run the experiment
python svm_experiment.py
```

## Output Files
- `svm_optimization_results.csv`: Complete results table
- `best_svm_convergence.png`: Convergence graph for the best SVM
- `class_distribution.png`: Visualization of class distribution
- `feature_correlation.png`: Heatmap of feature correlations

## License
[MIT License](LICENSE)

## Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

Collab link for this :- https://colab.research.google.com/drive/1_ycr3S5dT6RMvMCfM7SAyv3t7ODDywtf?usp=sharing
