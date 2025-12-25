## Clinical Trial Phase Classification Using NLP

This project investigates whether the phase of a COVID-19 clinical trial can be predicted from its textual description.

## Key Findings

Linear models consistently confused adjacent phases, reflecting real clinical overlap.

Phase 4 recall remained low across models due to semantic similarity with Phase 3.

Hierarchical classification improved interpretability but was limited by error propagation.

Performance ceilings were caused by representation limits, not model choice.

## Conclusion

In this project, I was predicting COVID-19 clinical trial phases using text data. 
Starting with TF-IDF, I evaluated multiple linear classifiers, including Logistic Regression and Linear SVM. 
Detailed analysis of confusion matrices and model coefficients showed that there were misclassifications occurring in different phases of the trial.
Despite applying class weighting, switching classifiers, and reformulating the task as hierarchical
classification, model performance, particularly recall for late-stage (Phase 4) trials, consistently
stayed the same. Further investigation revealed that this limitation is in the clinical trial text data.
The key outcome: text-only TF-IDF features are insufficient to really classify the exact clinical trial
phase, especially in late (phase 3, phase 4) stages. This finding highlights the importance of feature
representation and problem formulation in applied machine learning and motivates future work
incorporating structured metadata or contextual embeddings.
