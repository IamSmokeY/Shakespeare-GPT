# Shakesphere GPT

This project implements a decoder only GPT (Generative Pre-trained Transformer) model for text generation using PyTorch. The model is trained on a dataset of Shakespeare's works and can generate new text based on the learned patterns.

## Requirements

- Python 3.7+
- PyTorch
- tqdm
- matplotlib
- wandb

## Installation

1. Clone the repository:
bash
git clone https://github.com/IamSmokeY/Shakespeare-GPT.git
cd Shakespeare-GPT
2. Install the required packages:
bash
pip install -r requirements.txt

## Usage

1. Prepare your dataset:
    - Place your text file (e.g., `tinyShakesphere.txt`) in the project directory.

2. Run the training script:
bash
python gpt.py

3. The model will be trained and the generated text will be saved to `generated.txt`.

## Configuration

You can modify the model configuration in the `GPTConfig` class within the `gpt.py` file. Key parameters include:
- `vocab_size`
- `batch_size`
- `block_size`
- `n_embed`
- `n_heads`
- `n_layers`
- `dropout`
- `max_iters`
- `eval_interval`
- `lr`
- `eval_iters`

## Logging

The training process is logged using Weights & Biases (wandb). Make sure to set up your wandb account and configure the project name in the script.

## Visualization

The training and validation loss are plotted and displayed using matplotlib.

## Credits

This project is inspired by and based on the work of Andrej Karpathy.
