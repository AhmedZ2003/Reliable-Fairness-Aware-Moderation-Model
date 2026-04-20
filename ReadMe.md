## Setup Instructions

### Requirements
- Python 3.10+
- GPU recommended for training, GPU used: RTX 3060.

### Installation
1. Clone or download this repository.
2. Install dependencies: pip install -r requirements.txt

### Data Preparation
- Download the [Jigsaw dataset](https://www.kaggle.com/competitions/jigsaw-multilingual-toxic-comment-classification/data)
- The notebooks expect CSV files with columns: `comment_text`, `toxic`, `black`, `white`, `muslim`, `jewish`.
- Run Part 1 to preprocess and split the data.

## How to use the notebooks?
- Run the Jupyter notebooks in order (part1.ipynb to part5.ipynb).
- Use `pipeline.py` for inference on new text.


The assignment is divided into five parts, each addressing a key aspect of building a reliable faireness moderation system:

- **Part 1**: Data preparation, model training, threshold optimization, and baseline evaluation.
- **Part 2**: Fairness audit on protected attributes (e.g., racial groups) using metrics like disparate impact and AIF360.
- **Part 3**: Adversarial attack simulations, including character-level evasion and label-flipping poisoning.
- **Part 4**: Mitigation strategies, such as reweighting, oversampling, and model calibration.
- **Part 5**: End-to-end pipeline integration and evaluation.

The final output is a `ModerationPipeline` class in `pipeline.py` that provides a structured decision-making process for moderating text.