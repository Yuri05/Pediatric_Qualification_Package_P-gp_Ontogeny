The presented qualification report evaluates the predictive performance of the OSP suite to predict P-gp related drug transporter activity in children.

Therefore, PBPK models of specific *in vivo* probe substances covering children aged below 6 months up to adolescents were built and evaluated. All models are whole-body PBPK models, allowing for dynamic pediatric translation in organs expressing P-gp. The qualification report demonstrates the level of confidence of the OSP suite with regard to reliable PBPK predictions of age-related P-gp-mediated drug transport during model-informed drug development. The presented PBPK models as well as the respective qualification plan and qualification report are provided open-source and transparently documented ([https://github.com/Open-Systems-Pharmacology/Pediatric_Qualification_Package_P-gp_Ontogeny](https://github.com/Open-Systems-Pharmacology/Pediatric_Qualification_Package_P-gp_Ontogeny)). 


## Translation of Adult PBPK to Children

Using a developed and validated (adult) PBPK model for an *in vivo* probe substance, a pediatric PBPK model can be established for children by translating physiology, clearance processes (as parameterized in the adult model) and age-dependent protein binding including the variability therein.[[Maharaj 2013](#references)] 

The PBPK models are developed with clinical data of healthy adult subjects obtained from the literature, covering available dosing ranges for e.g. intravenous as well as oral administration, to capture both systemic clearance as well as gut-wall metabolic clearance processes. For orally administered drugs, the same formulations that are used in children should ideally be included in the model for adults. Plasma concentrations following multiple dose application, mass balance information and other clinical measurements need to be included for model development, if available. During model translation from adults to children for a specific substance, uncertainties in data-quality caused by impact of disease or the target study population, inaccurate in vitro assay-techniques regarding mass balance, as well as study differences may cause not being able to adequately predict the PK in children for all reported studies. 

Prediction performance of the PBPK model for these probe substances in children are then shown by means of e.g. predicted versus observed clearance (CL) plots, of which the results support an adequate prediction of the ontogeny function for the application of PBPK model translation of adult PBPK to children.

For qualification purpose, during the translation of adult PBPK to children the following assumptions and considerations were made: 

- when translating an adult model to children, it was assumed that the metabolism and excretion pathways are qualitatively the same in children as in adults.
- no further changes to input parameters other than those for the physiology and protein binding were assumed. All other parameters (e.g. lipophilicity, intestinal permeability, solubility) were kept unchanged.

## Anthropometric and Physiological Information 

The age-dependencies of the relevant anthropometric (height, weight) and physiological parameters (e.g. blood flows, organ volumes, binding protein concentrations, hematocrit, cardiac output) in children was gathered from the literature and has been previously summarized [[Edginton 2006](#references)]. The information was incorporated into PK-Sim® and was used as default values for the simulations in children.

The  applied ontogeny and variability of plasma proteins and active processes that are integrated into PK-Sim® for translation to children are described in the publicly available ‘PK-Sim® Ontogeny Database Version 7.3 [[Ontogeny Database](#references)] or otherwise referenced for the specific process.

## **P-gp transporter ontogeny** information

The renal ontogeny of P-gp was published by [[Hunt 2024](#references)]. This ontogeny goes back to transporter expression measurements from human postmortem renal cortical tissue samples [[Cheung 2019](#references)]. The ontogeny of the renal P-gp transporter was applied to all other P-gp expressing organs, mainly, liver and intestine and implemented in PK-Sim in the following way:

| **Post Menstrual Age [yr(s)]**   | **Ontogeny Scaling Factor**    | **GeoSD** |
| :-------------- | ----------- | ----------- |
| 0.1                            | 0                           | 2.903     |
| 0.2                            | 0.001                       | 2.901     |
| 0.3                            | 0.004                       | 2.89      |
| 0.4                            | 0.015                       | 2.857     |
| 0.5                            | 0.04                        | 2.783     |
| 0.6                            | 0.088                       | 2.653     |
| 0.7                            | 0.163                       | 2.472     |
| 0.8                            | 0.264                       | 2.267     |
| 0.9                            | 0.381                       | 2.072     |
| 1                              | 0.499                       | 1.91      |
| 1.1                            | 0.606                       | 1.789     |
| 1.2                            | 0.696                       | 1.702     |
| 1.3                            | 0.767                       | 1.64      |
| 1.4                            | 0.822                       | 1.597     |
| 1.5                            | 0.864                       | 1.567     |
| 1.6                            | 0.895                       | 1.546     |
| 1.7                            | 0.918                       | 1.53      |
| 1.8                            | 0.936                       | 1.519     |
| 1.9                            | 0.949                       | 1.511     |
| 2                              | 0.959                       | 1.504     |
| 2.1                            | 0.967                       | 1.5       |
| 2.2                            | 0.973                       | 1.496     |
| 2.3                            | 0.978                       | 1.493     |
| 2.4                            | 0.982                       | 1.491     |
| 2.5                            | 0.985                       | 1.489     |
| 2.6                            | 0.987                       | 1.487     |
| 2.7                            | 0.989                       | 1.486     |
| 2.8                            | 0.991                       | 1.485     |
| 2.9                            | 0.992                       | 1.484     |
| 3                              | 0.993                       | 1.484     |
| 4                              | 0.998                       | 1.481     |
| 5                              | 0.999                       | 1.48      |
| 10                             | 1                           | 1.48      |




## Qualification of **P-gp transporter ontogeny**

To qualify the OSP suite for the pediatric translation of the pharmacokinetics of drugs that are transported by P-gp, the following probe substance was included:

- Digoxin [[Digoxin-Model](#references)]


The adult PBPK model reports and the corresponding PK-Sim project files are filed at: [https://github.com/Open-Systems-Pharmacology/OSP-PBPK-Model-Library/](https://github.com/Open-Systems-Pharmacology/OSP-PBPK-Model-Library/)

