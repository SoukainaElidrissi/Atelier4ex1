# PyTorch Lab: Autoencoder and Variational Autoencoder (VAE) with MNIST Dataset



## Work Done:

###  Autoencoder (AE) VS Variational Autoencoder (VAE)

1. **Autoencoder (AE)**
   - Establish an autoencoder architecture and train the model on the MNIST dataset.
   - Specify the best hyperparameters for training.

2. **Variational Autoencoder (VAE)**
   - Establish a variational autoencoder architecture and train the model on the MNIST dataset.
   - Specify the best hyperparameters for training.

3. **Evaluation:**
   - Evaluate both models by plotting loss, KL divergence, and other relevant metrics.
   - Draw conclusions based on the evaluation results.

4. **Latent Space Visualization:**
   - Plot the latent space representations of both AE and VAE models.
### Analysis
In this experiment, we explore the implementation and performance of Autoencoders (AE) and Variational Autoencoders (VAE) on the MNIST dataset, a collection of grayscale images depicting handwritten digits. The dataset is accessible on Kaggle at [MNIST Dataset](https://www.kaggle.com/datasets/hojjatk/mnist-dataset).

## Autoencoder (AE)

### Architecture and Training:
We designed a straightforward autoencoder architecture consisting of an encoder and decoder. The encoder compresses input data, while the decoder reconstructs it using densely connected layers.

### Hyperparameters:
- Learning rate: 0.001
- Batch size: 64
- Epochs: 50

## Variational Autoencoder (VAE)

### Architecture and Training:
VAEs, a variant of autoencoders, incorporate a probabilistic layer to introduce variability in the latent space. The architecture includes both an encoder and decoder with probabilistic components.

### Hyperparameters:
- Learning rate: 0.0001
- Batch size: 64
- Epochs: 50

### Loss and KL Divergence:
We visualize training and validation losses for both AE and VAE. Additionally, we plot the KL divergence for the VAE.

### Dataset:

- MNIST Dataset: [MNIST Dataset](https://www.kaggle.com/datasets/hojjatk/mnist-dataset)


## Insights and Conclusions:

- **Performance Evaluation:** 
  - Both AE and VAE models demonstrated promising results in reconstructing MNIST digits, with VAE showcasing improved variability in generated samples.
  
- **Latent Space Analysis:** 
  - Latent space visualization revealed distinct differences between AE and VAE, with VAE exhibiting a smoother distribution, indicating its probabilistic nature.



Through a meticulous comparison of performance metrics and the visualization of the latent space, we draw conclusions regarding the efficacy of AE and VAE on the MNIST dataset. While AE excels at capturing essential features, VAE introduces a probabilistic element, yielding a more structured and continuous latent space representation. The choice between AE and VAE is contingent on specific application requirements, with VAE offering distinct advantages in generating diverse and realistic data.
