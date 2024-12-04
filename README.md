# Named_Entity_Recognition_Healthcare
"BeHealthy" is a health-tech company and has a web platform that allows doctors to list their services and manage patient interactions and provides services for patients such as booking interactions with doctors and ordering medicines online. Here, doctors can easily organise appointments, track past medical records and provide e-prescriptions. So, companies like "BeHealthy" are providing medical services, prescriptions and online consultations and generating huge data day by day.

The following snippet of medical data may be generated when a doctor is writing notes to his/her patient or as a review of a therapy that he or she has done. "The patient was a 62-year-old man with squamous cell lung cancer, which was first successfully treated by a combination of radiation therapy and chemotherapy."

As we can see in this text, a person with a non-medical background cannot understand the various medical terms. We have taken a simple sentence from a medical data set to understand the problem and where one can understand the terms 'cancer' and 'chemotherapy'.

We have been given such a data set in which a lot of text is written related to the medical domain. There are a lot of diseases that can be mentioned in the entire dataset and their related treatments are also mentioned implicitly in the text, which we saw in the aforementioned example that the disease mentioned is cancer and its treatment can be identified as chemotherapy using the sentence. However, note that it is not explicitly mentioned in the dataset about the diseases and their treatment, but we can build an algorithm to map the diseases and their respective treatment.
The train dataset is used to train the Continuous Random Field (CRF) model, and the test dataset is used to evaluate the built model.

The model is trained with the following datasets:
-train_sent
-test_sent
-train_label
-test_label

I have performed the following broad steps:
You need to process and modify the data into sentence format. This step has to be done for the 'train_sent' and ‘train_label’ datasets and for test datasets as well.
After that, you need to define the features to build the CRF model.
Then, you need to apply these features in each sentence of the train and the test dataset to get the feature values.
Once the features are computed, you need to define the target variable and then build the CRF model.
Then, you need to perform the evaluation using a test data set.
After that, you need to create a dictionary in which diseases are keys and treatments are values.
