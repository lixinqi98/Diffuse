# Denosing Diffusion Generative Models

## Requirements

To install requirements:

```setup
pip install -r requirements.txt
```

## Training Diffusion Models

To train a diffusion model, first specify model architecture and hyperparameters in `config.json`. Once specified, run this command:

```train
python diffusion_lightning.py --train --config config.json --n_gpu NUM_AVAIL_GPUS
```

## Sample Generation

To generate samples from a trained diffusion model specified by `config.json`, run this command:

```eval
python diffusion_lightning.py --config config.json --model_dir MODEL_DIRECTORY --sample_dir PATH_TO_SAVE_SAMPLES --n_samples NUM_SAMPLES
```
