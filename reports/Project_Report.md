# Pharmaceutical Environmental Monitoring and Contamination Risk Analytics

## Project Overview

This project focuses on the analysis of pharmaceutical Environmental Monitoring data to understand microbial contamination patterns, identify high risk areas and microorganisms, and assess contamination related risks.

The analysis combines pharmaceutical microbiology knowledge with Python, data analysis, visualization and machine learning techniques to develop a practical decision support approach.

## Project Objectives

The main objectives of this project are to understand contamination patterns across Grade C and Grade D areas, identify recurring microorganisms, identify high risk locations, analyze probable contamination sources, study excursion trends and develop an early warning risk assessment model.

## Dataset

The dataset contains Environmental Monitoring records from pharmaceutical manufacturing areas.

The analysis covers Grade C and Grade D areas and includes Settle Plate, Active Air Sampling and Surface Monitoring.

The monitoring conditions considered are At Rest and During Operation.

The dataset contains 2748 Environmental Monitoring records.

## Analysis Approach

The project follows a structured data science workflow.

Environmental Monitoring Data  
→ Data Cleaning  
→ Exploratory Data Analysis  
→ Excursion Analysis  
→ Microorganism Analysis  
→ Risk Analysis  
→ Feature Engineering  
→ Machine Learning  
→ Model Evaluation  
→ Business Insights and Recommendations

## Environmental Monitoring Analysis

Grade C areas were expected to follow a fortnightly monitoring frequency, while Grade D areas were expected to follow a monthly monitoring frequency.

The analysis identified a monitoring frequency gap for Grade C areas because the available records were recorded as Monthly.

Grade D monitoring frequency was aligned with the expected monthly schedule.

## Excursion Analysis

A total of 45 Grade C and Grade D excursion records were identified.

Grade C accounted for 34 excursions and Grade D accounted for 11 excursions.

Most excursions were observed During Operation.

Surface Monitoring contributed 20 excursions, Settle Plate contributed 18 excursions and Active Air Sampling contributed 7 excursions.

## High Risk Areas

The highest number of excursions were observed in the Autoclave Activity Area and Washing Room.

Other important areas identified during the analysis were Media Preparation, Unloading Room, Inoculation Room and DSP 2.

These areas can therefore be considered for focused Environmental Monitoring review and contamination investigation.

## Microorganism Analysis

Bacillus spp. was the most frequently observed microorganism among Grade C and Grade D excursions.

The major microorganisms identified were Bacillus spp., Staphylococcus spp., Penicillium spp., Corynebacterium spp., Aspergillus spp. and Micrococcus spp.

Bacillus spp. accounted for approximately 35.6 percent of the Grade C and Grade D excursions.

The top three microorganisms together accounted for approximately 68.9 percent of the excursions.

## Probable Source Analysis

The identified excursions were grouped into personnel associated, spore former or environmental, and mould or environmental source categories.

Personnel associated contamination accounted for 17 excursions.

Spore former or environmental contamination accounted for 16 excursions.

Mould or environmental contamination accounted for 12 excursions.

This indicates that both personnel related and environmental contamination patterns should be considered during investigations.

## Bacillus Analysis

Bacillus spp. accounted for 16 Grade C and Grade D excursions.

All identified Bacillus excursions occurred During Operation.

Surface Monitoring contributed 8 excursions, Active Air Sampling contributed 4 excursions and Settle Plate contributed 4 excursions.

The major areas associated with Bacillus excursions were Washing Room, Autoclave Activity Area, Inoculation Room, DSP 2 and Media Preparation.

The strongest high risk patterns were observed around the Autoclave Activity Area and Inoculation Room.

## Personnel Associated Contamination

Staphylococcus spp., Corynebacterium spp. and Micrococcus spp. showed personnel associated contamination patterns.

The identified events were mainly observed During Operation.

During investigation, areas such as gowning practices, personnel movement, operator interventions, aseptic behaviour and cleaning practices can be reviewed according to site procedures.

## Mould Analysis

Penicillium spp. and Aspergillus spp. represented the mould related contamination pattern.

A total of 12 mould related excursions were identified.

During investigation, cleaning and disinfection practices, HVAC conditions, humidity, temperature, utilities, equipment maintenance and facility conditions can be reviewed when supporting data are available.

Any specific disinfectant or antifungal strategy should follow validated site procedures and QA requirements.

## Risk Analysis

Among the 45 Grade C and Grade D excursion records, 24 were classified as High Risk and 21 were classified as Medium Risk.

Approximately 53.3 percent of the identified excursions were classified as High Risk.

All High Risk records occurred During Operation.

Surface Monitoring, spore former or environmental microorganisms, personnel associated microorganisms and mould related microorganisms were important contributors to the identified risk patterns.

## Batch Impact Assessment

Out of the 45 Grade C and Grade D excursion records, 23 records were classified as having potential risk to an ongoing Teriparatide Drug Substance batch.

The remaining 22 records showed no immediate batch impact signal.

These results are intended for risk assessment support and should not replace formal investigation, QA review or batch disposition.

## Trend Analysis

The analysis showed an increase in Grade C and Grade D excursions during the later part of the study period.

January 2025 to March 2025 accounted for 24 of the 45 Grade C and Grade D excursions.

Bacillus spp. was the major microbial contributor during this period.

## Control Strategy

The identified contamination patterns can be used to support a risk based control strategy.

High risk areas can be prioritized for focused Environmental Monitoring review.

During Operation monitoring can receive additional attention during activities associated with higher contamination risk.

Recurring microorganisms can be investigated together with their probable source categories.

Personnel practices, cleaning and disinfection, HVAC, utilities, equipment and facility conditions can be reviewed as part of investigations.

Specific corrective actions should follow approved site procedures, QA requirements and applicable regulatory controls.

## Machine Learning Approach

A Machine Learning model was developed to assess contamination risk using the available monitoring and operational information.

During model development, CFU Result was initially considered as a feature.

However, CFU Result was excluded from the final model because the excursion target is directly related to CFU results and applicable limits. Including CFU Result could therefore introduce target leakage.

The final model used Grade, Monitoring Method, Condition and Ongoing Batch as input features.

A Random Forest classifier was used for the final risk screening approach.

## Model Performance

The tuned Random Forest model achieved a ROC AUC of 0.712 and a recall of 0.973.

The precision was 0.112 and the F1 score was 0.200.

The high recall indicates that the model was able to identify most of the contamination risk events, while the relatively low precision indicates that the model also generated a number of false positive predictions.

Therefore, the model is more suitable for early warning and risk screening rather than standalone decision making.

## Project Limitations

The analysis is based on the Environmental Monitoring parameters available in the dataset.

RH, temperature, HVAC and detailed personnel information were not directly available for modelling.

Additional environmental, equipment and personnel data could improve future analysis.

The observed relationships should be considered as associations and should not automatically be interpreted as causal relationships.

Machine Learning predictions should support, and not replace, formal Environmental Monitoring investigations, QA review and CAPA procedures.

## Final Conclusion

The project identified important microbial contamination patterns, high risk areas and operational risk trends across Grade C and Grade D areas.

Bacillus spp. was the dominant microorganism among the identified excursions, while the Autoclave Activity Area and Washing Room showed the highest number of excursions.

The Machine Learning model showed potential for early identification of contamination risk events, with a ROC AUC of 0.712 and recall of 0.973.

Overall, the project demonstrates how pharmaceutical microbiology knowledge can be combined with Data Science and Machine Learning to support Environmental Monitoring analysis, risk assessment and investigation planning.

