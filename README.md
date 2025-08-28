# 2D Footprint Clustering based on Graph Similarity Measures
This repository is an exercise is to reproduce the methodologies in [Duong et al. (2023)](https://doi.org/10.1145/3615900.3628790). The paper discusses the potential of using the concepts of graph similarity and spectral clustering to cluster a set of building footprints based on similarities of their shape characteristics. The authors suggest that a geometric graph distance, rooted in Wasserstein distance from transportation theory, is capable of capturing the graph structure as well as the spatial properties of the geometric graph. The methods and algorithm were tested and fine-tuned on dataset from Hanford Village George Washington Carver Addition area as a prototype, where it mainly has Cape Cod houses, duplexes, and industrial buildings.

## Dependencies
- `numpy`
- `scikit-learn`
- `POT`
- `cython`
- `wwl`
- `igraph`
- `scipy`
- `matplotlib`
- `sklearn`
- `skgeom`
- `shapely`
- `networkx`

## Workflow
1. Skeleton Graph Computation
2. Graph Embedding: From skeleton graph to graph features
3. Continuous Weisfeiler-Lehman and Wasserstein Distance Computation
4. Spectral Clustering

## Preliminary results
| | Spectral Clustering | K-means Clustering |
| :------: | :------: | -------: |
|Silhouette analysis| <img width="598" height="537" alt="Screenshot 2025-08-27 215353" src="https://github.com/user-attachments/assets/0a893621-5bd7-4c66-94d7-adcd3624d986" /> | <img width="598" height="537" alt="Screenshot 2025-08-27 215518" src="https://github.com/user-attachments/assets/c97bbd49-4c7e-449c-a57d-3a8312ad50e4" /> |
|*k*=2| <img width="597" height="806" alt="Screenshot 2025-08-27 215631" src="https://github.com/user-attachments/assets/3140ae8f-82c9-42b1-82bf-e89f0c8e3b43" /> | <img width="589" height="804" alt="Screenshot 2025-08-27 215750" src="https://github.com/user-attachments/assets/9fa1c54a-8626-4d73-bef8-72e2dbcbcdef" /> |
|*k*=3| <img width="588" height="806" alt="image" src="https://github.com/user-attachments/assets/cf43f60a-67bf-4341-802b-2df3a9830960" /> | <img width="585" height="802" alt="image" src="https://github.com/user-attachments/assets/111813c0-c881-4e1d-8260-e8c9e6cf712b" /> |
|*k*=4| <img width="585" height="807" alt="image" src="https://github.com/user-attachments/assets/3afecc13-77e8-44af-a597-c12775f015cb" /> | <img width="597" height="807" alt="image" src="https://github.com/user-attachments/assets/b96cc534-625b-4a25-8b0c-e804b3059f88" /> |
 





