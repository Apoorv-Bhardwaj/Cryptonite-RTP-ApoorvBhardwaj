# Fashion MNIST CNN

Test accuracy: 0.9106 (91.06%). This is a good result for a simple noisy dataset.

Test loss: 0.2403. Lower is better; this is consistent with ~91% accuracy.

Per-class highlights:

Very strong: Trouser (0.99 precision, 0.98 recall), Sandal, Bag, Ankle boot, Sneaker and shoe \& trouser classes are easy for the model.

Weaker: Shirt (precision 0.75, recall 0.71) which means model confuses shirts with other top classes (T-shirt/top, pullover, coat).

Macro averages: precision ≈ 0.9102, recall ≈ 0.9106, F1 ≈ 0.9102 which is consistent, not skewed by class imbalance (dataset is balanced).

GPU: Tesla T4; memory usage small (Allocated ~19 MB, Reserved ~46 MB) which is indicates the model is lightweight and not saturating the GPU. You can safely increase batch size or move to a larger model for transfer learning.



\# CNN



Full fine-tuning achieved substantially higher accuracy than partial fine-tuning, as updating all layers allowed the model to better adapt pretrained features to the specific characteristics of the DeepWeeds dataset. Full fine-tuning significantly outperformed partial fine-tuning, demonstrating that adapting the entire network is crucial for achieving high performance on the DeepWeeds dataset. While partial fine-tuning is computationally cheaper, it limits the model’s ability to learn domain-specific visual features.

