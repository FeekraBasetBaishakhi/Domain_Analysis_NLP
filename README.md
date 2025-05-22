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
