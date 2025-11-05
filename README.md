# Image Color Clustering with K-Means

This mini-project applies **unsupervised learning** to discover the dominant colors of an image using **K-Means clustering**.

## Objective

- Represent an image as a set of RGB pixels.
- Apply K-Means to group similar colors into *k* clusters.
- Extract the main color palette of the image.
- Reconstruct the image using only the clustered colors.

## Method

1. Load an RGB image (`PIL`).
2. Reshape it from `(H, W, 3)` to `(N_pixels, 3)`.
3. Apply `KMeans(n_clusters=k)` from `scikit-learn`.
4. Use the cluster centers as the **dominant colors**.
5. Replace each pixel by its cluster center and reconstruct the image.
6. Visualize:
   - Original image
   - Clustered image
   - Color palette bar

## Tools

- Python
- NumPy
- Pillow (PIL)
- scikit-learn
- Matplotlib

## Project Structure

```text
color-clustering-kmeans/
├── image_color_clustering.ipynb
├── images/
│   └── sample.jpg
├── results/
│   ├── original_image.png
│   ├── clustered_image_k5.png
│   └── color_palette_k5.png
└── README.md
