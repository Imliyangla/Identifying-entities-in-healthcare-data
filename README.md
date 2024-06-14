# Identifying entities in healthcare data 
> The aim of this project is to build a custom Named Entity Recognition (NER) system to identify diseases and treatments from medical data. This involves transforming datasets into sentence formats, defining features for a Conditional Random Field (CRF) model, training the model, and evaluating its performance. The final objective is to create a dictionary mapping diseases to their treatments. This system enhances data interpretation, aiding in service delivery and patient care.



## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)


## General Information
- `Aims`:Develop a custom NER system for identifying diseases and treatments. Enhance service delivery and patient care through meaningful data extraction.
- `Objective`: Map diseases to their corresponding treatments from textual medical data. Train and evaluate a CRF model to achieve accurate identification of medical entities.
- `Dataset`: The dataset contains: Train Sentences: 2,599, Test Sentences: 1,056. Labels: 'O' (Other), 'D' (Disease), 'T' (Treatment). Structure: Words in individual lines, blank lines indicating sentence boundaries.

## Methods:
- Data Preprocessing: Construct sentences from individual words and Label sentences appropriately.
- Concept Identification: Use PoS tagging to identify frequent NOUN and PROPN tokens.
- Feature Definition for CRF: Include PoS tags and preceding word information. Mark sentence boundaries.
- Feature Extraction: Extract feature values and labels for sentences.
- Model Building: Train a CRF model using the extracted features and labels.
- Evaluation: Predict labels for test data. Calculate F1 score to assess model performance.
- Custom NER: Map predicted treatments to diseases.
- Predict treatment for 'hereditary retinoblastoma.'

## Conclusions
- Accurate mapping of medical entities using the CRF model.
- The model has succesfully predicted the treatmetn for the disease 'herditary retinoblastoma' as 'radiotherapy'. Therefore, we can confidently say that this CRF model is able to predict treatments against diseases by using a NER system. 




## Technologies Used
- pandas - version 2.1.2
- numpy - version 1.26.1
- matplotlib - version 3.7.1
- spacy - version 3.7.5
- sklearn - version 1.5.0


## Acknowledgements
- We would like to thank UpGrad for giving us the oppurtunity to work on this project. 


## Contact
Created by [Imliyangla](https://github.com/Imliyangla) - feel free to contact us!




<!-- You don't have to include all sections - just the one's relevant to your project -->
