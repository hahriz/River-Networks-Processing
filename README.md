# River networks code

The Python code converts the extracted river-channel network into a directed graph using NetworkX. The processed river channels are represented as continuous linear paths, which are first simplified through thresholding and skeletonization using scikit-image. The code then identifies and generates nodes from the processed channel network and establishes edges connecting these nodes along the river channels. Each edge is assigned a direction corresponding to the inferred upstream-to-downstream flow direction, producing a directed graph that represents the connectivity and flow structure of the river network. NetworkX is subsequently used to calculate in-degree and out-degree, degree centrality, closeness centrality, clustering coefficient, and betweenness centrality for the resulting directed network. 

Versions used are as follows: 
- matplotlib 3.5.1
- NetworkX 2.7.1
- NumPy 1.21.5
- Python 3.9.12 or 3.10
- SciPy 1.10.1
- Scikit-Image 0.19.2
- Skimage submodules 0.19.2
