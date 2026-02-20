# Behavioral Anomaly Segmentation  
PCA + Gaussian Mixture Modeling Framework  
I compared probabilistic clustering with density-based anomaly detection to evaluate behavioral outlier consistency across modeling assumptions.
---

## Overview

This project implements an unsupervised behavioral segmentation framework using Principal Component Analysis (PCA) and Gaussian Mixture Models (GMM).

The objective is to identify structured behavioral patterns and detect probabilistic anomalies in high-dimensional interaction data.

Rather than relying on labeled outcomes, this approach models latent structure within engagement behavior to uncover:

- Dominant behavioral clusters  
- Mixed-membership interaction profiles  
- Overlapping probabilistic segments  
- High-variance behavioral outliers  

This framework is applicable to cybersecurity (user behavior analytics), fraud detection, risk modeling, and anomaly detection environments.

---

## Methodology

### Dimensionality Reduction — PCA

High-dimensional interaction variables were reduced using PCA to:

- Preserve dominant variance structure  
- Identify engagement intensity axes  
- Detect compositional behavior differences  

The first principal component captures overall intensity.  
The second component captures interaction structure differences.

---

### Probabilistic Clustering — Gaussian Mixture Models

Gaussian Mixture Models (GMM) were applied for soft clustering.

This allows:

- Probabilistic segment membership  
- Identification of hybrid behavior  
- Detection of overlapping clusters  
- More realistic behavioral modeling compared to hard clustering  

Posterior probability distributions were analyzed to detect anomaly-like behavior patterns.

<img width="703" height="547" alt="GMMclusters" src="https://github.com/user-attachments/assets/4150ff84-212b-4516-a782-942d052082f5" />


## Isolation Forest Comparison

To compare clustering-based segmentation with density-based anomaly detection, Isolation Forest was applied to the same feature space.

This provides an alternative perspective on behavioral outliers under a different modeling assumption.

<img width="703" height="547" alt="IsolationForestAnomalyDetection" src="https://github.com/user-attachments/assets/c4c6f269-fb2b-494d-abdc-9805b8859141" />


---

## Technologies

Python · scikit-learn · pandas · numpy · matplotlib  

---

## Future Extensions

- Isolation Forest anomaly comparison  
- DBSCAN density-based clustering  
- Application to cybersecurity log datasets  
- Temporal behavioral drift modeling  

---

## Author

Regina  
Cybersecurity & Risk Analytics  
