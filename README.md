# Fine-Tuning ALBERT for Question Answering (QA)

This repository fine-tunes ALBERT for Question Answering (QA) using Parameter-Efficient Fine-Tuning (PEFT) with LoRA and BitsAndBytes quantization.

## Features

- **ALBERT Fine-Tuning**: Adapts ALBERT for extractive QA tasks.
- **LoRA & BitsAndBytes**: Efficient training with low-rank adaptation and 4-bit quantization.
- **Dataset Preparation**: Uses the SQuAD dataset for training.
- **Training Pipeline**: Utilizes Hugging Face `Trainer` for efficient model training.
- **Evaluation**: Computes F1-score and exact match metrics for model performance.

## Files

1. **`FineTune_ALBERT_QA.ipynb`**: Python script implementing the training pipeline.
2. **Dataset**: SQuAD dataset for Question Answering tasks.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/AbdulrahmanAhmed20072/FineTune-ALBERT-QA.git
   ```
2. Install the required dependencies:
   ```bash
   pip install datasets bitsandbytes accelerate evaluate transformers torch peft numpy
   ```

## Usage

1. Load and preprocess the dataset.
2. Fine-tune ALBERT with LoRA and quantization.
3. Evaluate model performance.
4. Predict answers for new question-context pairs.

Run the script:
```bash
python FineTune_ALBERT_QA.ipynb
```

## Outputs

- Fine-tuned ALBERT model for Question Answering.
- F1-score and exact match evaluation on test data.
- Extracted answer predictions for given questions.

## Example

Context:
```
The sunset painted the sky orange and pink as a breeze rustled the leaves.
```

Question:
```
What colors were mentioned in the description of the sunset?
```

Predicted Answer:
```
orange and pink
```
