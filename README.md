# MLOPS-Assignment2
ML OPS assignment for Hugging Face Fine-Tuning, Experiment Tracking &amp; Model Deployment

This project demonstrates a complete **MLOps workflow** — By importing the notebook file to Kaggle, enable free GPU feature ON in kaggle, training the model, tracking experiments with Weights & Biases, and deploying the model to Hugging Face Hub.

============================================================================

**Kaggle Link:** https://www.kaggle.com/code/rvivekanandhan/g25ait2077-vivekanandhanr-mlops-assignment-2

**Hugging Face model link:** https://huggingface.co/Vivek-ML-Projects/distilbert-goodreads-genres

**WandB Dashboard:** https://wandb.ai/vivek-iitj/mlops-assignment2

============================================================================

**Project Description**

This project implements a full MLOps pipeline for fine-tuning a DistilBERT model on the UCSD Goodreads book reviews dataset to classify book reviews into 8 different genres (Poetry, Children, Comics & Graphic, Fantasy & Paranormal, History & Biography, Mystery/Thriller/Crime, Romance, and Young Adult). 

The workflow includes importing the notebook file to Kaggle, enable free GPU feature ON in kaggle and tokenization, model training using Hugging Face Transformers and experiment tracking with Weights & Biases (W&B), detailed evaluation using classification metrics, and finally deploying the trained model and tokenizer to the Hugging Face Hub for public access. The entire process focuses on reproducibility, production-ready code practices and end-to-end MLOps principles.

============================================================================

**Model Selection**

I chose the **DistilBERT-base-cased** model because it offers an excellent balance between accuracy and efficiency. According to its Hugging Face model card, DistilBERT is a distilled version of BERT that reduces the number of parameters by 40% while retaining about 97% of BERT’s performance on language understanding benchmarks. 

This makes it faster and lighter, which is ideal for projects where computational resources are limited or where real-time inference is required. Despite being smaller, DistilBERT still captures rich contextual information from text, making it suitable for tasks such as sentiment analysis, classification, and question answering. 

I've selected this model because it provides strong results with lower memory and processing requirements, making it practical for both academic experiments and deployment in production environments.

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



