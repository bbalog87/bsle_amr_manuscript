# AMR and BSLE Epidemiological Analysis

## Overview
This repository contains the **data analysis scripts and resources** for the study on antimicrobial resistance (AMR) and extended-spectrum beta-lactamase-producing Enterobacteriaceae (BSLE) in relation to human-wildlife interactions. The study investigates the prevalence of **multidrug resistance (MDR) and BSLE carriage** and evaluates key risk factors such as socio-demographic factors and wild animal consumption.

The analysis follows **reproducible research principles** using Python for data processing, statistical modeling, and visualization.



**Title:** Zoonotic Transmission and Antimicrobial Resistance: The Role of Human-Wildlife Interactions in the Spread of Extended-Spectrum Beta-Lactamase-Producing Enterobacteriaceae (BSLE)

**Abstract**
Antimicrobial resistance (AMR) is a growing public health challenge, particularly in settings where human-wildlife interactions may facilitate the transmission of resistant bacteria. This study investigates the prevalence and risk factors associated with multidrug resistance (MDR) and extended-spectrum beta-lactamase-producing Enterobacteriaceae (BSLE) among individuals with different exposure histories, including wild animal consumption. Using a structured epidemiological survey and phenotypic/genotypic resistance profiling, we analyzed the impact of socio-demographic characteristics and potential transmission pathways. Logistic regression modeling identified wild animal consumption as a statistically significant predictor of BSLE carriage (OR = 2.85, 95% CI: 1.08–7.53, p = 0.035), while MDR prevalence was nearly universal (98.8%), making statistical differentiation challenging. These findings underscore the importance of One Health approaches in AMR surveillance and intervention strategies.

**Introduction**
Antimicrobial resistance (AMR) has become one of the most pressing global health challenges, threatening the efficacy of current therapeutic strategies. The rapid emergence and dissemination of multidrug-resistant (MDR) and extended-spectrum beta-lactamase-producing Enterobacteriaceae (BSLE) complicate clinical management, particularly in resource-limited settings. While healthcare environments have been widely studied as AMR reservoirs, increasing evidence suggests that human interactions with wild animals may contribute to the emergence and transmission of resistant bacteria through environmental and dietary pathways. However, the role of human-wildlife interactions in the spread of MDR and BSLE remains poorly characterized. 

The objective of this study is to assess the prevalence of MDR and BSLE, evaluate their association with socio-demographic characteristics and wild animal consumption, and provide a deeper understanding of potential zoonotic AMR transmission routes. By integrating epidemiological data with resistance profiling, we aim to inform evidence-based policy interventions for AMR containment.

**Materials and Methods**

**Study Design and Population**
This cross-sectional study enrolled participants from diverse socio-economic backgrounds, capturing information on demographics, antibiotic use, healthcare exposure, and dietary habits, including wild animal consumption. Biological samples were collected from each participant, and bacterial isolates were subjected to phenotypic antimicrobial susceptibility testing and genotypic characterization of resistance markers. 

A total of 250 participants were recruited, stratified into different exposure groups based on self-reported interaction with wild animals. Ethical approval was obtained, and informed consent was secured from all participants prior to sample collection.

**Sample Collection and Laboratory Analysis**
Biological samples (fecal and nasal swabs) were collected from participants under aseptic conditions. Bacterial isolates were obtained using selective media and identified via biochemical and molecular assays. Phenotypic resistance was assessed using the disk diffusion method on Mueller-Hinton agar, following CLSI guidelines. BSLE production was confirmed using the double-disk synergy test. 

Genotypic characterization of resistance genes (TEM, SHV, CTX-M, OXA-1) was performed using multiplex PCR. Molecular detection of blaCTX-M variants was conducted to assess the genetic diversity of BSLE isolates.

