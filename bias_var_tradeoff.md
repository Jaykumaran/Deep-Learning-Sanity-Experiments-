Ideal: low bias, low variance for better generalization.

<img src ="https://learnopencv.com/wp-content/uploads/2017/02/Bias-Variance-Tradeoff-In-Machine-Learning-1.png">


| **Issue**     | **Symptoms**                                              | **Potential Fixes**                                                                 |
|---------------|-----------------------------------------------------------|--------------------------------------------------------------------------------------|
| **High Bias** | Underfitting: training error is high                      | - Add more layers                                                                    |
|               |                                                           | - Add more features                                                                  |
|               |                                                           | - Train longer                                                                       |
|               |                                                           | - Try a more complex model (new architecture) if nothing else works                 |
|               |                                                           | **Note:** More data typically doesn't help                                           |
| **High Var**  | Overfitting: large gap between training and validation loss | - Reduce number of features                                                          |
|               |                                                           | - Add more training data                                                             |
|               |                                                           | - Use early stopping                                                                 |
|               |                                                           | - Reduce model complexity (fewer layers/parameters)                                  |
|               |                                                           | - Apply regularization (L1, L2, dropout, etc.)                                       |


Good explanation: https://www.appliedaicourse.com/blog/bias-and-variance-in-machine-learning/
