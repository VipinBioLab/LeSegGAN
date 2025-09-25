# LeSegGAN: A Hybrid Attention-Based GAN for Accurate Lesion Segmentation

## Overview
Accurate segmentation of skin lesions is critical for the early detection of melanoma and other skin cancers. Traditional deep learning methods (CNNs, transformers) face limitations in capturing both local and global contextual features, handling irregular lesion boundaries, and maintaining robustness against common artifacts such as hair, shadows, and illumination variations.

**LeSegGAN** is a novel hybrid attention-enhanced **Generative Adversarial Network (GAN)** framework designed to address these challenges. It integrates convolutional and inception modules with residual connections and channel attention in the generator, while employing a **Vision Transformer (ViT)-based discriminator** for improved segmentation accuracy through adversarial learning.

## Key Features
- **Hybrid Generator**: Combines convolution, inception, residual connections, and channel attention for rich multi-scale feature extraction.
- **ViT-based Discriminator**: Incorporates transformer-based global attention for better adversarial learning.
- **Composite Loss Function**: Weighted Binary Cross-Entropy + Dice Loss + Focal Loss to handle class imbalance and enhance performance.
- **Benchmark Evaluation**: Tested on four widely used datasets:
  (**NOTE:** All images will be uploaded after final acceptance of the manuscript)
  - Waterloo Skin Cancer
  - MED-NODE
  - SD-260
  - ISIC-2016
- **Superior Performance**: Outperforms state-of-the-art models (U-Net, U-Net++, SegNet, FCN, DTP-Net) in both accuracy and IoU metrics.

## Results
| Dataset              | Accuracy | IoU    |
|-----------------------|----------|--------|
| Waterloo Skin Cancer  | 0.9943   | 0.9451 |
| MED-NODE              | 0.9759   | 0.9664 |
| SD-260                | 0.9873   | 0.8709 |
| ISIC-2016             | 0.9724   | 0.7717 |

LeSegGAN consistently demonstrates strong generalization ability and robustness across diverse datasets.

## Installation
Clone this repository and install the required dependencies:
```bash
git clone https://github.com/your-username/LeSegGAN.git
cd LeSegGAN
pip install -r requirements.txt
```

## Citation
If you find this work useful in your research, please cite it as follows:
```bash
@article{LeSegGAN2025,
  title   = {LeSegGAN: A Hybrid Attention-Enhanced GAN for Accurate Lesion Segmentation in Dermatological Images},
  author  = {Kar, Mithun Kumar and Venugopal, Vipin and Anoop, B. N.},
  journal = {IEEE Access (submitted)},
  year    = {2025}
}
```

