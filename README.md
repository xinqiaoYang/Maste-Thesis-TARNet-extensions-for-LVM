# 📖 TARNet - based causal machine learning extensions for latent variable modeling

## 📝 Abstract
This is a repository which stores my master thesis research, including dat (data), doc/fig (figures in the paper), exp (code for simulation study and empirical study). <br>
Estimating individual treatment effects is essential due to variations in treatment
effects across individuals. The research showed a TARNet causal inference extension
of the latent variable modeling framework, namely using the learned representation
or latent construct other than a single outcome variable to infer the individual
treatment effects. This model also reduces estimation variability by addressing
measurement errors. Validation experiments were conducted on 12 simulated
datasets and real-world medication data.

---

## 📂 Repository Structure
The repository is organized as follows:

- [📜 README.md: Project overview and documentation]
- [📂 dat/ :Raw ACTG175 dataset, best model paramters, LFM model fitting parameters saved and factor score saved ]
- [📂 doc/fig : Results in figure format which also appeared in the thesis ]
- [📂 exp/ : Jupyter notebooks conducted with **Python** for experiments of simulation study and empirical study]

---
## 📌 Details
This section provides some details of some documents in the respitory.

- ✅ **dat/model_1.pth, model_2.pth and model_3,pth** – They stored different LFM models fitted with DeepIRTools with iw_samples= 5000, 10000, 8000, respectively for **Step 1** in empirical study.
- ✅ **dat/fs_2.pth** – saved factor scores froom **model_2.pth**, and used this factor store in the end.
- ✅ **exp/Simulation_Study_Updated_1.ipynb**  – experiment 1 for simulation study.
- ✅ **exp/Simulation_Study_Updated_2.ipynb** – experiment 2 which overcomes the TARNet overfitting problem. Same logic as Simulation_Study_Updated_1 except adding the interaction term of **Z** in data generation part, and reducing the number of parameters.
- ✅ **exp/learning_representation.ipynb** – **Step 1** of fitting the model in empirical study.
- ✅ **exp/fixing_tarnet.ipynb** – **Step 2** of fitting the model in empirical study, with hyperparameter tuning. Best model's parameters were saved in **dat/best_model.keras**.
- ✅ **exp/fixing_tarnet_2.ipynb** –  Same logic as **exp/fixing_tarnet.ipynb** except adding the code to make scatter plot of estimated ITE and simulated ITE. This plot was not included in the paper because the simulated ITE from OLS were almost constant, thus it was not a good representation of the estimation. Note that, the estimated ITE could vary a little bit every time you run, but it wouldn't affect the conclusion of the model comparasions in empirical study.

## 🚀 Environment 
Python version is recommended as 3.11.11 or higher. This model is computationally intensive. It is **highly recommended** to use a **GPU** or **TPU** for efficient training. Training on a CPU may take significantly longer.







