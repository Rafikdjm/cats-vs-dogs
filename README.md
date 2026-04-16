# Cats vs Dogs — CNN Classifier 

Binary image classification using a custom CNN built with TensorFlow/Keras,  
trained on the Kaggle Dogs vs. Cats dataset (~25 000 images).

## Results
| Metric | Value |
|---|---|
| Val Accuracy | ~82% |
| Epochs | 50 |
| Image size | 150×150 |

## Model architecture
- 3× Conv2D + MaxPooling blocks (32 → 64 → 128 filters)
- Dropout (0.5) + Dense (512) + Sigmoid output
- Optimizer: Adam (lr=1e-4), Loss: Binary Crossentropy

## Dataset
[Kaggle Dogs vs. Cats](https://www.kaggle.com/c/dogs-vs-cats)  
~25 000 images — 80/20 train/val split

## Run
```bash
pip install -r requirements.txt
jupyter notebook cats_vs_dogs.ipynb
```

> ⚠️ Images not included (too large). Download the dataset from Kaggle.
