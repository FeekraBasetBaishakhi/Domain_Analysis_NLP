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

2.How many times it appears

3.Listed in order from most to least frequent
