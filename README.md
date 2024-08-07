# (WIP) Reliable IA

## Table of Contents
- [(WIP) Reliable IA](#wip-reliable-ia)
	- [Table of Contents](#table-of-contents)
	- [Contributing](#contributing)
- [Introduction : why](#introduction--why)
- [Scientific Themes](#scientific-themes)
	- [Transparency](#transparency)
	- [Ethics](#ethics)
	- [Robutness](#robutness)
	- [Environment](#environment)
	- [Reproducibility](#reproducibility)
- [Platform :](#platform-)
- [Stategic Themes](#stategic-themes)
	- [Human-Centered: "Contrôle Humain"](#human-centered-contrôle-humain)
	- [Responsability](#responsability)
	- [Privacy](#privacy)

## Contributing
Please feel free to send me [pull requests](https://github.com/data-corentinv/awesome-reliable-ai/pulls) or email (vasseur.corentin@gmail.com) to add links.

# Introduction : why

Notes : 
* Responsable vs Irresponsable (= ne pas avoir conséquence de ses actes)
* Responsible AI : 6 keys (Human-Centered ML, Secure, Interpretable IA, Explainable, Ethics, Compliance)

* A LIRE: 
    - https://betaandbit.github.io/RML/#p=1
	- []: https://www.datanami.com/2020/04/06/brief-perspective-on-key-terms-and-ideas-in-responsible-ai/
	Thrustworthy/Reliable AI : 7 keys Scientific (Human-Centered ML, Robustness,  Ethics, Environmental, Transparency,) & Strategic (Privacy & Data Gouv, Tracking & Reproducible operations)
	- []: https://www.emedgene.com/7-keys-to-a-trustworthy-ai-according-to-the-eu-guidelines/
	- https://docs.google.com/presentation/d/1Md24K25opDU9lb5llop8i_vYs1aLvryW9iemF1y6gAU/edit#slide=id.p33
	- CausualML Challenge: https://neurips.cc/Conferences/2022/CompetitionTrack


* Ex. AI fails : 
	- Understand how it works ? « Ballon foot »,  « Barbe masque détection »
	- Impact société dû biais : Recrutement, COMPAS, etc. 
	- AutoML - performance basée sur des métriques techniques (eg. accuracy) et non business (e.g. recrutement)

* Législation : 
	- Avant sur la Data : RGPD (2016)
	- Maintient sur l’IA : Thrustworthy IA, DI US
	- Guide Pratique : https://www.afjv.com/news/10981_guide-pratique-nouveau-reglement-ia.htm
	- OECD: https://oecd.ai/en/accountability

* Responsible ML : 
	- https://info.h2o.ai/rs/644-PKX-778/images/OReilly_Responsible_ML_eBook.pdf

* CNIL 
  - https://www.cnil.fr/fr/intelligence-artificielle/guide

# Scientific Themes
- Monitoring

Model observability 
- https://arize.com/ml-observability/
- https://neptune.ai/blog/ml-model-monitoring-best-tools
- https://towardsdatascience.com/ml-infrastructure-tools-ml-observability-8e4d7df6db43
- https://towardsdatascience.com/what-is-ml-observability-29e85e701688
- https://medium.com/arize-ai/ml-infrastructure-tools-ml-observability-4b74d05a5fd6
- https://www.montecarlodata.com/blog-beyond-monitoring-the-rise-of-observability/


- Alerting 


## Transparency

- Methodology
- Explainability
- Interpretable IA

Questions: 
- How does each features contribute to a model's prediction?
- How does a prediction change dependent on feature inputs?
- What features are or not are significant for a given outcome?
- What features would you change to obtain a different prediction?
- How robust is the model?

Tools: 
- https://github.com/SelfExplainML/PiML-Toolbox
- https://github.com/g8a9/ferret
- [explainerdashboard](https://github.com/oegedijk/explainerdashboard)

Shap: Patrick Hall
- https://maven.com/p/d3409b/understand-shap-s-hapley-additive-ex-planations

A Selection of Medium articles : 
- https://pub.towardsai.net/shapash-making-ml-models-understandable-by-everyone-8f96ad469eb3
- https://www.marktechpost.com/2022/02/10/uc-berkeley-researchers-introduce-imodels-a-python-package-for-fitting-interpretable-machine-learning-models/
- LimeCraft: https://arxiv.org/pdf/2111.08094.pdf
- Xplique: https://github.com/deel-ai/xplique


* Shap (Shapley Additive exPlanations) : Shap is a model agnostic and works by breaking down the contribution of each feature and attributing a score to each feature.
* LIME (local Interpretable Model-agnostic Explanations) : LIME is another model agnostic method that works by approximinating the behavior of the model locally around a specific prediction.
* Eli5 : library for debugging and explaining classifiers. It provides feature importance scores, as well as "reason codes" for scikit-learn, Keras, Xgboost, LightGBM, CatBoost
* Shapash : python library which aims to make machine learning interpretable and understandable to everyone. Shapash provides several types of visualization with explicit labels.
* Anchors : method for generating humain-interpretable rules that can be used to explain the predictions of a machine learning model.
* XAI (eXplainable AI): XAI is a library for explaining and visualizeing the predictions of machine learning models including feature importance scores, decision trees, and rule-based explanations.
* BreakDown : tool that can be used to explain the predictions of linear models. It works by decomposing the model's output into the contribution of each input feature.
* Interpret-text: interpret-text is a library for explaining the predictions of natural language processing models.
* iml (Interpretable MAchine Learning): iml currently contains the interface and IO code from the Shap project and it will potentially also do the same for the Lime project.
* aix360 (AI Explainibility 360): aix360 includes a comprehensive set of algorithms that cover different dimensions.
* OmnniXAI (short for Omni eXplainable AI), adresses several problems with interpreting judgements produced by machine learning models in practice.
* Seldon (alibi explain / detect):
  * https://www.seldon.io/solutions/open-source-projects/alibi-explain
  * https://www.seldon.io/solutions/open-source-projects/alibi-detect
 
* Source: https://www.linkedin.com/posts/maryammiradi_ai-explainability-beyond-the-surface-uncommon-activity-7212004104263380993-qmcn/?utm_source=share&utm_medium=member_ios

## Ethics
- https://gendered-news.imag.fr/genderednews/
- Methodology
- Lesson : 
  - https://ethics.fast.ai/
  - https://ethical.institute/index.html
- https://www.youtube.com/watch?v=0Q4wU2dyMbI&t=161s
- https://github.com/dssg/aequitas
- Bais: 
	* https://causalnex.readthedocs.io/en/latest/03_tutorial/04_sklearn_tutorial.html#Dataset-bias-evaluation
	* Comment mesurer les biais dans les données ? https://www.youtube.com/watch?v=2df7doSlUwA
- Identifying and managing bias in AI: https://doi.org/10.6028/NIST.SP.1270 / https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.1270.pdf
- DALLE: https://www.vox.com/future-perfect/23023538/ai-dalle-2-openai-bias-gpt-3-incentives
- Google: https://ai.googleblog.com/2018/09/introducing-inclusive-images-competition.html

- https://github.com/Trusted-AI/AIF360/tree/master/examples

- Facebook, Balance : https://github.com/facebookresearch/balance

## Fairness
- https://arxiv.org/pdf/2102.08453.pdf

## Robutness
* Notes
- http://www.trustworthymachinelearning.com/

* Ex. 
	- Confiance interval 
	- Perturbations : graines aléatoire
	- MAPIE
  

## Environment

- Impact environment : carbonml
- Solutions : small data ?


## Reproducibility

Notes: 
- Tracking
- Model registry
- Train Dataset 

Tools: 
- mlflow


# Platform :
- https://github.com/Giskard-AI/giskard


# Stategic Themes


## Human-Centered: "Contrôle Humain"
## Responsability
## Privacy


**Quelques sources:**

* Algo Audit: http://algaudit.inrialpes.fr/
* Projet INRIA régulation numérique: https://www.inria.fr/en/regalia-pilot-project-regulation-algorithms
* Interview Clément Henin et Daniel Le Métayer: https://linc.cnil.fr/fr/clement-henin-et-daniel-le-metayer-fournir-des-explications-du-fonctionnement-des-algorithmes
* Vidéo BigData Paris: https://www.alain-bensoussan.com/avocats/nouveau-reglement-sur-lia-pour-une-ia-digne-de-confiance/2021/10/25/
* Réglement: https://www.senat.fr/europe/textes_europeens/COM_2021_206.pdf
* Human-Learn: https://github.com/koaning/human-learn
* Labelia Labs: https://github.com/LabeliaLabs/referentiel-evaluation-dsrc
* Méthodo : https://dataanalyticspost.com/grille-evaluation-dispositifs-medicaux/amp/
* Fiancial Risk Management and Explainable Trusworthy, Responsible AI: https://www.frontiersin.org/articles/10.3389/frai.2022.779799/full
* "Domaine de validité": https://www.quantmetry.com/blog/domaine-de-validite-ia-confiance/
* Faire émerger un cadre sur IA Confiance (construction outil IA de Confiance - Responsable (label IA resp en FR et Europe de l'Ouest): https://www.youtube.com/watch?v=Ip4dCZ8xhEo
* Implicity: autorisation FDA, algo ECG: https://www.prnewswire.com/news-releases/implicity-receives-fda-clearance-for-ai-powered-ecg-analyzer-for-implantable-loop-recorders-301446711.html?tc=eml_cleartime
* https://fortune-com.cdn.ampproject.org/c/s/fortune.com/2022/03/22/ai-explainable-radiology-medicine-crisis-eye-on-ai/amp/
* ML in High-Risk Applications: https://learning.oreilly.com/library/view/machine-learning-for/9781098102425/
* https://www.seldon.io/using-explainable-ai-xai-for-compliance-and-trust-in-the-healthcare-industry
* Trusworthy AI: https://csdl-downloads.ieeecomputer.org/mags/co/2023/02/10042078.pdf?Expires=1677230283&Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiaHR0cHM6Ly9jc2RsLWRvd25sb2Fkcy5pZWVlY29tcHV0ZXIub3JnL21hZ3MvY28vMjAyMy8wMi8xMDA0MjA3OC5wZGYiLCJDb25kaXRpb24iOnsiRGF0ZUxlc3NUaGFuIjp7IkFXUzpFcG9jaFRpbWUiOjE2NzcyMzAyODN9fX1dfQ__&Signature=bTlcKKXtID1zywcPUxJSfte2GKSLWwKYxaUZb53hMCrbcoholFbfKys5nAv-qDwJXTpFFd0JXj~s0FH0sx9IDfXNcEocUFVBmJcaoy17YqWlPtjuG9QihbwZsl0qkcRdnMHrbLB7n5fl1yDO17aAl0d2qzCkpmH8XYQnytgvuCMka2jGqdUEnAvl8EgW3hQMB6oyvOc2dw-ndBoaVJJssvqqt7Dw~qmKlyVuCOX48VKmM5LP8ear1ZCtbn1fgU87ZaDIRj3XuiOsqZUYCRcpaPABFOr3oK~z3Y4~GdbFntjhf7J8JB80elaO15RaE487SMkeGaYq6vKJVlGLJTn-SA__&Key-Pair-Id=K12PMWTCQBDMDT
* AAAI Spring Symposium 2023: https://aita.sciencesconf.org/
* Example of ethical charter (pole emploi): https://www.pole-emploi.org/files/live/sites/peorg/files/images/Communiqu%c3%a9%20de%20presse/Charte%20de%20p%c3%b4le%20emploi%20pour%20une%20Intelligence%20Artificielle%20%c3%a9....pdf



Books: 
- ML in High-Risk Applications: https://learning.oreilly.com/library/view/machine-learning-for/9781098102425/
  * Chp1: Contemporary Model Governance: "Going fast and breaking thinkgs. It can mean that a small group of data scientists and engineers causes real harm at scale to many people." -> Cas d'application sur la voiture autonome chez Uber (gestion incidents, risk management, documentation).
  * Chap2: Debugging ML Systems: "Tests data area under the curve (AUC) tells us almost nothing aboout harms or security vulnerabilities. Yet these problems are often whu AI systems fail once deployed." -> Cas d'application octroi de crédit (détection de dérives, stress-tests).
  * Chap3: Security for ML: "The worst ennemy of security is complexity. Unduly complex AI systems are innately insecure." -> Censure anti-terroriste de FB (Attaques, vol de données / modèles, sécurité IT)
* https://csdl-downloads.ieeecomputer.org/mags/co/2023/02/10042078.pdf?Expires=16775762de%20l%27orga%20hi%C3%A9rarchique39&Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiaHR0cHM6Ly9jc2RsLWRvd25sb2Fkcy5pZWVlY29tcHV0ZXIub3JnL21hZ3MvY28vMjAyMy8wMi8xMDA0MjA3OC5wZGYiLCJDb25kaXRpb24iOnsiRGF0ZUxlc3NUaGFuIjp7IkFXUzpFcG9jaFRpbWUiOjE2Nzc1NzYyMzl9fX1dfQ__&Signature=q4XZkM-AYoMgGHBnRE9iIJlIWMA5BCQBTTqtdftLtIaXuYRy1-eLUdzP4Vz1yPgu2hm8FBcKS3-Fx-fvR1p61ur7ehV2-I5jLjPERv5kZuLDfXvX91G566akf8kbaudTzUY37cNhC5-Dvl8kxiN274fh1PwrindCf2a-SJWkNwH8BMTmnyNEUjsGz2PMIIBsAyROSg3wTHL2pS6l0Rz6cMC65BFRwTbw0Dp3uj3Q2R1Vz~5k-P7Lcj03ETpyDZ-DoIA28cVfyCRIUXcd0HRo~Qx24iZtnhuo8QDzXnrMTJRm6X4G7qiZB9I4-OMz43nmsWpTm0jGK1xq1bnNIPqtYA__&Key-Pair-Id=K12PMWTCQBDMDT



