# Network-Intrusion-Detection-System-NIDS-


Network Intrusion Detection System (NIDS)
Security Analytics using Machine Learning & Deep Learning

This repository features a robust Network Intrusion Detection System designed to identify and classify cyber threats in real-time. By leveraging advanced oversampling techniques and Deep Learning architectures, this system overcomes the common "needle in a haystack" problem—class imbalance in network traffic data.


To make your GitHub README more visually engaging and professional, you can use specific emojis to represent each dataset's unique role in your project.

Here is the updated Datasets section for your README:
📊 Datasets Used

I evaluated the system across three benchmark datasets, representing different eras and complexities of network security.
🏛️ NSL-KDD (The Benchmark)

Description: A refined version of the classic KDD Cup '99 dataset. It removes redundant records to prevent classifier bias.

Key Challenge: Severe class imbalance, especially in U2R (User-to-Root) and R2L (Remote-to-Local) attacks.

Use Case: Ideal for testing the effectiveness of SVM-SMOTE in defining clear boundaries for rare attacks.

🛡️ UNSW-NB15 (The Hybrid)

Description: Created in a controlled environment to reflect modern network traffic and low-footprint attack patterns.

Key Challenge: Contains 9 attack categories (e.g., Fuzzers, Backdoors, Worms) that mimic contemporary synthetic threats.

Use Case: Used to validate the model's ability to generalize across diverse, modern attack signatures.

🌐 CIC-IDS2017 (The Gold Standard)

Description: High-fidelity data capturing real-world network flows (HTTP, HTTPS, SSH) and human-like background traffic.

Key Challenge: Massive dimensionality (80+ features) and realistic extreme imbalance (e.g., Heartbleed attack).

Use Case: The primary test for our Deep Learning models and KMeans-SMOTE clustering for high-dimensional synthetic data generation.

⚖️ Data Balancing Strategy


🔍 KMeans-SMOTE: Used to cluster the majority class and generate synthetic minority samples in safe areas to avoid noise.

📈 SVM-SMOTE: Applied to focus specifically on the "danger zone" near the decision boundary.

