# Neural Networks project, 2022
- ## Artist similarity with Graph neural Networks (re-implementation)
In this repository we present a complete re-implementation of the paper ['Artist Similarity with Graph Neural Networks'](https://arxiv.org/abs/2107.14541).
- Since the project's code wasn't provided by the authors, except for the [dataset](https://gitlab.com/fdlm/olga://paperswithcode.com/paper/artist-similarity-with-graph-neural-networks), we attempted to repeat the experiments described in the paper, and we have additionally tried 
4 additional Graph Neural Networks architectures.
- With some of these new architectures we were able to get even better results with respect to the GraphSAGE architecture.
Our best architecture outperforms the 3 layers GraphSAGE by the 15% in accuracy, even though we hadn't the access to the whole dataset.
Indeed we have obtained slightly different results from those described in the paper, but still they are coherent with the authors' conclusions.

The whole implementation is in the Olga.ipynb python notebook, whereas the other files in this repository are used to carry out the experiments.
* COOA.pt : This .pt file contains the adjacency matrix in 'coordinate format'.
* MsbMapped.json, graphSimilarities.json : These json files contain the relation between artists in a .json format; they are extracted and used within the notebook, the details are in the 'Olga.ipynb' file.
* dizofartist.json : This file contains the encoding between the id of an artist in the dataset and its name/band name.
* olga.csv : This is the olga dataset in .csv format.
* acousticbrain.npy : This file is too heavy and it is not present in this repository, but it is available at the main [project repository](https://gitlab.com/fdlm/olga://paperswithcode.com/paper/artist-similarity-with-graph-neural-networks). 
This file contains the numpy array of the nodes' features. Further details are explained in the notebook.
* models : It is the folder which contains all the trained models in our project.



