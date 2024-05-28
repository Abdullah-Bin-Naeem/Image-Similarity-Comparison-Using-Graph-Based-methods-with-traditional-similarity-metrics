# Image-Similarity-Comparison-Using-Graph-Based-methods-with-traditional-similarity-metrics

# Image Similarity Comparison

This project aims to compare the similarity between two images using both traditional similarity metrics and a graph-based method. The traditional metrics include Structural Similarity Index (SSIM), Root Mean Square Error (RMSE), Peak Signal-to-Noise Ratio (PSNR), and Image Structural Similarity Measure (ISSM). The graph-based method involves dividing the images into patches, creating fully connected graphs for each image, and computing similarity based on the cosine similarity between the adjacency matrices.

## Introduction

In this project, we compare the similarity between two images using different methods. We evaluate both traditional similarity metrics and a novel graph-based approach.

## Methodology

### Traditional Similarity Metrics
- **Structural Similarity Index (SSIM):** Measures the structural similarity between two images.
- **Root Mean Square Error (RMSE):** Measures the average difference between corresponding pixels of two images.
- **Peak Signal-to-Noise Ratio (PSNR):** Measures the ratio between the maximum possible power of a signal and the power of corrupting noise.
- **Image Structural Similarity Measure (ISSM):** Measures the similarity between two images based on luminance, contrast, and structure.

### Graph-Based Method
1. **Divide Images:** Resize both images to 120x120 pixels.
2. **Create Graphs:** Divide each image into patches and create fully connected graphs for each image.
3. **Edge Calculation:** Compute the difference between the mean intensities of corresponding patches and assign them as edge weights.
4. **Cosine Similarity:** Compute the cosine similarity between the adjacency matrices of the graphs.

## Results

### Traditional Similarity Metrics on the images you can see in data/:
- **Structural Similarity Index (SSIM):** 0.01138052929677652
- **Root Mean Square Error (RMSE):** 222.40602572272581
- **Peak Signal-to-Noise Ratio (PSNR):** 1.1878726175040497
- **Image Structural Similarity Measure (ISSM):** 0.9886194707032234

### Graph-Based Method:
- **Graph-Based Cosine Similarity:** 0.9999999999999972

## Performance Comparison

- **SSIM Time:** 0.003396272659301758 seconds
- **RMSE Time:** 0.0 seconds
- **PSNR Time:** 0.0 seconds
- **ISSM Time:** 0.0 seconds
- **Graph-Based Cosine Similarity Time:** 0.011644840240478516 seconds

  
## Our findings
- Graph based methods are more accurate however their excetion is significantally high. It grows exponentially by increasing the graph size(in our case increasing the number of patches).

## How to Run
- Clone or download this repository and just run the jupyter notbook file (Don't forget to change the image names and paths :basecampy:)
- Yes its that simple 🧁




## Contributing

Contributions are welcome! Please fork the repository and submit a pull request.

## License


This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact
For any questions or inquiries, please contact abdullahbinnaeempro@gmail.com.

