## Structure

```text
benchmark_v2/
  datasets/   Local datasets, extracted archives, and Hugging Face caches
  registry/   JSON registries for benchmark runs, metrics, configs, and checkpoints
  train/      Training scripts and configuration files
  models/     Model definition files
  zoo/        Trained model checkpoints
  collect/    Collected checkpoint trajectories
```

## Tasks

- Image classification
- Text classification
- Image segmentation
- LLM Adaptation
- Reinforcement learning

The main registry files are:

```text
registry/image_classification.json
registry/text_classification.json
registry/image_segmentation.json
registry/reinforcement_learning.json
```

## Artifacts

- Trained checkpoints: `zoo/**/*.pth`
- Collected checkpoints: `collect/**/*.pth`
- Training configs: `train/**/config/*.json`
- Model code: `models/*.py`

## Datasets

This benchmark uses or caches several public research datasets, including CIFAR-10, CIFAR-100, MNIST, SVHN, STL-10, Tiny ImageNet, PASCAL VOC 2012, Oxford-IIIT Pet, ISIC 2018 Task 1, SST-2, AG News, IMDB, GoEmotions, Yelp Review Full, Acrobot-v1, and LunarLander-v3.

Third-party datasets, pretrained models, and cached assets retain their original licenses and terms of use. Before public release, verify which assets can be redistributed and replace non-redistributable files with download instructions or scripts.

