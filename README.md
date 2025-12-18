# mlb-pitch-velocity-differentials
This project analyzes and models the velocity differential between a pitcher’s primary fastball and their non-fastball offerings using publicly available MLB Statcast data from 2020–2024.


## Modeling Pitch Velocity Differentials Using Public Statcast Data ##

# Overview #
Velocity separation is a key component of pitch effectiveness, influencing hitter timing, pitch tunneling, and overall arsenal quality.

The goal of this project is to replicate a real-world baseball R&D workflow: from data cleaning and feature engineering through model development and evaluation.

Source: Public MLB Statcast data

Seasons: 2020–2024

Pitch-level features aggregated at the pitcher-season level

All data used in this repository is publicly accessible and reproducible.

Feature Engineering
Key feature groups explored include:

Pitch movement metrics (vertical and horizontal break)

Release characteristics (release height, horizontal release point)

Spin-related features (spin rate, transformed spin axis features)

Fastball baseline velocity

Pitch-type indicators for secondary offerings

Particular emphasis was placed on normalizing horizontal and vertical features to account for handedness effects.

Modeling Approach

Baseline linear models to establish interpretability

Tree-based models to capture non-linear interactions

Cross-validation at the pitcher level to reduce leakage

Evaluation focused on RMSE and stability across seasons

Results & Insights

Vertical movement and spin-related features were consistently strong predictors of velocity separation.

Horizontal movement features added explanatory power, particularly for sliders.

Explicit pitch-type indicators contributed less predictive value than underlying movement and spin characteristics.

Non-linear transformations of spin axis were useful for certain pitch classes but not universally beneficial.

Next Steps

Incorporate pitch usage and sequencing context

Evaluate season-to-season stability of velocity gaps

Explore hierarchical models to account for pitcher-level random effects
