# LuxVeri at GenAI Detection Task 3: Cross-Domain Detection of AI-Generated Text Using Inverse Perplexity-Weighted Ensemble of Fine-Tuned Transformer Models

This repository contains the code and models used for our participation in **Task 3 of the GenAI Content Detection Workshop at COLING 2025**, focusing on **Cross-Domain Machine-Generated Text (MGT) Detection**.  

## 📌 Competition Overview  

For details on the competition, visit:  
[COLING 2025 Workshop on MGT Detection Task 3](https://github.com/liamdugan/COLING-2025-Workshop-on-MGT-Detection-Task-3)  

## 📝 Task Description  

Task 3 focuses on detecting AI-generated text across multiple domains, including **non-adversarial** and **adversarial settings**:  

- **Subtask A: Non-Adversarial MGT Detection**  
- **Subtask B: Adversarial MGT Detection**  

## 🏆 Our Approach & Results  

We developed an **inverse perplexity-weighted ensemble** method using fine-tuned transformer models for improved cross-domain generalization.  

### **Subtask A (Non-Adversarial MGT Detection)**  
- **Models Used**:  
  - Fine-tuned RoBERTa-base  
  - RoBERTa-base with OpenAI detector integration  
- **TPR Score**: **0.826**  
- **Rank**: **10/23**  

### **Subtask B (Adversarial MGT Detection)**  
- **Models Used**:  
  - Fine-tuned RoBERTa-base  
- **TPR Score**: **0.801**  
- **Rank**: **8/22**  

## 📂 Provided Files  

We have submitted Jupyter Notebook (`.ipynb`) files containing our full pipeline, including:  
✅ Data Preprocessing  
✅ Model Training & Fine-tuning  
✅ Inference & Ensemble Predictions  
✅ Evaluation & Submission Formatting  

📌 **Please check the notebooks for complete implementation details.**  

## 🔧 Installation & Usage  

### Environment Setup  

```bash
pip install -r requirements.txt
```
### Running the Notebooks

Open and run the .ipynb files in Jupyter Notebook or Google Colab.


```bash
jupyter notebook
```

### 📊 Evaluation
To validate predictions before submission:

```bash
python format_checker.py --prediction_file_path=predictions.jsonl
python scorer.py --gold_file_path=data/gold_labels.jsonl --prediction_file_path=predictions.jsonl
```

### 📜 Citation
If you use our work, please cite:

```bash
@misc{mobin2025luxverigenaidetectiontask,
      title={LuxVeri at GenAI Detection Task 3: Cross-Domain Detection of AI-Generated Text Using Inverse Perplexity-Weighted Ensemble of Fine-Tuned Transformer Models}, 
      author={Md Kamrujjaman Mobin and Md Saiful Islam},
      year={2025},
      eprint={2501.11918},
      archivePrefix={arXiv},
      primaryClass={cs.CL},
      url={https://arxiv.org/abs/2501.11918}, 
}
```