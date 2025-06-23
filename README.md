# ModernBERT for Aspect-Based Sentiment Analysis (ABSA) in Academic Peer Reviews


This project develops and evaluates a strong transformer-based baseline for sentence-level aspect-based sentiment analysis (ABSA) using the ASAP-Review dataset of academic peer reviews. The final implementation focuses on systematic fine-tuning and interpretability analysis of ModernBERT, demonstrating robust performance and model transparency.


## Features

Preprocessing, quality checks, and exploratory data analysis (EDA) for ABSA.

Baseline and ModernBERT classifier implementation using HuggingFace Transformers.

Hyperparameter sweep with Weights & Biases (WANDB) for robust model selection.

LIME-based interpretability: visual explanations of model decisions on real review examples.

Full reproducibility: scripts, notebooks, and environment files provided.

## Repository Structure


├── docs/                   # All reports including every stage of the development  
├── src/                    # Jupyter notebooks for EDA, training, and interpretability  
├── figures/                # LIME plots, learning curves, and result visualizations  
├── requirements.txt        # Python dependencies  
├── README.md               # This file  



## Getting Started
Clone the repository
```
git clone https://github.com/erdemert/IS584_Project.git
cd IS584_Project
```
Install dependencies.
Experiments are conducted on a Python 3.11.12 environment.
```
pip install -r requirements.txt
```
Place the dataset files (CSV) into the src/ directory.

Run the experiments.  
--EDA_ASAP_Review.ipynb #The source code that contains initial quality checks.  
--initial-training.ipynb #The file that contains the initial experiments with constant parameters.  
--final_training.ipynb #The file that contains the final source code including lime. (Run this file to --simulate the experiments.)  
--final_training_outputs_visible.ipynb #The file contains training except lime part but also contains the outputs of the experiments.  

Model checkpoints, best configurations, and scripts to reproduce all results and plots are available in the repository.  

WANDB experiment logs: https://wandb.ai/erdemerturk-middle-east-technical-university/aspect-sentiment-modernbert  

## Final Results
Test Macro-F1: 0.826  
Test Accuracy: 0.785  
Extensive interpretability analysis (LIME) shows the model focuses on aspect-relevant and contextually meaningful words.

## Contact
For questions or contributions, please open an issue or contact erdem.erturk@metu.edu.tr.

