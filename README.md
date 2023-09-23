# **Fintech Bootcamp Module 13 Homework Assignment - Deep Learning**
### **Darcy Davis**
---

### **Introduction**
Risk management is pivotal for venture capital firms. This project leverages the capabilities of deep learning to assist Alphabet Soup, a venture capital firm, in its decision-making process. By analyzing data from over 34,000 organizations funded by Alphabet Soup, we aim to craft a model that predicts the success of startup applications.

### **Objective**
Construct a neural network model to predict the likelihood of startups achieving success when funded by Alphabet Soup.

### **Dataset**
The dataset encompasses details of over 34,000 organizations, shedding light on various facets of each business, including their success trajectory.

### **Model Evolution & Results**

1. **Original Model**: 
   - Compiled using the binary cross-entropy loss function, the Adam optimizer, and accuracy as the evaluation metric.
   - **Loss**: 0.5545
   - **Accuracy**: 72.72%
   
2. **Alternative Model 1**: 
   - Removed "CLASSIFICATION" and "APPLICATION_TYPE" from the dataset.
   - Retained 2 hidden layers.
   - Abided by the 2/3 rule of thumb.
   - Trained with 50 epochs.
   - **Loss**: 0.5714
   - **Accuracy**: 72.26%
   
3. **Alternative Model 2**: 
   - Incorporated dropout layers and regularization.
   - Reduced the number of hidden neurons per layer.
   - **Loss**: 0.5886
   - **Accuracy**: 72.27%
   
4. **Alternative Model 3**:
   - Assessed dataset balance and then undersampled the majority class.
   - Excluded regularization and dropout layers.
   - **Loss**: 0.5822
   - **Accuracy**: 72.52%

### **Conclusion**
Unfortunately, making changes to the neural network, including dropping feature columns, introduction regularisation, reducing the hidden number of neurons; as well as undersampling to create balanced classes did not yield significant changes in accurracy.

---

**Note**: For an in-depth walkthrough, refer to the [accompanying Jupyter Notebook](venture_funding_with_deep_learning.ipynb): `venture_funding_with_deep_learning.ipynb`.

---

### **Tools & Libraries**
- **Pandas**: Data manipulation and analysis.
- **Scikit-learn**: Data preprocessing and model evaluation.
- **TensorFlow & Keras**: Neural network model construction, compilation, and optimization.

---

### **Author**
Darcy Davis

---

**Last Updated**: September 23rd, 2023

---

This README offers a snapshot of the Jupyter Notebook. For thorough explanations, code implementations, and analyses, please consult the notebook directly.
