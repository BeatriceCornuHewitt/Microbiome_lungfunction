# Analysis scripts for: The Upper Respiratory Tract Microbiome is Associated with Lung Function in Adults: Cross-Sectional and Longitudinal Analyses in a Population-Based Cohort
[![MIT License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

**Authors**: Beatrice Cornu Hewitt <a href="https://orcid.org/0000-0002-4594-4393" target="orcid.widget" rel="noopener noreferrer" style="vertical-align:top;"><img src="https://orcid.org/sites/default/files/images/orcid_16x16.png" style="width:1em;margin-right:.5em;" alt="ORCID iD icon"></a><br>
**Contact**: b.cornuhewitt@uu.nl<br>

## Study Overview
This repository contains the complete analytical pipeline for our study investigating the relationship between the upper respiratory tract (URT) microbiome and respiratory health. We utilize data from the Dutch VGO cohort (Veehouderij en Gezondheid Omwonenden), a large population-based study designed to assess the health effects of living near livestock farms.
The analysis integrates high-resolution 16S rRNA gene sequencing data from both nasopharyngeal (NP) and oropharyngeal (OP) niches with longitudinal clinical spirometry data spanning a 7-year follow-up period.

## Objective
The primary objective of this work was to determine whether the composition and diversity of the URT microbiome are associated with lung function parameters and their decline over time. Specifically, we aimed to:
1. Identify specific microbial taxa in the NP and OP associated with spirometry outcomes 
2. Evaluate the longitudinal stability of the URT microbiome over 7 years.
3. Assess whether baseline microbial profiles can predict spirometry outcomes after 7 years, or the rate of lung function decline.

## Methods
- NP and OP swabs from: rural residents at T0 (2014/15) and T1 (2021/22) were collected as part of the VGO study in 2 phases. 16S rRNA sequencing was carried out to characterise the microbiome. 
- Spirometry was also conducted at T0 and T1 of the same participants during home visits. 
- The analysis was split into the 3 questions defined above, exploring the associations between the URT microbiome and spirometry outcomes. 

## Key Findings
- Niche Differentiation: We observed distinct microbial signatures between the NP and OP, with the NP showing higher stability but lower overall diversity compared to the OP.
- Associations with Lung Function: Cross-sectionally several key genera were significantly associated with spirometry outcomes (higher NP *Streptococcus*, *Prevotella*, and *Moraxella* and higher OP *Bifidobacterium* were linked to lower lung function).
- Stability over Time: While the URT microbiome is dynamic, we identified a core set of taxa that remained highly stable within individuals over the 7-year follow-up.
- Predictive Value: Several baseline taxa, including NP *Moraxella* and *Anaerococcus* and OP *Rothia dentocariosa*, were linked to poorer follow-up lung function

## Repository navigation
*  [`0_functions.R`]: Curated functions for analyses
*  [`1_Cleaning_spirometry_data.Rmd`]: Script for processing raw clinical data
*  [`2_Cross_sectional_analyses.Rmd`]: Core cross-sectional microbiome analyses.
*  [`3_Longitudinal_analyses.Rmd`]: Stability analysis and longitudinal analyses.