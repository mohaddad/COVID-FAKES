# COVID-FAKES
Bilingual (Arabic/English) COVID-19 Twitter dataset for misleading information detection

      -We provide an automatically annotated, bilingual (Arabic/English) COVID-19 Twitter dataset (COVID-19-FAKES). 

      -This dataset has been continuously collected from February 04, 2020, to March 10, 2020. 

      -We used the streaming options of the API to collect real-time data.

      -After establishing the connection, we used the following search keywords, which are the trendings related to the coronavirus disease (COVID-19), to collect the corresponding shared Tweets ("Coronavirus", "Corona_virus", "Corona-virus", "Novel_Coronavirus", "2019-nCoV", "Novel-Coronavirus", "NovelCoronavirus", "2019_nCoV", "nCoV", "COVID-19", "SARS-CoV-2", "covid19").

      -It could be remarked that Twitter API allows only the return of 3,200 Tweets per query at most. Moreover, due to some technical issues (connection errors, Internet problems, or power issues, etc.) we missed collecting some Tweets for sometimes during some days or for a few days.

      -For assigning labels to the collected Tweets and building different annotation models, we collected a set of ground-truth information related to COVID-19 disease. We rely on the published information on the official websites and official Twitter accounts of the WHO, UNICEF, and UN as we perceived as trusted information sources. Additionally, we enriched the collected ground truth with the pre-checked facts from various fact-checking websites. 

      -Label: (Real=1, Misleading=0).

      -The annotation process is divided into two phases. The first is the model-building phase, which is designed to train a binary classification model for 13 different machine learning algorithms while using 7 different feature extraction techniques with each of the used algorithms. While the second phase is the annotation phase. For the data in both phases, they are passed through the same preparation, preprocessing, and feature engineering steps (feature selection and feature extraction).

      -For generalization, we are reporting the obtained class of each Tweet with each of the 7 feature extraction techniques (Term Frequency (TF), Term Frequency Inverse Document Frequency (TF-IDF)-(unigram, bigram, trigram, N-gram, character level), and Word Embedding), for each of the used 13 machine learning algorithms (Decision Tree (DT), k-Nearest Neighbor (kNN), Logistic Regression (LR), Linear Support Vector Machines (LSVM), Multinomial Naive Bayes (MNB), Bernoulli Naive Bayes (BNB), Perceptron, Neural Network (NN), Ensemble Random Forest (ERF), Extreme Gradient Boosting (XGBoost), Bagging Meta-Estimator (BME), AdaBoost, and Gradient Boosting (GB)).



      -The English part of the dataset consists of 31  ".CSV" files.

      -Each file contains 100,000 TweetId and their corresponding classes.

      -The techniques are as follows:
            C1: Decision Trees.                      C2: Multinomial Naive Bayes.
            C3: Bernoulli Naive Bayes.               C4: Logistic Regression.
            C5: k-Nearest Neighbors.                 C6: Perceptron.
            C7: Multilayer Perceptron.               C8: Linear SVM.
            C9: Random Forest.                       C10: Bagging meta-estimator.
            C11: XGBoost.                            C12: AdaBoost.
            C13: Gradient Boosting (GBM).

      -The used Feature Extraction Techniques are as follows:
            1: Term Frequency (TF).                                                       2: Term Frequency Inverse Document Frequency (TF-IDF) - unigram.
            3: Term Frequency Inverse Document Frequency (TF-IDF) - bigram.               4: Term Frequency Inverse Document Frequency (TF-IDF) - trigram.
            5: Term Frequency Inverse Document Frequency (TF-IDF) - N-gram.               6: Term Frequency Inverse Document Frequency (TF-IDF) - character level.
            7: Word Embedding.


      -The column title indicates the technique used for assigning the corresponding class label (e.g., "C1_1---->Decision Trees using Term Frequency (TF)", "C4_7---->Logistic Regression using Word Embedding"). 

*This dataset was introduced in: (Mohamed K. Elhadad, Kin Fun Li, and Fayez Gebali, "COVID-19-FAKES: A Twitter (Arabic/English) Dataset for Detecting Misleading Information on COVID-19, "Advances in Intelligent Networking and Collaborative Systems - The 12th International Conference on Intelligent Networking and Collaborative Systems (INCoS-2020)", Springer, 2020. (https://doi.org/10.1007/978-3-030-57796-4_25)
