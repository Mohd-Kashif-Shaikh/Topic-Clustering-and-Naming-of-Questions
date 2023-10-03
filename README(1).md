
#  Introduction :-

The findings of a clustering analysis performed on a dataset of text-based queries are presented in this study. This analysis's main goal was to combine related questions in order to find underlying trends and insights in the data. The phases of the analysis are described in this report, along with the preprocessing methods used and the most important findings from the clusters that resulted.


# Data Overview :- 
Before delving into the clustering process, I performed an initial examination of the dataset:

"Null Values": I checked for the presence of null values using data.info(). Fortunately, there were no missing values in the dataset, ensuring that the data was complete and ready for analysis.

"Dataset Summary": I summarized the dataset using data.describe() to obtain key statistics about the data, such as the number of rows and columns.This information provided me a foundational understanding of the dataset.
# Data Preprocessing :-
 1) Text Preprocessing :-To prepare the text data for clustering, I applied a series of preprocessing techniques:
>

    Removal of Punctuation: I had removed non-alphabetical characters from the text to ensure consistency in our analysis.

    Lowercasing: Text was converted to lowercase to standardize the text data.

    Tokenization: Sentences were tokenized into individual words.

    Stopword Removal: Common English stopwords were removed to focus on meaningful words.

    Stemming: Words were stemmed using the Porter stemming algorithm to reduce variations and facilitate clustering.


2) Text Vectorization :-To prepare the text data for clustering, I apploed the CountVectorizer technique. This method converted textual information into a numerical format suitable for clustering.
>

    CountVectorizer: I used CountVectorizer from scikit-learn to transform the text corpus into a term-frequency matrix. This involved tokenization, removal of stopwords, and stemming to reduce word variations.



## Algorithms used :
Clustering Algorithm :-

For the clustering analysis,I had employed the Latent Dirichlet Allocation (LDA) algorithm, a powerful technique commonly used for text clustering and topic modeling. 
## Results and Observations :-
Cluster Labels :- Based on the clustering analysis,I divided the dataset into four distinct clusters. Each cluster was assigned a label based on the dominant theme or content found within it:



    Cluster 0: "Paper Folding Puzzles"

    Cluster 1: "Family & Relationship Descriptive"

    Cluster 2: "Visual Patterns Recognition"

    Cluster 3: "Arrangement & Movement Scenarios"

## Conclusions :-
In this clustering study, I successfully classified comparable questions into meaningful clusters based on the content and themes present in the text data. The use of LDA as the clustering algorithm produced significant clusters. The validation metric (CHI) confirmed the separation of clusters.

These clusters can now be used to acquire insights into the various types of queries in the dataset and aid in various downstream tasks.
##  Future Work :- 
By tweaking the clustering process and researching other methods like feature engineering or various clustering algorithms, even better clustering results may be obtained. Domain-specific knowledge may also be contributed to the clusters in order to enhance their interpretability for the best outcomes.
