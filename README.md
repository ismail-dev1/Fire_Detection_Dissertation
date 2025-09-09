# Fire Detection on SYNFire (Dissertation)

This repo contains code and **results** (no large weights) for:
- **YOLOv8 (segmentation)** on SYNFire
- **ResNet18 (fire presence)** on SYNFire

## Structure
- `notebooks/` – Colab notebooks used for training/eval
- `results/`
  - `resnet/` – CSV/JSON/plots for ResNet runs
  - `yolo_runs/<run>/` – Ultralytics per-run plots + metrics (no weights)
- `config/` – dataset YAMLs and configs
- `requirements.txt`, `env_info.txt` – environment snapshot
