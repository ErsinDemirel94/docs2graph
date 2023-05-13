# Docs2graph
Colab test to try combining NER and simple rules to create a social network from a list of documents.
How does it work?
- Provide a list of texts with possible named entities. (Turkish)
- Apply NER using huggingface to detect and extract named entities such as people, organizations and location.
- Convert the output into pandas dataframe.
- Tokenize and deduplicate outputs to join same occurrences with slight different differences in writing.
- Using a simple rule, convert the dataframe into a graph format. (If 2 name occur in same document, create a relationship.)
- Visualize relations using networkx library.
![alt text](https://github.com/ErsinDemirel94/docs2graph/blob/main/indir.png)
