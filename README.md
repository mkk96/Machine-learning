# Machine Learning (Coursera) Exercises

> My solutions to the eight programming exercises from Andrew Ng's Stanford *Machine Learning* course on Coursera, in Octave/MATLAB.

![Octave](https://img.shields.io/badge/GNU%20Octave-0790C0?style=flat-square&logo=octave&logoColor=white)
![MATLAB](https://img.shields.io/badge/MATLAB-compatible-E16737?style=flat-square)
![Coursera](https://img.shields.io/badge/Coursera-Machine%20Learning-0056D2?style=flat-square&logo=coursera&logoColor=white)

## Overview

This repository holds my coursework for the classic Coursera / Stanford **Machine Learning** course by Andrew Ng, which I completed during my B.Tech in Computer Science at Jamia Millia Islamia (2017–2018).

The course provides the scaffolding for each exercise: the driver scripts (`exN.m`), plotting helpers, datasets, the `fmincg` optimiser, the SVM trainer, the Porter stemmer, the `jsonlab` library and the submission scripts. Each exercise asks the student to implement the core algorithm inside the marked `YOUR CODE HERE` sections of specific function files. **Those sections are my work. Everything else is course starter code** written by the course staff, and the exercise handouts (`exN.pdf`) are course material too.

## Exercises

| # | Topic | What I implemented | Folder |
| --- | --- | --- | --- |
| 1 | **Linear regression** | Cost function and gradient descent for one and many variables, feature normalisation, normal equation, data plotting (predicting food-truck profit and house prices) | [`machine-learning-ex1`](machine-learning-ex1/ex1/) |
| 2 | **Logistic regression** | Sigmoid, cost and gradient, regularised cost with polynomial feature mapping, prediction (university admissions and microchip quality-control datasets) | [`machine-learning-ex2`](machine-learning-ex2/ex2/) |
| 3 | **Multi-class classification and neural network prediction** | Vectorised regularised logistic regression, one-vs-all training and prediction, and feed-forward prediction with pre-trained weights on handwritten digits | [`machine-learning-ex3`](machine-learning-ex3/ex3/) |
| 4 | **Neural network learning** | Feed-forward cost with regularisation, backpropagation and the sigmoid gradient, checked against numerical gradients | [`machine-learning-ex4`](machine-learning-ex4/ex4/) |
| 5 | **Regularised linear regression, bias and variance** | Regularised cost and gradient, learning curves, polynomial features and a validation curve for choosing λ | [`machine-learning-ex5`](machine-learning-ex5/ex5/) |
| 6 | **Support vector machines** | Gaussian kernel, a search over *C* and σ on a validation set, and a spam classifier pipeline (email preprocessing, vocabulary lookup, feature vectors) | [`machine-learning-ex6`](machine-learning-ex6/ex6/) |
| 7 | **K-means clustering and PCA** | Closest-centroid assignment, centroid update, random initialisation, image colour compression, PCA projection and reconstruction (including the faces dataset) | [`machine-learning-ex7`](machine-learning-ex7/ex7/) |
| 8 | **Anomaly detection and recommender systems** | Gaussian parameter estimation, F1-based threshold selection, and the collaborative filtering cost and gradient for movie ratings | [`machine-learning-ex8`](machine-learning-ex8/ex8/) |

### Where to look

The files I edited in each exercise:

| Exercise | Files |
| --- | --- |
| ex1 | `warmUpExercise.m`, `plotData.m`, `computeCost.m`, `gradientDescent.m`, `featureNormalize.m`, `computeCostMulti.m`, `gradientDescentMulti.m`, `normalEqn.m` |
| ex2 | `plotData.m`, `sigmoid.m`, `costFunction.m`, `predict.m`, `costFunctionReg.m` |
| ex3 | `lrCostFunction.m`, `oneVsAll.m`, `predictOneVsAll.m`, `predict.m` |
| ex4 | `sigmoidGradient.m`, `nnCostFunction.m` |
| ex5 | `linearRegCostFunction.m`, `learningCurve.m`, `polyFeatures.m`, `validationCurve.m` |
| ex6 | `gaussianKernel.m`, `dataset3Params.m`, `processEmail.m`, `emailFeatures.m` |
| ex7 | `findClosestCentroids.m`, `computeCentroids.m`, `kMeansInitCentroids.m`, `pca.m`, `projectData.m`, `recoverData.m` |
| ex8 | `estimateGaussian.m`, `selectThreshold.m`, `cofiCostFunc.m` |

Some sections are still unfinished: `randInitializeWeights.m` in ex4 is the starter stub, which returns zeros, and the optional house-price predictions in `ex1_multi.m` are still set to `0`.

## How to run

You need [GNU Octave](https://octave.org/) (free) or MATLAB.

```bash
cd machine-learning-ex1/ex1
octave
```

Then, at the Octave/MATLAB prompt, run the driver script for that exercise:

```matlab
ex1          % linear regression, one variable
ex1_multi    % linear regression, multiple variables
```

| Exercise | Driver scripts |
| --- | --- |
| ex1 | `ex1`, `ex1_multi` |
| ex2 | `ex2`, `ex2_reg` |
| ex3 | `ex3`, `ex3_nn` |
| ex4 | `ex4` |
| ex5 | `ex5` |
| ex6 | `ex6`, `ex6_spam` |
| ex7 | `ex7`, `ex7_pca` |
| ex8 | `ex8`, `ex8_cofi` |

Each script works through the exercise in parts, plotting figures and printing results, and pauses between parts (press Enter to continue). The bundled `submit.m` scripts were for grading on the original Coursera platform and you don't need them to run the code.

---

Made by [Mukul Kumar](https://mkk96.github.io) · [GitHub](https://github.com/mkk96) · [LinkedIn](https://www.linkedin.com/in/mukul-kumar-60322616b/)
