# COVID-19-Vaccine-Classification-based-on-symptoms-text
## Objective
Classify the type of Covid 19 vaccine from the symptoms caused by the vaccine reported in the VAERS reports.
## Material and methods
Bag of Words(BoW)and term frequency-inverse document frequency vectorized(TF-IDF)classifiers are for text extraction and then Multinomial Naive Bayes was used to classify the vaccine type based on the text. The classes pfizer and moderna were imbalanced so SMOTE was used before implementing text classification model. Compared the two techniques through F1 score, accuracy and precision.
## Results 
After excluding vaccination errors and dropping duplicates, 15,772 VAERS reports were retained for the analysis.The overall model accuracy using BoW TECHNIQUE was 98% with F1 score 99 for pfizer class and 64 for moderna class. The lime explaination highlighted itching word classidied class pfizer and old to class moderna. The word cloud of symptoms of moderna shows symptoms like sore arm, old, fatigue, headache. For pfizer, fever, vitals, feeling fainted, BP, dizzy. For the TfIdf technique, got an accuracy of 98%, with F1 score for moderna 45% and pfizer 99%. The lime explainer showed 'fever' to be a driving factor for class pfizer. Headache, pain, old, sore arm were major symptoms extracted by tfidf for class moderna. Fever, vital, fainting, dizziness, shakiness, blurry vision, rash, vomiting were major symptoms extracted by tfidf for class pfizer.
