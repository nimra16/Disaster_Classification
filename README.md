# Aerial Disaster Image Classification: Comparative Analysis of Deep Learning Models

## Abstract

Timely and accurate classification of aerial images in post-flood scenarios is essential for effective disaster response. However, most existing deep learning models are limited by their reliance on binary classification tasks such as disaster vs no disaster. Furthermore, most existing studies utilize traditional model training approaches that require a high amount of data. These limitations hinder model generalization to diverse real-world conditions. In this study, we address these challenges by utilizing a benchmark dataset that contains drone images encompassing five classes: collapsed building, fire, flooded areas, normal, and traffic incident. The dataset consists of 6,432 images, carefully split into training, validation, and test sets for balanced evaluation. We conduct a comparative analysis of several deep learning models, including MobileNet, Inception, Xception, and ResNet-50. Experimental results demonstrate that MobileNet achieves the highest overall accuracy of 95% and consistently strong F1-scores across all classes, outperforming the other models. These findings highlight the effectiveness and suitability of lightweight deep learning architectures for robust aerial image classification in disaster management applications.

## Repository Structure

```
.
├── InceptionV3.ipynb
├── MobileNet.ipynb
├── preprocessing.ipynb
├── ResNet50.ipynb
├── test.ipynb
├── Xception.ipynb
└── Results/
    ├── AIDER dataset results.xlsx
    ├── mobilenet_confusion_matrix.png
    ├── mobilenet_training_accuracy.png
    └── mobilenet_training_loss.png
```

- **preprocessing.ipynb**: Data preparation and splitting.
- **MobileNet.ipynb**: MobileNet model training, evaluation, and results.
- **InceptionV3.ipynb**: InceptionV3 model training and evaluation.
- **Xception.ipynb**: Xception model training and evaluation.
- **ResNet50.ipynb**: ResNet-50 model training and evaluation.
- **Results/**: Visualizations, plots, and results summary (including the Excel file).

## Dataset

- **Source**: AIDER benchmark dataset (6,432 drone images)
- **Classes**: 
  - Collapsed building
  - Fire
  - Flooded areas
  - Normal
  - Traffic incident
- **Splits**: Training, validation, and test sets (see `preprocessing.ipynb` for details)

## Models Compared

- MobileNet
- InceptionV3
- Xception
- ResNet-50

## Key Findings

- **MobileNet** achieved the highest overall accuracy (95%) and strong F1-scores across all classes.
- Lightweight architectures like MobileNet are highly effective for aerial image classification in disaster management.

## How to Run

1. **Install dependencies**  
   Make sure you have Python 3.7+ and the required libraries:
   ```
   pip install tensorflow keras scikit-learn matplotlib seaborn
   ```

2. **Prepare the dataset**  
   - Place the AIDER dataset in the appropriate directory as referenced in the notebooks.
   - Run `preprocessing.ipynb` to split and preprocess the data.

3. **Train and evaluate models**  
   - Open and run the model notebooks (`MobileNet.ipynb`, `InceptionV3.ipynb`, `Xception.ipynb`, `ResNet50.ipynb`) in Jupyter or VS Code.

4. **View results**  
   - Plots, confusion matrices, and the summary Excel file are saved in the `Results/` directory.

## Results

Example: MobileNet confusion matrix and training curves are available in [Results/](Results/).

## Citation

If you use this code or dataset, please cite our paper (add citation here).

## License

This project is for academic research purposes. See [LICENSE](LICENSE) for details.

---
For questions or contributions, please open an issue or