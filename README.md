# A Data-Driven Sliding-window Pairwise Comparative Approach for the Estimation of Transmission Fitness of SARS-CoV-2 Variants and Construction of the Evolution Fitness Landscape

## Table of Contents
- [Graphical Abstract](#Graphical%20Abstract)
- [Description](#description)
- [Installation](#installation)
- [Key Insights](#key-insights)
- [Data Preprocessing and Sliding Window Approach](#data-preprocessing-and-sliding-window-approach)
- [Project Structure](#project-structure)
- [Results and Insights](#results-and-insights)
<!-- - [License](#license) -->
<!-- - [Usage](#usage) -->

## Graphical Abstract
![Graphical Abstract](Figures/Manuscript_figures_JPG_format/Main%20Figures/Graph_Abstract.jpeg)

## Description
This repository contains the Differential Population Growth Rate (DPGR) model, a novel sliding-window, data-driven approach to estimate and compare the transmission fitness of SARS-CoV-2 variants. DPGR utilizes pairwise comparisons across specific time windows to quantify relative fitness advantages between viral strains, creating a dynamic fitness landscape that reflects the evolutionary trends of Variants of Concern (VOCs) such as Omicron and Delta. This generalized approach is appilcable to any viral surveillance dataset of exponentially growing viral populations.

By addressing key issues with sampling biases and allowing for real-time epidemiological insights, DPGR provides a robust framework that complements transmission fitness estimation.


## Installation
To set up and run the project locally, clone this repository and install the necessary dependencies:

```bash
git clone https://github.com/QinLab/DPGR.git
cd DPGR
pip install -r requirements.txt
```

## Key Insights

Here, we highlight some key insights from applying the DPGR model:

### Transmission Fitness Variability by Region
Omicron consistently exhibited higher transmission fitness over Delta across various geographic levels (countries and continents).

#### Fitness Estimation in the Country Level
![Transmission Fitness Estimation in Country Level](Figures/Manuscript_figures_JPG_format/Main%20Figures/Figure_1_omicron_vs_delta_countries_short.jpg)

#### Fitness Estimation in the Continent Level
![Transmission Fitness Estimation in Continent Level](Figures/Manuscript_figures_JPG_format/Main%20Figures/Figure_2_omicron_vs_delta_continents.jpg)


### Fitness Evolution Landscape Construction
The fitness landscape generated through pairwise DPGR analyses shows how each successive variant of concerns of SARS-CoV-2 dominates over the other. This model provides a clear visualization of the evolutionary trajectory in fitness between major VOCs.
![Constructed Evolution Fitness Landscape of USA](Figures/fitness_landscape_plots/USA_fitness_landscape_labeled.png)

### Fitness Stair of the Co-Circulating Variants
![Fitness Stair](Figures/figures_for_step_plot/USA_variant_step_plot.png)
![Fitness Stair of Omicron Sub-lineages](Figures/figures_for_step_plot/North%20America_omicron_sublineage_step_plot.png)


<!-- ![Fitness Landscape](images/fitness_landscape.png)

### Noise and Sampling Bias Robustness
DPGR remains resilient to sampling biases. When Gaussian noise or synthetic sampling bias was introduced, the model continued to yield reliable estimates with a consistent linear trend, indicating its utility in real-world genomic surveillance settings with incomplete data.

![Noise and Bias Robustness](images/noise_bias_robustness.png)
