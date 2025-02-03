# Products-Recommender-System-using_PySpark-OpenAI

---
## Introduction
The goal of this project is to:

1. Process and analyze large-scale product and user interaction data using PySpark.

2. Build a recommender system using collaborative filtering and k-means clustering.

3. Generate personalized product recommendations using OpenAI.

4. Visualize product clusters and evaluate the recommender system's performance.

---

## Step-by-Step Workflow
### **1️⃣ Importing Necessary Libraries**
- PySpark: For distributed data processing.

- Pandas and NumPy: For data manipulation and analysis.

- (paid) OpenAI: For generating personalized recommendations.(paid)
- (free) SentenceTransformer: Vector Embedding

- Matplotlib and Plotly: For data visualization.

### **2️⃣ Loading Data with PySpark**
- Load the dataset into a PySpark DataFrame.

- Perform initial data exploration.

### **3️⃣ Data Preprocessing**
- Combine product titles and descriptions into a single column for text processing.

- Convert the combined text into a list for further processing.

### **4️⃣ Text Embedding with sentence_transformers/OpenAI**
- (paid) Use OpenAI's text-embedding-3-small model to convert text into numerical embeddings.
- - (free) Use sentence_transformers all-MiniLM-L6-v2 model to convert text into numerical embeddings.

- Store embeddings in a PySpark DataFrame.

### **5️⃣ Clustering Products with K-Means**
- Use k-means clustering to group similar products based on their embeddings.

- Determine the optimal number of clusters using the Elbow Method and Silhouette Score.



### **6️⃣ Visualizing Product Clusters**
- Use PCA to reduce the dimensionality of embeddings for visualization.

- Plot the clusters in a 2D space using Plotly.

### **7️⃣ Generating Recommendations**
- Identify recently viewed products and their corresponding clusters.

- Recommend similar products from the same clusters.

### **8️⃣ Displaying Recommendations**
- Display the recommended products based on the user's recently viewed items.  

### **🚀 Live Demo**
You can explore the live demo of this project here:
Open In Colab
Link:

### **Future Scope**
Incorporate user demographics and product categories for more personalized recommendations.

Fine-tune hyperparameters for improved clustering accuracy.

Experiment with alternative recommendation algorithms (e.g., matrix factorization, deep learning models).

### **License**
This project is licensed under the MIT License.

### **Contributing**
Contributions are welcome! Fork the repository and submit pull requests with improvements.
