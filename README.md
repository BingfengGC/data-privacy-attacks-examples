# Examples of Data Privacy Attacks

The repo contains a set of examples for common types of data privacy attacks applied to trained models in a black box setting, that are relevant to the Energy sector.

We use two main packages (https://github.com/Trusted-AI/adversarial-robustness-toolbox)[IBM Adversial Toolbox] and (https://www.tensorflow.org/responsible_ai/privacy/guide)[Tensorflow Privacy]

There are two notebooks in this repos:

1. MiscDataPrivacyAttackExamples.ipynb
    - Reconstruction/Attribute attacks example with MNIST OCR example with the MI Face algorithm using IBM ART
    - Model Extraction example with MNIST OCR - CopyCNN algorithm using IBM ART
    - Model Leakage attack with synethic household smart meter data using the SVM linear classifer
    - Property Inference Attack with synethic household smart meter data (with high vs low tariff labels) with using the Random Forest Classifier model
        - We're trying to extract the high vs low tariff ratio with this property inference attack
1. TensorFlowPrivacyTest_Full_Flow.ipynb
    - CNN EuroSAT model without privacy attack protection (with privacy vulnerability report to Membership Inference attacks)
       - Implements Membership Inference Attack as a Privacy Attack
    - CNN EuroSAT model with Differential privacy protection (with privacy vulnerability report to Membership Inference attacks)

## Install dependencies

Run the following command in your Python virtual environment to install relevant dependencies

```
pip install -r requirements.txt
```