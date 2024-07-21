# F-score

A measure of predictive performance in Information Retrieval systems.
Its calculated using the precision and recall  of the test. 

- Precision: true positive / total predicted positive samples
    a.k.a Positive Predictive Value
    
- Recall: true positve / total sample that should have been predicted positive
    a.k.a Sensitivity 


There atleast is two kinds F1 and Fbeta.
- F1 is harmonic mean (?) of precison and recall, defined as:
    = 2 * (precion * recall / percision + recall)
    = 2tp / 2tp + fp + fn

- Fbeta: uses (B) factor so that recall is B times as important as precision
    https://en.wikipedia.org/wiki/F-score

