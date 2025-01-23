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
├── Data Augmentation
│   ├── Data Augmentation.ipynb
│   ├── Final_augmentated_data(tamil)
│   └── Final_augmentated_data(malayalam)
├── data
│   ├── train dataset
│   └── test dataset
├── models
│   ├── transformers
│   ├── deep_learning
│   └── machine_learning
├── results
│   └── metrics
└── README.md
```

## Results
Tamil:

| Model Type           | Accuracy | Precision | Recall | F1-Score |
|----------------------|----------|-----------|--------|----------|
| Transformer          | 70%  | 70.33%    | 70% | 69.707%   |
| Deep Learning (GRU) | 51%     | 46.0210%  | 51%  | 38.2893%   |
| Machine Learning     | XX.XX%  | XX.XX%    | XX.XX% | XX.XX%   |

Malayalam:

| Model Type           | Accuracy | Precision | Recall | F1-Score |
|----------------------|----------|-----------|--------|----------|
| Transformer          | 90%  | 90.5844%    | 90% | 89.9638%   |
| Deep Learning (GRU) | 58%     | 77.1739%  | 58%  | 49.0043%   |
| Machine Learning     | XX.XX%  | XX.XX%    | XX.XX% | XX.XX%   |



## Contributing
Contributions are welcome! Please create a pull request or raise an issue if you encounter any problems.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact
For questions or collaborations, please contact [Anindo Barua Bijoy](https://www.linkedin.com/in/anindo-barua-bijoy/).