**Statistical Analysis and Model Justification**
Descriptive statistics were used to summarize demographic and resistance data. Logistic regression was employed to identify predictors of BSLE carriage, adjusting for potential confounders. Logistic regression is the most appropriate model for this study due to its ability to quantify associations between categorical dependent and independent variables while controlling for multiple risk factors. Given the high MDR prevalence (98.8%), Fisher’s exact test was used for MDR analysis, as traditional regression methods failed to converge due to complete separation.

**Figure Interpretation and Data Insights**

1. **Forest Plot (Adjusted Odds Ratios for BSLE Risk Factors)**
   - This plot displays the **odds ratios (OR) and 95% confidence intervals (CI)** for key predictors of BSLE carriage.
   - The **logarithmic scale** ensures proper visualization of ORs that vary greatly in magnitude.
   - **Interpretation:**
     - **Sex (Male)**: OR = 6.00 (95% CI: 1.72–21.02, p = 0.005) → Males are six times more likely to carry BSLE-producing bacteria than females.
     - **Wild Animal Consumption**: OR = 2.85 (95% CI: 1.08–7.53, p = 0.035) → Significant association, indicating a zoonotic transmission risk.
     - **Hospitalization History**: OR = 3.88 (95% CI: 0.69–21.97, p = 0.125) → Positive trend, but not statistically significant.
     - The **red vertical line at OR = 1** represents the null hypothesis (no association). Factors with confidence intervals that do not cross this line are statistically significant.

2. **Bar Plot (BSLE Prevalence by Wild Animal Consumption)**
   - This figure shows the proportion of individuals carrying BSLE-producing bacteria based on whether they consumed wild animals.
   - **Key Findings:**
     - **Individuals who consumed wild animals had a higher BSLE prevalence** than those who did not.
     - **Reinforces the statistical association seen in logistic regression.**

3. **Heatmap (AMR Co-Resistance Patterns)**
   - Displays pairwise **correlations** between antibiotic resistance patterns.
   - **Interpretation:**
     - Strong **positive correlations (red)** indicate that resistance to certain antibiotics frequently co-occurs.
     - **Examples:** Resistance to **Cefotaxime (CTX) and Ceftazidime (CAZ)** was strongly correlated, reflecting the shared resistance mechanisms among third-generation cephalosporins.
     - High correlation values suggest **cross-resistance**, which complicates treatment strategies.

**Discussion**
This study provides critical insights into the role of human-wildlife interactions in the spread of antimicrobial resistance. The nearly universal prevalence of MDR (98.8%) indicates a strong selective pressure for resistance, likely due to excessive antibiotic exposure in both clinical and community settings. The association between BSLE carriage and wild animal consumption (OR = 2.85, p = 0.035) suggests a potential zoonotic transmission pathway, highlighting the need for enhanced surveillance in regions where wildlife consumption is common.

The observed male predominance in BSLE carriage (OR = 6.00, p = 0.005) aligns with previous studies indicating differential exposure risks, possibly related to occupational and dietary behaviors. While hospitalization history trended toward increased risk (OR = 3.88, p = 0.125), the lack of statistical significance suggests that community transmission routes may play a more substantial role in resistance dissemination.

Our findings emphasize the importance of One Health approaches in AMR mitigation strategies. Integrated surveillance systems that incorporate human, animal, and environmental data are essential for understanding resistance dynamics and designing targeted interventions. Policymakers should prioritize regulations limiting antibiotic misuse in both human medicine and livestock production while promoting public awareness campaigns on the risks associated with wildlife consumption.

**Conclusion**
This study provides compelling evidence that human-wildlife interactions contribute to the spread of BSLE, emphasizing the need for integrated One Health surveillance strategies. The high prevalence of MDR underscores the urgent need for coordinated global action to combat AMR. Future research should focus on longitudinal studies and whole-genome sequencing approaches to trace resistance transmission pathways more precisely. Strengthening antimicrobial stewardship programs and enhancing public health messaging regarding zoonotic AMR risks will be crucial steps toward mitigating the impact of drug-resistant infections on human and animal populations.

**Keywords**: antimicrobial resistance, BSLE, MDR, wild animal consumption, One Health, zoonotic transmission
