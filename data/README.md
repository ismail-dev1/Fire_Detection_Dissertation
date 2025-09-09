# Data layout (not included)

SYNFIRE_YOLOV8_SEG/
├── images/
│   ├── train/
│   ├── val/     # frozen
│   └── test/    # frozen
└── labels/
    ├── train/
    ├── val/
    └── test/

For the ResNet **presence** task:
- any **non-empty** `labels/<split>/<stem>.txt` → positive (fire present)
- empty/missing label file → negative
