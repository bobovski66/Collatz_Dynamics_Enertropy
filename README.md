# Collatz Dynamics Through Entropy and Energy

This project explores the behavior of the Collatz map using entropy, 2-adic valuation, and dynamic analysis tools from data science and topology. The study uses delay embeddings, tracks 2-adic flows, projects dynamics via UMAP, clusters trajectories with HDBSCAN, and visualizes energetic and informational features of the sequences.

---

## 🧠 Key Concepts

- **2-adic valuation**: Represents an energy landscape that guides the Collatz sequence's behavior.
- **Shannon entropy**: Applied to ν₂ distributions to measure the uncertainty and randomness in the sequences.
- **Delay embeddings**: Revealing structure from the values and ν₂, allowing us to explore the dynamics in higher dimensions.
- **UMAP**: A method for dimensionality reduction that projects the high-dimensional dynamics into a lower-dimensional space.
- **HDBSCAN**: A density-based clustering algorithm used to identify clusters within the dynamic Collatz sequences.

---

## 🔬 Exploratory Visuals

### 🔁 Animated Collatz Dynamics

**2-adic Valuation Delay Embedding (n = 27)**  
This animated GIF shows the 2-adic valuation dynamics of the Collatz sequence for \(n = 27\) as it evolves over time. The 3D delay embedding captures the shifts in valuation through the trajectory steps.  
![2-adic Delay Embedding Animation](images/nu2_3d_delay_embedding_n_27_animated.gif)

**Raw Value Delay Embedding (n = 27)**  
Here is the animated 3D delay embedding of the raw values of the Collatz sequence for \(n = 27\). The animation illustrates the shifting raw values over the trajectory's time steps.  
![Raw Value Delay Embedding Animation](images/raw_values_3d_delay_embedding_n_27_animated.gif)

### 🧭 UMAP Projections & Clustering

UMAP projections of different embeddings, colored by HDBSCAN cluster:

- **Raw Values**  
  A projection of the Collatz sequence’s raw values in a lower-dimensional space using UMAP. This visualization captures the spread of values over time, with each point representing a different sequence step.  
  ![](images/umap_value_embedding.png)

- **2-adic Valuation (ν₂)**  
  This UMAP projection shows the behavior of the 2-adic valuation (ν₂) over the Collatz sequence steps, revealing how the energy landscape evolves during the sequence.  
  ![](images/umap_nu2_embedding.png)

- **Fused Energy + Trajectory Embedding**  
  A combined representation of the energy (2-adic valuation) and the raw trajectory values of the Collatz sequence, allowing for a more nuanced understanding of how these elements interact over time.  
  ![](images/umap_fused_embedding.png)

Clustered with HDBSCAN:

- **Fused Clusters**  
  Clusters identified using HDBSCAN from the fused energy and trajectory embedding. This clustering method groups similar sequences together based on their UMAP projection.  
  ![](images/hdbscan_fused_clusters.png)

- **ν₂ Clusters**  
  Clusters based on the 2-adic valuation (ν₂) sequences, highlighting patterns in how different parts of the trajectory exhibit similar energy behaviors.  
  ![](images/hdbscan_nu2_clusters.png)

- **Value Clusters**  
  Clusters derived from the raw value sequences, revealing how different values in the trajectory group based on their behavior.  
  ![](images/hdbscan_value_clusters.png)

---

## 🧵 Delay Embeddings (3D)

The 2-adic valuation dynamics of the Collatz sequence for \(n = 27\) represented in a 3D delay embedding, capturing shifts in the ν₂ values as the sequence evolves.

- **ν₂ (2-adic Valuation) Delay Embedding (n = 27)**  
  This image shows the 3D delay embedding of the 2-adic valuation (ν₂) for \(n = 27\), visualizing the energy dynamics across steps of the sequence.  
  ![](images/nu2_3d_delay_embedding_n_27.png)

---

## ⚡ Energy & Entropy Dynamics

Entropy measures the uncertainty in the system. Here we show the stepwise entropy change based on the 2-adic valuation.

- **Stepwise Entropy (Shannon Entropy)**  
  This plot shows how the Shannon entropy of the ν₂ distribution changes over the Collatz steps. It gives insight into the unpredictability of the sequence based on its energy landscape.  
  ![](images/stepwise_shannon_entropy.png)

- **Histogram of ν₂ (2-adic Valuation) Shannon Entropy**  
  A histogram of the 2-adic valuation (ν₂) over the entire trajectory of \(n = 27\), showing the distribution of entropy across different steps.  
  ![](images/nu2_shannon_entropy.png)

---

## 📈 Sample Trajectories by Cluster

Each cluster has distinct energy signatures. These plots show the trajectory paths for different clusters, highlighting the values and 2-adic valuation dynamics over time.

- **Cluster 0**  
  A sample trajectory for \(n = 63\), showing both the raw values and the ν₂ over the sequence.  
  ![](images/trajectory_cluster_0_n_63.png)

- **Cluster 1**  
  Sample trajectories for \(n = 21\), revealing the energy flow and the raw values' path through time.  
  ![](images/trajectory_cluster_1_n_21.png)

- **Cluster 2**  
  Sample trajectories for \(n = 88\) and \(n = 92\), with their respective raw values and 2-adic valuations.  
  ![](images/trajectory_cluster_2_n_88.png)  
  ![](images/trajectory_cluster_2_n_92.png)

- **Cluster 3**  
  A trajectory for \(n = 58\), showing the evolution of the raw values and the ν₂ throughout the sequence.  
  ![](images/trajectory_cluster_3_n_58.png)

- **Cluster 4**  
  A trajectory for \(n = 37\), visualizing the changes in the raw values and 2-adic valuation.  
  ![](images/trajectory_cluster_4_n_37.png)

- **Cluster 5**  
  A trajectory for \(n = 87\), capturing the path through the trajectory and 2-adic energy changes.  
  ![](images/trajectory_cluster_5_n_87.png)


---

## 🧙‍♂️ Built With Curiosity

This project explores the Collatz conjecture as a dissipative system where energy flows and entropy changes reflect the underlying structure of number theory. The study takes a deep dive into the mathematical and informational properties of the sequence.

> Everything goes to 1... but how?


