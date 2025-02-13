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
- [📂 exp/ : Jupyter notebooks conducted with Python for experiments of simulation study and empirical study]

---
## 📌 Details
This section provides some details of each document in the respitory.

- ✅ **dat/model_1.pth, model_2.pth and model_3,pth** – They stored different LFM models fitted with DeepIRTools with iw_samples= 5000, 10000, 8000, respectively for Step 1 in empirical study.
- ✅ **dat/fs_2.pth** – saved factor scores froom model_2, and used this factor store in the end.
- ✅ **doc/fig** – 
- ✅ **Visualization Tools** – Built-in support for graphs and analytics.
- ✅ **Customizable Configuration** – Config files allow easy tuning of parameters.







