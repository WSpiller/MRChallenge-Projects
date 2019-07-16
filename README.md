# Overview
A collection of submitted material for the 2019 MR Data Challenge. The 2019 MR Data Challenge is a session presented at the 2019 Mendelian Randomization Conference, held at the University of Bristol. For more information on the conference, please visit the MR conference [website](https://www.mendelianrandomization.org.uk/).

The report accompanying each project is available for download [here](https://github.com/WSpiller/MRChallenge-Projects/tree/master/Projects).

**A plenary session at 11:00 AM on Friday 19th July in lecture theatre 1 of the the Chemistry Complex at the University of Bristol, showcasing the submitted analyses.**

A key aim of the session will be to bring together methodologists and statisticians with experts from epidemiology, medical and biological sciences, to comment and debate the results. The session will include presentations from subject matter experts on state-of-the-art lipids research; an overview of all analyses attempted at a meta-level; quickfire presentations from individuals and teams on their analysis; debate on the strengths and limitations of different methodological approaches.

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

*Apostolos Gkatzionis<sup>1</sup>*

<sup>1</sup>MRC Biostatistics Unit, University of Cambridge

### Project Summary

The aim of this analysis is to assess the causal effects of three blood lipid fractions (LDLcholesterol, HDL-cholesterol and triglycerides) on the risk of suffering from type 2 diabetes. In parallel to that, we illustrate the use of the JAM-MR algorithm, a recentlyproposed algorithm for pleiotropy-robust Mendelian randomization using summary data.

---

## 4. HDL and age-related macular degeneration

*Chin Yang Shapland<sup>1</sup>*

<sup>1</sup>MRC Integrative Epidemiology Unit, Univerity of Bristol.

### Project Summary

Age-related macular degeneration (AMD) is a painless eye-disease that eventually leads to vision loss. A
GWAS have identified several rare and common variants located in gene regions that are associated with lipid
levels (Fritsche et al. 2016). And later the reason for association was speculated and confirmed by separate
studies (Leeuwen et al. 2018, J. Colijn et al. (2018)). Multivariable MR study showed evidence of a causal
relationship between AMD and HDL cholesterol but not with LDL cholesterol and triglycerides (Burgess and
Smith 2017). Following a Bayesian model averaging approach within a multivariable MR design, out of 30
metabolites, total cholesterol in extra-large HDL particles (XL.HDL.C) had the highest inclusion posterior
probability as a risk factor for AMD (Zuber et al. 2019). With the same summary data used in (Zuber et al.
2019), we aim to find valid genetic instruments to infer causality between XL.HDL.C and AMD.

---

## 5. Improving reliability of MR studies testing the effect of molecular phenotypes

*Maria Carolina Borges<sup>1</sup><sup>2</sup>, Philip Haycock<sup>1</sup><sup>2</sup>, Aroon Hingorani<sup>3</sup><sup>4</sup>, and Deborah Lawlor<sup>1</sup><sup>2</sup>*

<sup>1</sup>MRC Integrative Epidemiology Unit, Univerity of Bristol.

<sup>2</sup>Population Health Sciences, Bristol Medical School, University of Bristol, Bristol, UK

<sup>3</sup>UCL Institute of Cardiovascular Science, University College London, London, UK

<sup>4</sup>MRC Farr Institute, University College London, London, UK

### Project Summary

One major limitation of Mendelian randomization (MR) is the unprovable assumption that the association between genetic instrument and outcome is entirely mediated by the exposure and not by direct effects of the genetic instrument. A large proportion of recently developed methods aim at accounting for spurious pleiotropy to improve the reliability of MR results. However, these methods ideally require that many genetic instruments for the exposure are available, which is often not the case when the exposure is a molecular phenotype.

In the context of MR, spurious pleiotropy can arise from three main scenarios:

* **Counfounding by linkage disequilibrium**: the genetic instrument influences the exposure and is correlated (i.e. in linkage disequilibrium) with another genetic variant that influences the outcome independently.

* **Reverse causation**: the genetic instrument primarily influences the outcome, which subsequently affects the exposure.)

* **Horizontal pleiotropy**: the genetic instrument influences exposure and outcome via two independent biological pathways.

We propose a framework combining methods developed within and outside the MR community to explore robustness of MR findings to spurious pleiotropy when only one or a few genetic instruments are available for a particular exposure.

---

## 6. Investigating the Causal Effect of LDL and HDL on Ischemic Stroke

*Okezie Uche-Ikonne<sup>1</sup>, Michael Holmes<sup>2</sup>, Frank Dondelinger<sup>3</sup>, and Tom Palmer<sup>1</sup>*

<sup>1</sup> Department of Mathematics and Statistics, Lancaster University, Lancaster, UK

<sup>2</sup> Medical Research Council Population Health Research Unit, University of Oxford, Oxford, UK

<sup>3</sup> Faculty of Health and Medicine, Lancaster University, Lancaster, UK

### Project Summary

There has been considerable research on the role of blood lipids and their associations with various cardiovascular traits (Holmes and Davey Smith 2018). While observational analyses have led to naïve classifications of “good” (higher density lipoprotein, HDL) and “bad” (lower density lipoprotein, LDL) blood lipids, the underlying causal relationships suggest that while LDL and triglycerides may have atherogenic characteristics, HDL-cholesterol is unlikely to play an important role in atherogenesis.

The MR Data Challenge provides a summary level dataset by which contains the associations of genotypes (comprising 148 SNPs) with lipid traits and the associations of genotypes with 7 outcomes (W. Spiller, Bowden, and Zuber 2019). Of the seven outcomes, we selected ischemic stroke to investigate the casual relationship of LDL and HDL lipid traits using the Mendelian randomization (MR) approach (Davey Smith and Ibrahim 2003).

---

## 7. Examining heterogeneity in effect estimates of HDL-C upon CAD and potential biological mechanisms

*Daniel Long<sup>1</sup>, and Qingyuan Zhao<sup>2</sup>*

<sup>1</sup>University of Michigan Department of Statistics

<sup>2</sup>Department of Statistics, Wharton School, University of Pennsylvania

### Project Summary

HDL are heterogeneous subpopulations of discrete particles that differ in apolipoprotein and lipid composition. Previous Mendelian randomization (MR) studies reported heterogeneous associations between genetically determined HDL cholesterol (HDL-C) and coronary artery disease (CAD) (Voight et al. 2012; Zhao et al. 2018). Our research questions are:

* Which groups of genetic instruments yield similiar causal effect estimates of HDL-C on risk for CAD?

* Can these groups be linked to distinct biological mechanisms using GWAS data for the lipoprotein subfractions?

---










