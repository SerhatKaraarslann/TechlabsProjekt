# TechlabsProjekt
Automated Lung Disease Diagnosis with CNN-Based X-Ray Analysis 

A deep learning system for detecting 14 lung diseases from chest X-rays using EfficientNetB0 and ResNet50 architectures. Achieves 85% training/validation accuracy with class-imbalance mitigation strategies. 

Project Highlights 

    Multi-Disease Detection: Classifies 14 pathologies + "No Finding" 

    Imbalanced Data Handling: Log-scaled class weights & weighted loss 

    Hardware-Efficient: Optimized for local training (4/10 data packages used) 

    Model Comparison: Direct benchmark between EfficientNetB0 vs. ResNet50 

    Planned Features: Custom ConvNet, interactive visualizations 

Dataset Overview 

NIH Clinical Center Chest X-Ray Dataset 

    100,000+ frontal-view X-rays (30,000+ used) 

    15 classes (14 diseases + "No Finding") 

    Key Challenge:  

    Extreme class imbalance (Hernia: 0.25% vs No Finding: 58%) 

    Grayscale images stored as RGB 

Model Architecture 

Two-Stream Approach 

    EfficientNetB0 Base 

    Pretrained on ImageNet (first 150 layers frozen) 

    Custom head with Conv2D/ReLU layers 

    Softmax output (15 neurons) 

    ResNet50 Comparison 

    Same classification head 

    Identical training protocol 

Training Specs 

    Optimizer: Adam w/ learning rate scheduler 

    Loss: Weighted Categorical Cross-Entropy 

    Batch Size: 32-64 (local GPU constraints) 

Performance Comparison 

![grafik](https://github.com/user-attachments/assets/fce8c888-5c65-4d1b-8e60-bfc3487cc4d0)

Geplante Updates  

    Code Refactoring (In Progress) 

    Custom ConvNet Training 

    full dataset training 

 
