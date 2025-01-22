# Detecting AI-Generated Product Reviews in Dravidian Languages

This repository contains the implementation details and codebase for the Shared Task on Detecting AI-Generated Product Reviews in Dravidian Languages, as part of DravidianLangTech@NAACL 2025.

## Overview
The primary goal of this task is to classify product reviews as AI-generated or human-written in various Dravidian languages. This repository employs state-of-the-art transformer models, deep learning architectures, and traditional machine learning techniques to achieve this objective.

## Approach

### Transformer Models
We leveraged pre-trained transformer models for feature extraction and classification:
- [`idajikuu/AI-HUMAN-detector`](https://huggingface.co/idajikuu/AI-HUMAN-detector)
- [`akshayvkt/detect-ai-text`](https://huggingface.co/akshayvkt/detect-ai-text)
- [`MayZhou/e5-small-lora-ai-generated-detector`](https://huggingface.co/MayZhou/e5-small-lora-ai-generated-detector)

### Deep Learning Models
We implemented and fine-tuned the following deep learning architectures:
- **Recurrent Neural Networks (RNN)**
- **Gated Recurrent Units (GRU)**
- **Long Short-Term Memory Networks (LSTM)**
- **Bidirectional LSTMs (BiLSTM)**

### Machine Learning Models
We trained and evaluated traditional machine learning models for this task:
- **Random Forest**
- **Support Vector Machines (SVM)**
- **XGBoost**
- **Decision Tree**

## Repository Structure
```
├── data
│   ├── train dataset
│   └── test dataset
├── models
│   ├── transformers
│   ├── deep_learning
│   └── machine_learning
├── scripts
│   ├── preprocess.py
│   ├── train.py
│   └── evaluate.py
├── notebooks
│   └── exploration.ipynb
├── results
│   └── metrics
└── README.md
```

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/dravidian-ai-detector.git
   cd dravidian-ai-detector
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
1. **Preprocess Data:**
   ```bash
   python scripts/preprocess.py --input data/raw --output data/processed
   ```
2. **Train Models:**
   ```bash
   python scripts/train.py --model_type <transformer|deep_learning|machine_learning>
   ```
3. **Evaluate Models:**
   ```bash
   python scripts/evaluate.py --model_path models/<model_name>
   ```

## Results
| Model Type           | Accuracy | Precision | Recall | F1-Score |
|----------------------|----------|-----------|--------|----------|
| Transformer          | XX.XX%  | XX.XX%    | XX.XX% | XX.XX%   |
| Deep Learning (GRU) | 58%     | 77.1739%  | 58%  | 49.0043%   |
| Machine Learning     | XX.XX%  | XX.XX%    | XX.XX% | XX.XX%   |

## Contributing
Contributions are welcome! Please create a pull request or raise an issue if you encounter any problems.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact
For questions or collaborations, please contact [Anindo Barua Bijoy](https://www.linkedin.com/in/anindo-barua-bijoy/).
