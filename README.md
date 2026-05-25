# MLOPS-Assignment2
ML OPS assignment for Hugging Face Fine-Tuning, Experiment Tracking &amp; Model Deployment

This project demonstrates a complete **MLOps workflow** — converting a Jupyter notebook into production scripts, tracking experiments with Weights & Biases, and deploying the model to Hugging Face Hub.

============================================================================

**Kaggle Link:** https://www.kaggle.com/code/rvivekanandhan/g25ait2077-vivekanandhanr-mlops-assignment-2

**Hugging Face model link:** https://huggingface.co/Vivek-ML-Projects/distilbert-goodreads-genres

**WandB Dashboard:** https://wandb.ai/vivek-iitj/mlops-assignment2

============================================================================

**Project Description**

This project implements a full MLOps pipeline for fine-tuning a DistilBERT model on the UCSD Goodreads book reviews dataset to classify book reviews into 8 different genres (Poetry, Children, Comics & Graphic, Fantasy & Paranormal, History & Biography, Mystery/Thriller/Crime, Romance, and Young Adult). 

The workflow includes converting the Jupyter notebook to clean and modular Python scripts (data.py, train.py, eval.py, utils.py), proper data preprocessing and tokenization, model training using Hugging Face Transformers and experiment tracking with Weights & Biases (W&B), detailed evaluation using classification metrics, and finally deploying the trained model and tokenizer to the Hugging Face Hub for public access. The entire process focuses on reproducibility, production-ready code practices and end-to-end MLOps principles.

============================================================================

**Model Selection**


DistilBERT-base-cased was chosen because it is 40% smaller and 60% faster than BERT-base while keeping about 97% of its language understanding ability. This made it ideal for this MLOps assignment, which focused on workflow efficiency instead of maximum accuracy.


============================================================================
### Setup Instructions

1. Import notebook `g25ait2077-vivekanandhanr-mlops-assignment-2.ipynb` into Kaggle.
2. Enable GPU: Settings → Accelerator → GPU T4 x2.
3. Enable Internet: Settings → Internet ON.
4. Add Kaggle Secrets: `WANDB_API_KEY` and `HF_TOKEN`.
5. Run all cells.
6. Push the fine tuned model to hugging face
7. Check the performance of model in WandB

============================================================================

**Results**
 
| **Metric**| **Score** |
|-----------|-------|
| Accuracy  | 0.571 |
| F1 Score  | 0.583 |
| Eval Loss | 2.401 |

============================================================================



