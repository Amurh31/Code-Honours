A full Natural Language Processing (NLP) pipeline for isiZulu text classification using the multilingual transformer model XLM-RoBERTa. This project demonstrates how low-resource African languages can be modeled using modern deep learning techniques.

📌 Overview

This project builds an end-to-end text classification system that:

Processes raw isiZulu text
Automatically generates labels using rule-based methods
Trains a transformer-based model
Evaluates performance using standard metrics
Visualizes results for analysis

🗂️ Project Structure
📁 project-root
│── 📓 pre-training.ipynb     # Main notebook (pipeline)
│── 📄 README.md             # Project documentation
│── 📁 data/                 # Dataset (optional)
│── 📁 models/               # Saved model output
📂 Dataset

File: zul_community_2017-sentences.csv
Language: isiZulu
Content: Community-generated sentences
🔧 Preprocessing
Removed null values
Dropped duplicates
Cleaned text
🏷️ Labeling Strategy

Since the dataset is unlabeled, rule-based labeling is used.

Example Categories:
Category	Example Keywords
🌍 Geography	intaba, umfula, izwe
🔬 Science	physics, gravity, experiment

⚠️ Note: This is a weak supervision approach and may introduce noise.

⚙️ Tech Stack
🤗 Transformers (xlm-roberta-base)
🧠 PyTorch
📊 Scikit-learn
🐼 Pandas & NumPy
📈 Matplotlib & Seaborn
🔄 Pipeline Workflow
Data Loading & Cleaning
Automatic Label Generation
Train/Test Split (80/20)
Tokenization (max length = 128)
Model Training
Evaluation & Visualization
Model Saving
🧪 Model Training
Parameter	Value
Model	XLM-R Base
Epochs	6
Batch Size	8
Learning Rate	2e-5
Max Length	128
📊 Evaluation Metrics
✅ Accuracy
🎯 Precision
🔁 Recall
⭐ F1-score (Primary metric)
📈 Results Visualization

The notebook includes:

📊 Performance bar charts
🔲 Confusion matrix
💾 Model Output

Trained model is saved to:

./xlmr_zulu_final/

You can reload it for:

Inference
Deployment
Further training
🚀 Getting Started
1️⃣ Clone the Repository
git clone https://github.com/your-username/your-repo.git
cd your-repo
2️⃣ Install Dependencies
pip install -r requirements.txt
3️⃣ Run the Notebook
jupyter notebook
🧹 Memory Optimization
import torch, gc
torch.cuda.empty_cache()
gc.collect()
🔮 Future Work
📌 Use manually annotated datasets
📌 Improve label quality
📌 Hyperparameter tuning
📌 Compare with Afro-centric models
📌 Deploy as API or web app
🤝 Contributing

Contributions are welcome!



This project is licensed under the MIT License.

👤 Author

Amukelani Vuyani Majola
Sunday Adeola Ajagbe
https://github.com/Adeola80


