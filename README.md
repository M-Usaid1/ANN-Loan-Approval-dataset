# ANN-Insurance-dataset-
1. No Overfitting

Train and val losses were nearly identical (0.147 vs 0.146) during training — the model generalized well without memorizing the training data.
2. Strong Test Accuracy (96.14%)

On completely unseen data the model correctly predicted 96 out of 100 cases. Very solid for a basic ANN with no BatchNorm or Dropout.
3. Balanced Precision & Recall

Both classes hit 0.96 precision — the model isn't biased toward predicting one class over the other despite the 62/38 imbalance in the dataset.
4. Slight Recall Drop on Rejected Class (0.94 vs 0.97)

The model misses a few rejected cases — meaning some applicants who should be rejected get predicted as approved. In a real lending scenario this would be the main area to improve.
5. F1-Score is Consistent

0.97 for Approved and 0.95 for Rejected — the macro average of 0.96 confirms the model performs reliably across both classes, not just the majority one.
6. Simple Architecture Was Enough

Just 3 Dense layers (16 → 32 → 64) without any regularization achieved 96% — this suggests the dataset is clean and well-structured, and the features (especially CIBIL score) are highly informative.
