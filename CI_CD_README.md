# Credit Fraud Detection - CI/CD Pipeline

This project includes GitHub Actions for automated testing and deployment.

## Quick Start

1. Install dependencies:
```bash
pip install -r requirements.txt
```

2. Run tests:
```bash
pytest tests/ -v
```

3. Run local Gradio app:
```bash
python fraud_detection.ipynb
```

## CI/CD Pipeline

The pipeline runs on every push and PR to `main` and `develop` branches.

### Jobs:
- **Lint**: Code quality checks
- **Test**: Unit tests on Python 3.10, 3.11
- **Train**: Model training (requires AIML_Dataset.csv)

See `.github/workflows/ci-cd.yml` for full configuration.
