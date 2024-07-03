## SymptomDiagnoser
<div align="center">
  <img src="https://github.com/HassanKhalil321/SymptomDiagnoser/blob/main/assets/Screenshot%202024-07-03%20144152.jpg" width="1000"/>
</div>


## Introduction
SymptomDiagnoser is a machine learning project aimed at classifying diseases based on symptoms. This tool leverages advanced algorithms to analyze patient-reported symptoms and provide a probable diagnosis, assisting healthcare professionals and patients in identifying potential medical conditions quickly and accurately.



## Dataset
The dataset used in SymptomDiagnoser is a crucial component of the project. Originally, the dataset contained information on 1100 diseases. However, to ensure the highest quality and reliability of our model, we carefully selected a subset of 510 diseases. This subset was chosen based on the following criteria:

## Model 

- **Text Vectorization**: The input text describing symptoms is converted into a numerical format using a text vectorization layer. This process transforms words into vectors, making them suitable for machine learning algorithms.

- **Embedding Layer**: The vectorized text is then passed through an embedding layer. This layer captures semantic relationships between words by converting them into dense vectors of fixed size, which helps in understanding the context of symptoms.

- **Global Average Pooling 1D**: The embedded vectors are aggregated using a global average pooling 1D layer. This layer reduces the dimensionality by averaging the elements along the time dimension, highlighting the most relevant features and reducing overfitting.

- **Dense Layer and Dropout**: The pooled features are fed into a dense (fully connected) layer, followed by a dropout layer. The dense layer applies a non-linear transformation to the input, and the dropout layer randomly sets a fraction of input units to zero during training to prevent overfitting.

- **Dense Layers**: Finally, the output from the previous layer is passed through two additional dense layers. These layers further process the features and produce the final output, which is the predicted disease based on the input symptoms.

## Loss
<div align="center">
  <img src="https://github.com/HassanKhalil321/SymptomDiagnoser/blob/main/assets/CCE.jpg" width="500"/>
</div>

## Results
<div align="center">
  <img src="https://github.com/HassanKhalil321/SymptomDiagnoser/blob/main/assets/ppp.png" width="600" hight='500'/>
</div>
