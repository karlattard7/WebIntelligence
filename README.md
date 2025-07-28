# Web Intelligence

## Task 1: Graph Analytics on Twitter Mention Network

The goal of this task is to analyze a **mention graph** constructed from a provided Twitter dataset. In this directed graph:

- **Vertices** represent Twitter users
- **Edges** represent **mentions** (e.g., if `userA` mentions `userB`, a directed edge is created from `userA → userB`)
- **Edge weights** reflect the **number of times** one user mentions another

### Graph Analytics Performed

A variety of graph metrics and analyses were conducted, including:

- **Number of nodes and edges**: Gives a basic overview of graph size
- **In-degree and out-degree**: Measures user popularity (in-degree) and user activity (out-degree)
- **Degree distribution**: Shows how mentions are spread across users
- **Average path length**: Measures the average number of steps between all pairs of users
- **Global clustering coefficient**: Indicates the tendency of users to form clusters (i.e., groups of users frequently mentioning each other)
- **Closeness centrality**: Identifies how quickly a user can reach others in the network
- **Betweenness centrality**: Identifies users that frequently act as bridges between other users

### Visualizations

A graph visualization was also generated. In the visual:
- **Node size** is proportional to their weighted degree
- **Edge thickness** represents the frequency of mentions

These visuals help identify **key influencers**, **communities**, and **interaction intensity** within the network.

---

## Task 2: Information Retrieval Using the Vector Space Model

The objective of this task is to build a basic **Information Retrieval (IR) engine** that can return documents relevant to a user query using the **Vector Space Model (VSM)**.

### 🧾 Steps Involved:

1. **Preprocessing**:
   - Case folding (lowercasing)
   - Tokenization
   - Removal of stop words
   - Stemming to reduce words to their base/root form

2. **TF-IDF Computation**:
   - Calculates **Term Frequency–Inverse Document Frequency** to weight the importance of each term across all documents

3. **Similarity Matching**:
   - **Cosine similarity** is used to measure the angle between the query vector and each document vector

4. **Ranking**:
   - Documents are ranked in descending order based on similarity scores
   - A final list of the **most relevant documents** is returned to the user

This task demonstrates the effectiveness of simple IR techniques in finding relevant text content based on keyword relevance and semantic weighting.

