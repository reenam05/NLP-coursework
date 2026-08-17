# Machine Learning Algorithm from scratch
 In this project, I had to independently research rule based and machine learning algorithms for different use cases. The aim was to learn which scenarios are best suited for a particular model.  

To show my understanding, I stated assumptions that should be considered, the performance of the model, test cases to show the model works under different conditions and the explanation of my approaches.

## Algorithms Implemented

- Rule based approach to classify an ambiguous word based on surrounding context in a paragraph.
  - The window (array) contains the context which would indicate the meaning of the word.
  - Disambiguous word: light (light - of little weight or light - pale in colour)
  - Created a vocabulary which links certain words to the different meanings of light
  - Created test cases
 
- Rule based spam detection
  - Created a vocabulary of spam related words
  - Used a count system to identify spam
  - Created test cases

- Anaphora resolution
  - Created the labels for the part of speech in sentences.
  - Implemented Hobbs Algorithm from scratch to detect the antecedent in a sentence. (E.g. Sentence: Alice and Peter shared a cake she felt sick .   Antecedent: Alice . )
  - Created test cases
 
- Named Entity Recognition
  -  Implement a Named Entity Recognition system that identifies and classifies entities into at least three categories (e.g., PERSON, LOCATION, ORGANISATION)
  - Used existing dataset to train the model (CoNLL-2002)
  - Used the Conditional Random Fields to identity and classify enities
  - Evaluated model using precision, recall, accuracy, f1-score

- Offensive Language Identification
    - Implement a system to classify social media posts as potentially offensive or 
non-offensive.
    - Used the OLID dataset to train the model
    - Used Support Vector Machine for binary classification
    - Converted samples of data into embeddings using TF-IDF

## Technologies
- Python
- Numpy
- NLTK
- sklearn
- sklearn_crfsuite

## Installation
git clone https://github.com/reenam05/NLP-coursework.git

cd NLP-coursework

pip install -r requirements.txt  

code main.ipynb

## Running the Project
Click on Execute cell next to the code cell

## Results
Accuracy: 
Named Entity Recognition - 97.5%
Offensive Language Identification - 75.9%

More evaluations for each approach are found in the notebook!