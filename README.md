# FGSM-Adversarial_Robustness
Auditing Neural Network Robustness using FGSM Adversarial Attacks
Auditing Neural Network Robustness via FGSM Adversarial Attacks

Project Overview

This project investigates the robustness of a Convolutional Neural Network (CNN) against Fast Gradient Sign Method (FGSM) adversarial attacks.

The model is trained on the MNIST handwritten digit dataset. FGSM attacks are then applied with different epsilon values to study how small input perturbations affect model performance.

Technologies Used

- Python
- PyTorch
- Torchvision
- NumPy
- Pandas
- Matplotlib
- Google Colab

Dataset

MNIST Handwritten Digit Dataset:

- 60,000 training images
- 10,000 testing images
- 10 digit classes (0–9)

Experimental Results

The CNN achieved 99.02% accuracy on clean test images.

Epsilon| Accuracy
0.00| 99.02%
0.05| 95.56%
0.10| 84.50%
0.15| 63.08%
0.20| 36.88%
0.25| 20.13%
0.30| 12.57%
### Accuracy vs FGSM Epsilon

![Accuracy Graph](accuracy_vs_epsilon.png)

### Attack Success Rate vs FGSM Epsilon

![ASR Graph](asr_vs_epsilon.png)

Key Findings

- The model achieved high accuracy on clean images.
- Increasing epsilon reduced classification accuracy.
- FGSM attacks became more successful as perturbation strength increased.
- At epsilon 0.30, the attack success rate reached approximately 87.31%.

Project Files
## Project Files
- `FGSM_Adversarial_Robustness.ipynb` – Complete project implementation.
- `fgsm_results.csv` – Experimental results.
- `accuracy_vs_epsilon.png` – Model accuracy graph.
- `asr_vs_epsilon.png` – Attack success rate graph.
- `fgsm_cnn_model.pth` – Trained CNN model weights.
- `requirements.txt` – Required Python libraries.

Conclusion

This experiment demonstrates that even a highly accurate neural network can be vulnerable to adversarial perturbations. It highlights the importance of evaluating and improving the robustness of deep learning models.

---

Project Domain: Artificial Intelligence | Deep Learning | Adversarial Machine Learning
