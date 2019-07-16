# Overview
A collection of submitted material for the 2019 MR Data Challenge. The 2019 MR Data Challenge is a session presented at the 2019 Mendelian Randomization Conference, held at the University of Bristol. For more information on the conference, please visit the MR conference [website](https://www.mendelianrandomization.org.uk/).

The report accompanying each project is available [here](https://github.com/WSpiller/MRChallenge-Projects/tree/master/Projects).

---

## 1. The role of lipoprotein subfractions in coronary artery disease

*Qingyuan Zhao<sup>1</sup>, Jingshu Wang<sup>1</sup>, Zhen Miao<sup>2</sup>, Nancy Zhang<sup>1</sup>, Sean Hennessy<sup>2</sup>, Dylan Small<sup>1</sup>, and Dan Rader<sup>2</sup>*

<sup>1</sup>Department of Statistics, Wharton School, University of Pennsylvania

<sup>2</sup>Perelman School of Medicine, University of Pennsylvania

### Project Summary

Earlier MR studies (Voight et al. 2012; Zhao, Chen, et al. 2019) found evidence of heterogeneity for the
effect of HDL cholesterol on coronary artery disease (CAD). In this report, the research question we aim to
explore is:

**Do lipoprotein subfractions have heterogeneous effects on CAD?**

To answer this question, we will conduct a MR screening study that estimates the causal effect of each
subfraction on CAD. Some highlighting features of our analysis include:

• Genome-wide three-sample design: This design allows us to utilize insturments that are only
weakly correlated with the subfraction trait (may not be genome-wide significant). This is crucial
because usually only a handful of genetic variants have genome-wide significant association with
subfraction traits.

• State-of-the-art statistical method: We used Robust Adjusted Profile Score (RAPS) which is not
biased by individually weak instruments, as long as the overall instrument strength is not weak. RAPS
is also robust to balanced and/or sparse pleiotropy; in particular, RAPS is asymptotically unbiased if
the InSIDE (INstrument Strength Independent of Direct Effect) assumption is satisfied.

• Multivariate MR: We applied a novel extension of RAPS to multivariate exposures. This allows us
to assess whether the (potential) effect of any lipoprotein subfraction is independent of the major lipid
traits (HDL-C, LDL-C, TG).

---

## 2. Testing instrument strength in two-sample MVMR estimation of lipid traits on AMD and Type 2 diabetes.

*Eleanor Sanderson<sup>1</sup>, and  Jack Bowden<sup>1</sup>*

<sup>1</sup>MRC Integrative Epidemiology Unit, Univerity of Bristol.

### Project Summary

One of the key assumptions of any Mendelian randomisation (MR) analysis is that the exposures are strongly
predicted by the set of SNPs used as instruments. In multivariable MR (MVMR) this assumption requires
that each exposure is strongly predicted by the SNPs included conditional on the predicted value of the
other exposures in the model. Many of the traits considered in the NMR data here are associated with
highly overlapping groups of SNPs and therefore it is particuarly important with data of this type to consider
whether these exposures can be reliably predicted by the set of SNPs if multiple traits from this data are
going to be included as exposures in an MVMR analysis.

Here I consider whether multiple traits in this dataset can be predicted at the same time. If a group of
exposures can all be strongly predicted by the set of SNPs then, assuming the other instrumental variable
assumptions are satisfied, it will be possible to estimate the direct effect of each exposure on an outcome.
However, if some or all of the exposures are weakly predicted then any MR analysis including those exposures
will be subject to weak instrument bias.

---

## 3. Mendelian Randomization Analysis of the Effect of Blood Lipid Fractions on the Risk of Type 2 Diabetes.

*Apostolos Gkatzionis<sup>1</sup>

<sup>1</sup>MRC Biostatistics Unit, University of Cambridge

### Project Summary

The aim of this analysis is to assess the causal effects of three blood lipid fractions (LDLcholesterol, HDL-cholesterol and triglycerides) on the risk of suffering from type 2 diabetes. In parallel to that, we illustrate the use of the JAM-MR algorithm, a recentlyproposed algorithm for pleiotropy-robust Mendelian randomization using summary data.

---


## 4. Mendelian Randomization Analysis of the Effect of Blood Lipid Fractions on the Risk of Type 2 Diabetes.

*Apostolos Gkatzionis<sup>1</sup>

<sup>1</sup>MRC Biostatistics Unit, University of Cambridge

### Project Summary

The aim of this analysis is to assess the causal effects of three blood lipid fractions (LDLcholesterol, HDL-cholesterol and triglycerides) on the risk of suffering from type 2 diabetes. In parallel to that, we illustrate the use of the JAM-MR algorithm, a recentlyproposed algorithm for pleiotropy-robust Mendelian randomization using summary data.

---














