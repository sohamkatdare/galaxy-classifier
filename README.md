# Galaxy Morphology Classifier

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.0+-red.svg)](https://pytorch.org/)

> A novel residual neural network architecture for autonomous classification of galaxy morphologies, trained on 300K+ galaxy images.

## Architecture

- **70+ layer** deep residual network with skip connections
- **Custom data augmentation** pipeline (rotation, flipping, color jitter) to handle galaxy orientation invariance
- **Efficient data loading** with prefetching and on-the-fly augmentation
- Convolutional feature extraction → residual blocks → classification head

## Results

| Metric | Value |
|--------|-------|
| Dataset Size | 300,000+ galaxy images |
| Architecture | Custom ResNet (70+ layers) |
| Parameters | ~2M |
| Training | GPU-accelerated with mixed precision |

## Quick Start

```bash
git clone https://github.com/sohamkatdare/galaxy-classifier.git
cd galaxy-classifier
pip install -r requirements.txt

# Train the model
python train.py --epochs 50 --batch-size 64

# Inference on a single image
python predict.py --image path/to/galaxy.jpg
```

## Project Structure

```
galaxy-classifier/
├── notebooks/          # Training and analysis notebooks
├── models/             # Model architecture definitions
├── data/               # Data loading and augmentation
├── train.py            # Training script
├── predict.py          # Inference script
├── requirements.txt
└── LICENSE
```

## Contributing

Contributions are welcome! See [CONTRIBUTING.md](CONTRIBUTING.md). Areas of interest:
- Alternative backbone architectures (EfficientNet, Vision Transformer)
- Multi-label classification (spiral arms, bars, rings)
- Model interpretability (Grad-CAM visualizations)
- ONNX export for deployment

## Citation

If you use this work in your research, please cite:
```bibtex
@software{katdare2024galaxy,
  author = {Katdare, Soham},
  title = {Galaxy Morphology Classifier},
  year = {2024},
  url = {https://github.com/sohamkatdare/galaxy-classifier}
}
```

## License

MIT License — see [LICENSE](LICENSE) for details.
