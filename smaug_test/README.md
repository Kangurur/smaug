---
library_name: peft
license: apache-2.0
base_model: distilbert-base-uncased
tags:
- generated_from_trainer
metrics:
- accuracy
model-index:
- name: smaug_test
  results: []
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# smaug_test

This model is a fine-tuned version of [distilbert-base-uncased](https://huggingface.co/distilbert-base-uncased) on an unknown dataset.
It achieves the following results on the evaluation set:
- Loss: 0.7087
- Accuracy: {'accuracy': 0.7}

## Model description

More information needed

## Intended uses & limitations

More information needed

## Training and evaluation data

More information needed

## Training procedure

### Training hyperparameters

The following hyperparameters were used during training:
- learning_rate: 5e-05
- train_batch_size: 4
- eval_batch_size: 4
- seed: 42
- optimizer: Use OptimizerNames.ADAMW_TORCH with betas=(0.9,0.999) and epsilon=1e-08 and optimizer_args=No additional optimizer arguments
- lr_scheduler_type: linear
- num_epochs: 4

### Training results

| Training Loss | Epoch | Step | Validation Loss | Accuracy          |
|:-------------:|:-----:|:----:|:---------------:|:-----------------:|
| No log        | 1.0   | 50   | 0.6790          | {'accuracy': 0.7} |
| No log        | 2.0   | 100  | 0.6772          | {'accuracy': 0.7} |
| No log        | 3.0   | 150  | 0.6935          | {'accuracy': 0.7} |
| No log        | 4.0   | 200  | 0.7087          | {'accuracy': 0.7} |


### Framework versions

- PEFT 0.13.2
- Transformers 4.46.3
- Pytorch 2.5.1+cu118
- Datasets 3.1.0
- Tokenizers 0.20.3