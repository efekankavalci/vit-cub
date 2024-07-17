# Fine Grained Image Classification with Vision Transformers

This project focuses on applying Vision Transformers (ViT) to fine-grained image classification tasks using the CUB-200-2011 dataset. The objective is to explore different fine-tuning strategies and visualize how attention mechanisms in ViTs contribute to image classification.

## Project Structure

- **Dataset**: Utilizes the CUB-200-2011 dataset, accessible via [Huggingface Hub](https://huggingface.co/datasets/efekankavalci/CUB_200_2011).
- **Preprocessing**: Images are preprocessed and augmented to enhance the model's ability to generalize. Augmentations include random horizontal flips, color jitter, and random affine transformations.
- **Model Training**: Various training setups are experimented with, including using static feature extractors, fine-tuning specific layers, and training entire models.
- **Visualization**: Attention maps are visualized to understand the model's focus areas during classification.

## Methods

1. **Static Feature Extractor**: ViT models pre-trained on ImageNet are used as feature extractors.
2. **Fine-tuning**: Fine-tuning is performed on:
    - Last encoder block
    - All attention layers
    - Full architecture
3. **Attention Visualization**: Raw attention maps and attention rollout technique are used to visualize which parts of the image influence the classification decision.

