![image](https://github.com/Alex-Fuster/hybrids_drought/assets/73120146/d0d2e438-b0aa-482c-b2c3-e9abbdc7624b)# Reduced fitness under abiotic stress in F1 hybrids of Antirrhinum majus subspecies with divergent flower colors
**Alexandre Fuster-Calvo, Coline C. Jaworski, Carina Basket**

## ABSTRACT

What maintains trait divergence in the face of gene flow? Two subspecies characterized by flower color in wild Antirrhinum majus L. (snapdragon) readily form hybrid zones where they meet. The sharp clines indicate strong selection on flower color, but the causal agents of selection are unknown. Because flower pigmentation is often implicated in abiotic stress tolerance, we experimentally compared drought tolerance of each subspecies and F1 hybrids from allopatric crosses. In benign conditions, all plants survived, and hybrids tended to be taller than parental phenotypes. However, hybrids had lower survival under drought stress than either parent. We hypothesize that survival probability is directly related to flower color genes, as hybrids that flowered were less likely to survive. Thus, reduced hybrid fitness due to maladaptation to abiotic stress may contribute to maintaining flower color divergence in the face of gene flow in A. majus.

## Repository description

FOLDERS:

- **`data/`** contains the raw data used for the analyses
- **`figures/`** figures of the manuscript produced in the code 
- **`tables/`** tables of the manuscript produced in the code
- **`scripts/`**:

    - *compute_dataset_analyses.Rmd*: it builts the dataset **dataset.csv** used for all the analyses from raw data in the **data** folder.

    - *mixed_models_treatment.color.Rmd*: it runs models to analyze the effects of flower color and treatment on trait responses. It produces Figure 1 and S2.

    - *compute_figure2A.Rmd*: it produces Figure 2A.

    - *risk_death_flowering.Rmd*: it tests for differences in death risk between flowering and non-flowering phenotypes conducting two-sample Z tests. It produces Figure 2B.

    - *compute_figure_S1.Rmd*: produces Figure S1.

    - *compute_figure_S3.Rmd*: produces Figure S3.
 
    - *compute_figure_S4.Rmd*: produces Figure S4.
 
  ## Dataset metadata

  All the analyses are conducted using the *dataset.csv* file. Below are the descriptions of each variable in the dataset:

- Unique_id: unique identifier for each individual plant.
- block: Greenhouse tray.
- trt: treatment (3 levels: control, early drought, late drought).
- cross: cross between parents' plants. Each parent plant is identified with a letter, which indicates the population, and an individual number (e.g. T2315 is the individual 2315 of the population Tha).
- pop_parent_1: letter of the population of parent 1 (e.g. T).
- pop_parent_2: letter of the population of parent 2.
- colors: phenotype, where M_M reders to *A.m. pseudomajus*, Y_Y refers to *A.m. striatum*, and M_Y to F1 hybrids.
- first_flower: date of first flower.
- wilt1: date of wilting signs over the first checking week.
- wilt2: date of wilting signs over the second checking week.
- wilt3 to wilt8 (").
- dead1: death at transplanting date.
- dead2: death at harvest.
- survived: survival at harvest (1 = survived).
- height_cm: plant height at harvest (cm).
- leaf_nodes_main: number of leaf nodes of tallest stem at harvest.
- bushiness: number of leaf nodes of secondary stems at harvest.
- flower_count: number of flowers produced throughout the experiment, surveyed at harvest.
- days_1flower: number of days from the start of the experiment to the first flower opening.
- flowering: presence of flowering = 1 (surveyed throughout experiment, so an individual may have 1 here and NA for flower count at harvest).
- w_b: whether cross is within or between populations.
- pop_T: whether any parent belongs to population T.
- pop_B: whether any parent belongs to population B.
- pop_V: whether any parent belongs to population V.
- pop_P: whether any parent belongs to population O.
- pop_L: whether any parent belongs to population L.
- initial_h: height when transplanted into greenhouse pots.
    
  

For any inquiries, please reach out to alexfuster7@gmail.com or cbaskett3@gatech.edu
