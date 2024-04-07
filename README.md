# Support-Vector-Classifier-for-Predicting-Survival-Likelihood-of-Hepatitis-Patients

Hepatitis is a disease characterized by the inflammation of the liver. It is a fairly common condition, and approximately 3.2 million people as of today suffer from either hepatitis B or C. Hepatitis A and B can be treated quite well through vaccination, but hepatitis C has no such effective vaccine. The biggest challenge when it comes to dealing with this virus, however, is that many infected individuals proceed with their lives without knowing that they are carrying the disease. In many cases, the lack of diagnosis allows the infected people's condition to progress to a stage where treatment can be difficult. Because of this, about 1.34 million people around the world die of hepatitis each year, the number being similar to that of many other infectious diseases such as HIV and malaria. Oftentimes, patients that are very likely to die from a certain condition aren't referred to a specialist as their doctors have a false perception of how well they are faring. In fact, only 8 percent of people admitted to hospitals needing specialized treatment end up receiving it. Therefore, knowing if a certain patient is at high risk of death is likely to greatly decrease the number of patients that die from any condition, including hepatitis. Also, improving our understanding of the risk factors that can contribute to a given prediction on whether or not a patient is likely to live or die can better inform us on how to diagnose diseases. Lastly, providing such predictions can allow doctors to provide proper treatment for a patient that is in critical condition. 60% of patients die in acute care hospitals, while 80% of Americans say that they would prefer to die at home.

The aim of this project is to build a model that, based on a few details about a given hepatitis patient, can provide an output on the individual's likelihood of survival.

These factors include:

The patient's age.
The patient's sexuality
Whether or not steroids were used for treatment.
Whether or not the patient was given antiviral drugs.
Whether or not the patient experiences fatigue(a large majority of people that have hepatitis experience severe tiredness).
Whether or not the patient experiences malaise(a feeling of nausea).
Whether or not the patient is diagnosed with anorexia.
Whether or not the patient has an enlarged liver.
Whether or not the patient has a firm liver.
Whether or not the patient's spleen is palpable.
Whether or not the patient has spider nevi(a certain condition where people can see thin lines under their skin as a result of an underlying issue)
Whether or not the patient has ascites(fluids being stored in the stomach).
Whether or not the patient has varices(odd, bloated up veins).
The patient's bilirubin levels.
The patient's alkaline phosphatase levels.
The patient's SGOT levels.
The patient's albumin levels.
When talking specifically about hepatitis, histology refers to "lobular disarray", which includes a multitude of complications. The attribute "histology" speaks to whether or not the patient suffers from these complications.
The target variable in the dataset is denoted as 'Class', and it tells us whether the patient in question did or didn't die from hepatitis or related complications.

For this project, three separate evaluation metrics will be used to assess the performance of a given model.

Accuracy: The model's accuracy is a helpful metric for getting an idea of how good the model is. However, since it is just a measure of the percentage of samples predicted correctly, it can return skewed results in imbalanced datasets. A number closer to 1 on this metric means that the model is more accurate.

ROC-AUC score: The model's ROC-AUC score refers to the area under the curve displaying the model's false positive rate against its true positive rate(recall). As with accuracy, this metric does not tell the entire story when used on an imbalanced dataset, because the false positive rate will generally be lower as a result of the large number of true negatives. This number should ideally be close to 1.

F1 score: The f1-score is a harmonic mean of precision and recall. This "combination" of precision and recall make f1-score a go-to metric in many problems, since precision and recall are both very important in and of themselves. It can also be more insightful than accuracy and AUC in imbalanced classification. As with the other two metrics, a score close to 1 is desirable. Because the dataset used in this project is heavily imbalanced, the f1-score will be the most important metric that's going to be taken into consideration when deciding whether a model works.

References

A Virus., 4-8-2021, "What is Viral Hepatitis?," No Publication, https://www.cdc.gov/hepatitis/abc/index.htm
Joseph Bennington-Castro, 4-25-2016, "AI can predict when we'll die — here's why that's a good thing," NBC News, https://www.nbcnews.com/mach/science/ai-can-predict-when-we-*ll*-die-here-s-why-ncna844276
Stephanie Soucheray, 4-21-2017, "WHO: Viral hepatitis deaths increasing," CIDRAP, https://www.cidrap.umn.edu/news-perspective/2017/04/who-viral-hepatitis-deaths-increasing

Liver &, 8-4-2021, "Acute hepatitis-general," No Publication, https://www.pathologyoutlines.com/topic/liveracutehepgeneral.html

neptune.ai, 7-19-2021, "F1 Score vs ROC AUC vs Accuracy vs PR AUC: Which Evaluation Metric Should You Choose?," https://neptune.ai/blog/f1-score-accuracy-roc-auc-pr-auc

Dataset used: Peter Turney), xx-xx-xxxx, "UCI Machine Learning Repository: Hepatitis Data Set," No Publication, https://archive.ics.uci.edu/ml/datasets/hepatitis

The files in this repository should be observed in the following order:
1. Initialization
2. Data Cleaning and Encoding Categoricals
3. Splitting the Data
4. Initial Model Testing
5. Binning and Polynomial Features for Improvement of LogisticRegression
6. Log Transform
7. Parameter Tuning
8. Test Set Evaluation
9. Analysis and Conclusion
10. Adding Percent Confidence to the Model
