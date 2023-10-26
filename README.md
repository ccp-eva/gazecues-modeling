# Variation in gaze understanding across the life span: A process-level perspective

---

> Project repository with source code, data files and analysis scripts associated with the studies.

---

## Pre-Print

Prein, J. C., Maurits, L., Werwach, A., Haun, D. B. M., & Bohn, M. (2023). Variation in gaze understanding across the life span: A process-level perspective. Retrieved from osf.io/preprints/psyarxiv/dy73a

## Structure

```
.
├── data                                    <-- data files
├── figures                                 <-- plots presented in the paper / supplements
├── model                                   <-- computational cognitive models (gaze model, random guessing, center bias)
├── paper
    ├── gazecues_modeling.pdf               <-- pre-print
|   └── manuscript.Rmd                      <-- manuscript file
├── saves                                   <-- saved output from stats analyses
├── stats
|   ├── gazemodel.Rmd                       <-- analysis for Study 2
|   ├── lifespan.Rmd                        <-- analysis for Study 1
│   ├── magnet.Rmd                          <-- analysis for Study 3
│   ├── supplements_animalvshumans.Rmd      <-- comparison TANGO with human vs. animal faces
│   ├── supplements_changepoint_parameters.Rmd <-- parameter settings for change point analysis in Study 2
│   └── supplements_gaussianprocess.Rmd     <-- trial-level vs. subject-level gaussian process model for Study 2
└── supplements
    └── supplements.Rmd                     <-- supplements file
```

<img src="./figures/gazemodel.png">

**Set-up and geometrical features of our gaze model.** 
Our gaze model assumes participants click at a certain point where two estimated gaze vectors meet. 
Each of these gaze vectors implies an estimated pupil angle for each eye that results from connecting the center of the agent’s eyeball and the center of the pupil. 
These angles are sampled from a product of two independent Normal distributions with equal variance, which are centered around the true pupil angles. 
Development of gaze understanding corresponds to a decrease in variance of the Normal distributions and, therefore, a more precise localization of the attentional focus of the agent. 
The model predicts that TANGO trials vary in difficulty: participants should be more imprecise in locating the target the further out it lands, resulting in a U-shaped pattern.
