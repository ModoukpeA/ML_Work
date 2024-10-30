### Objective

This script loads and preprocesses the data, builds a U-Net model for segmentation, and then trains the model on the pet images and masks.

- ### Data Loading and Preprocessing

We load the Oxford Pets dataset, resize images to 128x128 for easier computation, and normalize pixel values to be between 0 and 1.

- ### U-Net Model

We build a simplified U-Net model with several convolutional and pooling layers in the encoder, followed by transposed convolutions in the decoder. This structure allows the model to capture both low- and high-level features effectively, which is essential for segmentation tasks.

- ### Model Training

The model is trained using binary_crossentropy for binary segmentation, with early stopping to prevent overfitting.

- ### Visualization of Results

After training, we display a few images along with their true and predicted segmentation masks to visually assess the model’s performance.

### Why U-Net ?
