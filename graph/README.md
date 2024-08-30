# CS224W: Machine Learning with Graphs
- Traditional methods: Graphlets, Graph Kernels
- Methods for node embeddings: DeepWalk, Node2Vec
- Graph Neural Networks: GCN, GraphSAGE, GAT, Theory of GNNs
- Knowledge graphs and reasoning: TransE, BetaE
- Deep generative models for graphs
## Classic Graph ML Tasks
- Node Classification
- Link prediciton
- **Graph classification**
- Clustering
## Node Features
### Node Centrality
- Node centrality $C_v$ takes the node importance in a graph into account
  -  Eigenvector  centrality
  -  Betweenness centrality
  -  Closeness centrality
### Clustering Coefficient
- Measures how connected $v's$ neighboring nodes are:
$$e_v=\frac{\textnormal{\#(edges among neighboring nodes)}}{\begin{pmatrix}k_v\\2\end{pmatrix}}\in[0,1]$$
### Graphlets
- Observation: Clustering coefficient counts the #(triangles) in the ego-network
  - <span style="color:orange">**Graphlets**</span>, i.e.,  #(pre-specified subgraphs): Rooted connected non-isomorphic subgraphs
#### <span style="color:skyblue">Graphlet Degree Vector(GDV)</span>
- A count vector of graphlets rooted at a given node
- Graphlet-base features for nodes
- node's local network topology