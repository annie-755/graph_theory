GRAPH THEORY -ASSIGNMENT 

ANDREA MARY
IMS24030

This project does recursive spectral modularity partitioning to detect communities in Zachary’s Karate Club Graph, and tracks how various centrality metrics evolve as the graph is repeatedly split into smaller sub-communities.

Here, we use spectral modularity maximization, introduced by Newman, to partition the graph:
Compute the modularity matrix for a subgraph
Compute its leading eigenpair
Use the sign of the leading eigenvector to split the community
Recursively repeat on the most “splittable” subgraph
Stop when the leading eigenvalue becomes ≤ 0, indicating no modular structure remains

it was observed that High-betweenness nodes (bridging roles) shifted in importance as communities were refined.
Nodes like 0, 1, 3, and 33 showed:
High betweenness before splitting.
Decreasing or redistributed betweenness after the second split.
Clustering coefficient patterns aligned with the community membership:
Higher clustering within stable Community A; lower clustering in B.


The algorithm uncovered a hierarchical community pattern:
First: 2 major communities.
Then: one of them further split → 3 total.
This hierarchy reflects the known social divisions of the Karate Club.
