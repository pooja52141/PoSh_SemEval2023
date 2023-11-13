# PoSh at SemEval-2023 Task 10: Explainable Detection of Online Sexism

## Abstract
The growing popularity of online platforms and social media has intensified the problem of sexism, making it more prevalent and widespread. Online platforms have provided an anonymous space where individuals can freely express their misogynistic beliefs with discriminatory and abusive language, creating a culture of online harassment and hate speech, mainly targeting women. The dataset used in this task was provided by SemEval-2023 Task 10: Explainable Detection of Online Sexism. To precisely identify the different forms of online sexism, we utilize several sentence transformer models such as ALBERT, BERT, RoBERTa, DistilBERT, and XLNet. By combining the predictions from these models, we can generate a more comprehensive and improved result. Each transformer model is trained after pre-processing the data from the training dataset. Our team obtained macro f1 scores of 0.7937 for subtask A, 0.5284 for subtask B and 0.2674 for subtask C.

## Task Description
The task consists of three hierarchical subtasks. Task A is a binary classification problem where the goal is to predict whether a post is sexist or not sexist. Task B is a four-class classification problem where the system has to further classify sexist posts as (1) threats, (2) derogation, (3) animosity, or (4) prejudiced discussions. The goal of task C is to classify sexist posts as one of the 11-fine grained vectors. A common training dataset contains rewire_id, text, and label_sexist for task A, label_category for task B and label_vector for task C. The training dataset contains 14,000 rows of data. The development and test dataset for each task has rewire_id and text. For task A there were 2,000 rows of development and 4,000 rows of test data and for tasks B and C, 486 rows of data were for development and 970 for testing. All the data was in English. The final submission file contains rewire_id and label_pred which is the label predicted by the model for the corresponding text.
