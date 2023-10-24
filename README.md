# RumourDetectionResearch
Links:
AARD
https://github.com/yunzhusong/AARD 

BiGCN
https://github.com/TianBian95/BiGCN 

PLAN:
https://github.com/Ameame1/rumor-detection
https://github.com/Ameame1/Rumor-Out-of-Domain-Exploring-Method

WILL:
https://github.com/WillTan14/wills-ensemble

/Analysis.xlsx contains results from experiments


## AARD

1. Pytorch 1.4.0 and its associated packages are very difficult to find and install, thus install a more recent version instead (i.e. Pytorch 1.8.1)
2. If installing with CUDA, ensure that the procedures for installing the associated CUDA version is also installed together (in this case, CUDA11.1 was already installed)
3. Find relevant link from https://data.pyg.org/whl/ in order to install torch scatter, torch sparse, torch cluster as well as the associated version of torchvision and torchaudio detailed in https://pytorch.org/get-started/previous-versions/ 
4. Install en-core-web-sm from https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-3.0.0/en_core_web_sm-3.0.0-py3-none-any.whl (link from requirements.txt)
5. Install every other package from the given requirements.txt
6... (Further Instructions to be written)

## BiGCN

1. Pytorch 1.4.0 and its associated packages are very difficult to find and install, thus install a more recent version instead (i.e. Pytorch 1.8.1)
2. If installing with CUDA, ensure that the procedures for installing the associated CUDA version is also installed together (in this case, CUDA11.1 was already installed)
3. Find relevant link from https://data.pyg.org/whl/ in order to install torch scatter, torch sparse, torch cluster as well as the associated version of torchvision and torchaudio detailed in https://pytorch.org/get-started/previous-versions/ 
4. Install tqdm and joblib normally
5. Dataset for T15 and T16 should be first processed by running the following codes:<br />
    python ./Process/getTwittergraph.py Twitter15<br />
    python ./Process/getTwittergraph.py Twitter16
6. This creates the folder /data/Twitter##graph containing necessary .npz files
7. Copy and paste these .npz files into both directories - this is IMPORTANT to have it be able to test cross-domain

## Ensemble
1. GLoVe vectors must be installed from https://nlp.stanford.edu/projects/glove/