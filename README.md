# Potential Talents

A talent sourcing and management company are interested in finding talented individuals for sourcing these candidates to technology companies. The data comes from the sourcing efforts. They have removed any field that could directly reveal personal details and gave a unique identifier for each candidate. The data is in tabular format and it contains the following attributes:
- id: unique identifier for candidate (numerical)
- job_title: job title for candidate (text)
- location: geographical location of candidate (text)
- connections: number of connections candidate has, 500+ means over 500 (text)
- fit: how fit the candidate is for this role? (numeric, probability between 0-1)

The objective is to predict how fit the candidate is based on their available information (variable fit). 

In this project, to find the ability to predict the candidates' fitness for the provided keywords (positions required), different Natural Language Processing techniques were implemented in order to calculate the similarities. A list of the different text preprocessing techniques that were used:

- TF-IDF
- Word2Vec
- GloVe.
- BERT.
A mean similarity score was added to the data based on the mean of the cosine similarities of each one of those techniques. Then, Learning to Rank (LTR) is a deep learning technique that was applied to re-rank the candidates based
