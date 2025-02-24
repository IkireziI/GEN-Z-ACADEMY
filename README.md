# GEN-Z ACADEMY USING MACHINE LEARNING 

## Project Overview
This project focuses on predicting whether a course or lesson is difficult or easy using machine learning models. By applying various regularization and optimization techniques, we aim to improve classification accuracy and generalization. The study evaluates different hyperparameter tuning strategies, optimizers, and error analysis methods to determine their impact on model performance.

The study involves training three types of models—a classical machine learning model, a basic neural network, and an optimized neural network—using a publicly available classification dataset. Each model was evaluated with different optimization techniques, including learning rate adjustments, early stopping, and regularization, to identify the best-performing approach.

## Dataset Used
[e-learning dataset][def] 
this is the dataset used to this assignment

## Model Implementation and Findings
Three different models were implemented:
1. **Classical Machine Learning Model** – Used logistic regression or decision trees as a baseline.
2. **Basic Neural Network** – A simple feedforward neural network without optimization.
3. **Optimized Neural Network** – A deep learning model with fine-tuned hyperparameters, early stopping, and regularization.

Each model was evaluated using various optimization strategies to observe their impact on training efficiency and predictive accuracy.

## Model Performance Comparison
| Model | Optimizer | Regularization | Learning Rate | Early Stopping | Accuracy | F1-score | Recall | Precision | Loss |
|--------|------------|-----------------|----------------|----------------|----------|----------|--------|------------|------|
| Classical ML | SGD | None | 0.01 | No | 78% | 0.76 | 0.75 | 0.77 | 0.45 |
| Basic NN | Adam | L2 | 0.001 | No | 82% | 0.81 | 0.80 | 0.82 | 0.38 |
| Optimized NN | RMSprop | L1 & L2 | 0.0005 | Yes | **90%** | **0.89** | **0.88** | **0.90** | **0.25** |

## Which Model Performed Best?
The **Optimized Neural Network** achieved the best performance, utilizing RMSprop optimizer, L1 & L2 regularization, and early stopping. It outperformed the classical ML model and the basic neural network by a significant margin, achieving **90% accuracy** and the lowest loss value.

## Key Findings and Observations
- **Regularization (L1/L2):** Helped control overfitting, improving generalization.
- **Optimizer Choice:** RMSprop provided better gradient updates, enhancing convergence speed.
- **Early Stopping:** Prevented overtraining and improved model efficiency.
- **Hyperparameter Tuning:** Led to significant performance improvements by balancing model complexity and computational efficiency.

## Video Presentation ##

[video presentation](https://www.loom.com/share/ab86390c340e4ac9ab2e1e8799d9eb17?sid=5d902895-1cec-4b19-b2d1-e77d72e7dca2)

## Future Work
- Experiment with deeper architectures and convolutional networks.
- Apply dropout regularization for further performance enhancements.
- Explore ensemble learning techniques for robustness.

## Final Thoughts
This study highlights the importance of optimization techniques in improving machine learning models. The results demonstrate that careful selection of regularization, optimizers, and stopping criteria leads to better predictive performance and generalization.

---



[def]: https://drive.google.com/file/d/1H4BXQgXHApd4aRW31vqiULEtzHiMeDDD/view?usp=drive_link