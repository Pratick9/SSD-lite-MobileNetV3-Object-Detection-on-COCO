# SSD-lite MobileNetV3 Object Detection on COCO (Kaggle Notebook)

This project demonstrates building, training, and evaluating an **SSD-lite MobileNetV3 object detection model** on the COCO 2017 dataset — all implemented in a single Kaggle notebook.

---

## Project Overview

- Backbone: MobileNetV3 (lightweight CNN)
- Detection Head: SSD-lite (Single Shot MultiBox Detector lite)
- Dataset: COCO 2017 (filtered 50% subset for faster experimentation)
- Framework: PyTorch and torchvision
- Evaluation: COCO metrics (mAP, precision, recall, per-class AP)
- Visualization: Detection results with bounding boxes and confidence scores

---

## How to Use

1. Open the notebook `ssd_mobilenetv3_coco.ipynb` on Kaggle.
2. Make sure COCO 2017 dataset (validation images and annotations) is uploaded or linked as Kaggle dataset.
3. Run all notebook cells sequentially:
   - Data loading and filtering
   - Model training (default 5 epochs on 50% data)
   - Model evaluation with COCO API
   - Visualization of sample detections

---

## Key Features

- Efficient dataset filtering to avoid errors from images without annotations
- Training loop with pretrained SSD-lite MobileNetV3 weights for quick fine-tuning
- Full COCO evaluation with rich metrics output and per-class breakdown
- Clear visualization aiding qualitative analysis

---

## Notes

- The notebook uses a subset of the COCO dataset (10%) to reduce runtime and resource usage.
- For better results, consider extending training epochs or using the full dataset.
- Make sure to adjust dataset paths if running outside Kaggle.

---

## License

This notebook and code are released under the MIT License.

---

## Acknowledgments

- PyTorch and torchvision teams for excellent model and dataset utilities
- COCO dataset creators and maintainers
- pycocotools for evaluation tools

---

Feel free to fork, modify, and extend the notebook for your projects or learning.

