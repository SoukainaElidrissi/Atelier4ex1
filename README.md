# Autoencoder vs Variational Autoencoder on MNIST Dataset

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

## Conclusion:

Our analysis focuses on the convergence of the models. The VAE loss encompasses a reconstruction term and a KL divergence term, illustrating the delicate balance between preserving information and introducing variability.

## Latent Space Visualization:

We create plots representing the latent space representations of both AE and VAE. Each point in the plot corresponds to a digit in the dataset.

### Conclusion:

Our examination centers on the distribution of points in the latent space. The VAE's latent space is anticipated to display a smoother distribution due to its probabilistic nature.

## Overall Conclusion:

Through a meticulous comparison of performance metrics and the visualization of the latent space, we draw conclusions regarding the efficacy of AE and VAE on the MNIST dataset. While AE excels at capturing essential features, VAE introduces a probabilistic element, yielding a more structured and continuous latent space representation. The choice between AE and VAE is contingent on specific application requirements, with VAE offering distinct advantages in generating diverse and realistic data.
