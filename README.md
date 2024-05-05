Overview
Sentiment analysis is a natural language processing (NLP) task that involves determining the sentiment polarity of a given text. In this project, we utilize SVM, a popular machine learning algorithm, for sentiment classification. The dataset used for training and testing consists of text comments along with their corresponding sentiment labels.

Requirements
Python 3.x
pandas
matplotlib
scikit-learn (sklearn)

Usage
Clone the repository to your local machine:
git clone https://github.com/your-username/your-repository.git

Navigate to the project directory:
cd your-repository

Install the required Python packages:
pip install -r requirements.txt

Run the script:
python sentiment_analysis.py


Workflow
Data Loading: The script loads the dataset from a CSV file containing text comments and their associated sentiment labels.
Data Preprocessing: Missing values in the 'Comment' column are handled by replacing them with an empty string. Sentiment labels are assigned based on the 'polarity' column.
Exploratory Data Analysis (EDA): The number of positive and negative comments is counted, and a bar graph is plotted to visualize the distribution of sentiments in the dataset.
Data Splitting: The dataset is split into training and testing sets using a specified ratio (default: 80% training, 20% testing).
Model Training: A text classification pipeline is constructed using CountVectorizer and TfidfTransformer for feature extraction and SVM with a linear kernel for classification.
Model Evaluation: The trained model is evaluated on the test set using various metrics including accuracy, precision, recall, and F1 score. Classification reports are generated for both the training and testing sets.
