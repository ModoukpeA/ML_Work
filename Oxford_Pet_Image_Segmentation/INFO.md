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

![image](https://github.com/user-attachments/assets/e7290bcd-b757-4608-a668-6bc1368a4b57)

*Source: Towards Data Science (https://towardsdatascience.com/u-net-explained-understanding-its-image-segmentation-architecture-56e4842e313a?gi=78da42d798e8)*


The U-Net architecture is well-suited for image segmentation tasks like the Oxford Pets segmentation project because of its unique structure and ability to capture both the local and global features of images. A few reasons:

- **Symmetric Encoder-Decoder Structure:** U-Net's architecture is based on a symmetric encoder-decoder design, where the encoder gradually reduces the spatial dimensions (capturing high-level features) and the decoder gradually reconstructs the image’s original size (adding details back in). This structure helps retain the spatial context necessary for accurately segmenting images at a pixel level.

- **Skip Connections:** One of U-Net's key innovations is the use of skip connections, which connect each encoder layer to its corresponding decoder layer. These connections allow the network to retain fine-grained information from earlier layers in the encoding process, which is crucial for tasks where precise localization is important, such as segmenting pet boundaries in an image.

- **Effective for Small Data Sets:** U-Net was initially developed for biomedical image segmentation, where annotated data is often limited, similar to many specific-use cases in image segmentation. Its architecture performs well on smaller datasets, making it suitable for projects like Oxford Pets where high-quality labeled data is limited.

- **Detailed Boundary Detection:** U-Net's structure is designed to focus on boundary details, which is essential when segmenting objects with intricate shapes like pets. The model effectively captures the edges of objects, producing segmentations that closely follow the boundaries of objects in an image.
