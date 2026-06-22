# Contributing to Galaxy Classifier

Thank you for your interest in contributing to this deep learning galaxy morphology classifier!

## Getting Started

1. Fork and clone: `git clone https://github.com/<you>/galaxy-classifier.git`
2. Create a virtual environment: `python -m venv venv && source venv/bin/activate`
3. Install dependencies: `pip install -r requirements.txt`
4. Download the dataset (see README for instructions)

## How to Contribute

- **Model improvements** — New architectures, hyperparameter tuning, training strategies
- **Data augmentation** — Additional augmentation techniques for galaxy images
- **Documentation** — Improved explanations of architecture decisions, training curves
- **Visualization** — Better tools for inspecting model predictions and attention maps
- **Benchmarking** — Comparisons against other galaxy classification approaches

## Pull Request Guidelines

1. Create a descriptive branch: `git checkout -b improve/residual-block`
2. Include training metrics or visualizations if changing the model
3. Document any new dependencies in `requirements.txt`
4. Keep notebooks clean (clear outputs before committing)

## Code Style

- Follow PEP 8
- Use type hints for function signatures
- Document model architecture changes in the README

## License

By contributing, you agree that your contributions will be licensed under the MIT License.
