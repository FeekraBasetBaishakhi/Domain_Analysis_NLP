# Domain_Analysis_NLP
This project analyzes comments from Domestic Violence and Abusive Relationship discussion forums to identify and analyze the external websites and resources being shared within these communities. The analysis helps understand what online resources are most frequently referenced in discussions about domestic violence and abusive relationships.


1. Domain Extraction

Systematically scans through each comment to identify URLs. Then extracts domain names from identified URLs using pattern matching. Maintains a running list of all domains found. Then did special handling for URLs with 'www' prefix.

2. Text Cleaning

Removes complete URLs from the text and preserves the surrounding context of the discussion. Maintains the original meaning of comments while eliminating technical clutter.

3. Frequency Analysis

Counts total occurrences of each domain and generates frequency distribution of shared domains. Identifies most commonly referenced websites.

Output Generation:

1.Domain Statistics

1.Total count of domains found in the dataset.

2.Frequency distribution of domain occurrences.

3.List of unique domains identified.

2.Processed Dataset

1.Clean text without URLs.

2.Preserved comment context.

3.Ready for further natural language processing.


This code analyzes pairs of words (bigrams) in comments to find the most frequently occurring word combinations. For example, it can identify that phrases like "sexual violence" or "support groups" appear frequently in the text.

Methodology:

Step 1:Data Preparation

Takes the comments from our dataset and remove any empty or missing comments. Converts all text to proper string format for analysis.

Step 2:Setting Up the Analysis

Uses a tool called CountVectorizer to find word pairs then removes common English words (like "the", "and", "is") that don't add meaningful information. Specifically looks for pairs of words (bigrams) rather than single words.

Step 3:Counting and Sorting

Counts how many times each word pair appears in all comments and creates a list of all word pairs with their counts.Sorts them from most frequent to least frequent and keeps the top 20 most common word pairs

Output Generation:

Produces a clear list showing:

1.Each word pair (bigram)

This code analyzes groups of three consecutive words (trigrams) in the comments to identify the most common three-word phrases. For example, it can find patterns like "group helpline sidebars" or "support looking resources" that appear frequently in discussions.

This component of the project focuses on cleaning and standardizing text data from ""Domestic Violence"" and ""Abusive Relationship"" forum comments. It transforms raw text into a standardized format suitable for analysis by removing unnecessary elements and normalizing the text.

Required Tools: The process uses the Natural Language Toolkit (NLTK) for text processing, including:

1.Word tokenization (breaking text into words).

2.Stop words removal (removing common words).

3.Lemmatization (reducing words to their base form).

This documentation describes a Python script designed to analyze text data from comments, specifically focusing on word frequency analysis and visualization. The script processes comments from a CSV file, identifies the most frequently occurring words, and creates both numerical and visual representations of the findings.

Then  calculates the length of comments in the dataset to understand their distribution. Using the cleaned and filtered dataset 'abusiverelation_domesticviolence_comments_cleaned_filtered.csv', a new column named 'comment_length' is added, which contains the character count of each comment. Missing values in the 'comment_body' column are replaced with empty strings to ensure accurate computation. Statistical metrics such as the mean, minimum, maximum, and quartiles of comment lengths are then computed and displayed, providing insights into the variability and typical length of comments within the dataset.

 program analyzes how long comments are in a dataset from what appears to be a domestic violence support forum. It processes all comments from a CSV file and measures the length of each comment (counting the number of characters). The analysis helps understand how detailed or brief people's comments typically are in these discussions.

The program creates a visual representation of this data through a histogram, which shows how comment lengths are distributed. The histogram uses sky blue bars with black edges to make it easy to read, and displays how many comments fall into different length ranges. Additionally, it calculates basic statistical information about the comments, such as the average length, the shortest and longest comments, and how much the lengths vary. This information helps understand typical patterns in how people communicate in these support forums. The results are saved as a PDF file for future reference and further analysis.

The analysis begins by gathering information about each author's activity in the dataset. The program counts how many comments each unique author has posted, creating a complete record of posting frequency for every author in the system. This gives us the raw data about who posts and how often they contribute.
2.How many times it appears

This program performs a focused analysis of author participation patterns in the dataset. It first counts how many different authors (unique users) have posted comments, providing a clear picture of the community's size. Then, it goes a step further by creating a detailed mapping of each author's contribution.

Then identifying and examining the most active participants in the community by organizing authors based on their comment volumes. The program takes all author-comment pairs and sorts them in descending order based on the number of comments each author has made, effectively ranking authors from most to least active. It then zooms in on the top 50 most prolific authors, creating a focused view of the community's most engaged members. For each of these top contributors, the program displays their username and their total number of comments, providing a clear picture of who the most active participants are and exactly how much they've contributed to the community discussion. This information is valuable for understanding the core group of users who drive most of the community's conversations and activity.

This analysis creates a visual representation of the most active participants' contributions in the community. The program selects the top 50 authors based on their comment counts and generates a bar chart to display their activity levels. 

This program creates a comprehensive visual representation of word usage patterns in comments by generating a word cloud visualization.

**Sentiment Analysis and Text Processing of Support Forum Comments**

Analysis of GPT's Classification of Comments Related to Abusive Relationships

Automated Detection of Abusive Relationship Comments Using Naive Bayes Classification

Identifying Abuse-Related Comments Using Logistic Regression Analysis

Identifying Abuse-Related Comments Using Support Vector Machine Analysis



3.Listed in order from most to least frequent
