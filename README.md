# Reaction Time Analysis Using Factorial Experimental Design and ANOVA

## Overview

This project investigates how different behaviors and environmental stimuli
affect human reaction time using a controlled experimental design.
The analysis evaluates the effects of white noise, multitasking, and dominant
hand usage on reaction time performance measured in milliseconds.

A $2^3$ factorial randomized block design with replication was used to account for
between-participant variation while allowing for the estimation of main
effects and interaction effects between factors. Statistical modeling and
ANOVA techniques were applied to determine which factors significantly
influenced average reaction times and reaction time variability.

## Dataset

The dataset was generated experimentally through repeated reaction time tests
performed using a mobile reaction time application.

The Experiment:

- Setup:
  - 3 two-level experimental factors
  - 2 participants used as blocking factors
  - 4 replications for each treatment combination
  - Fully randomized run order
- Experimental Factors:
  - Noise: Presence or absence of white noise during testing
  - Multitask: Presence or absence of a simultaneous counting task
  - Dominant_Hand: Whether the participant used their dominant hand
- Blocking Factor:
  - Person: Participant identifier used to account for between-subject variation
- Response:
  - React_time: Reaction time measured in milliseconds
  
## Methods
- Experimental design construction
- Randomized block factorial design
- Replication and randomized run ordering
- Linear regression modeling
- Interaction effect analysis
- Analysis of variance (ANOVA)
- Smaller-the-better optimization analysis

## Models
- **Linear Regression Models:** Used to estimate the relationships between
experimental factors and average reaction time/variance of reaction times
- **ANOVA Framework:** Used to evaluate statistical significance of
main effects and interaction effects between experimental factors and
the average reaction time/variance of reaction times while accounting for 
the blocking variable

## Results

The analysis identified that cognitive multitasking is statistically associated with 
slower average reaction times, and none of the experimental factors were meaningfully
related to the variability of reaction times. 

The findings of the smaller-the-better analysis show that reaction times are fastest
under the absence of cognitive multitasking, which makes sense intuitively. 
Though this was the only experimental relationship found between the experimental
factors and the average reaction times, this finding has practical significance.
For example, those working in potentially dangerous circumstances should refrain
from cognitive multitasking to best prepare themselves for any quick decision-making
that may occur.

## Technologies
- R
- tidyverse
- MASS
- ANOVA
- Linear Regression
- R Markdown

## Structure
- Reaction_Time_Report.Rmd - Full analysis and modeling report/code
- Reaction_Time_Report.pdf - Report-ready document with only essential code
- Requirements.txt - R dependencies
- test1.jpg - Image of experimental conditions included in the report

## Notes
This project was completed as part of a graduate course project and adapted for portfolio presentation.