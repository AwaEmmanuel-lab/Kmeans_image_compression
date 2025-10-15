# 🖼️ K-Means Image Compression

This project demonstrates how to compress images using the **K-Means clustering algorithm**.  
The idea is to reduce the number of colors in an image while keeping its essential structure and visual quality.

---

## 📚 How It Works

1. The image is read using `matplotlib.pyplot.imread()`.
2. The image pixels are reshaped into a 2D array where each row represents a pixel and each column represents RGB color values.
3. K-Means clustering groups similar colors together.
4. Each pixel is replaced with the centroid color of its assigned cluster.
5. The compressed image is displayed using `matplotlib.pyplot.imshow()`.

---

## ⚙️ Requirements

Make sure you have the following Python libraries installed:

```bash
pip install numpy matplotlib scikit-learn
```

---

## 🚀 How to Use

1. Clone or download this repository.
2. Open the notebook file:
   ```bash
   KMeans_Image_Compression.ipynb
   ```
3. Run the cells in order.

You can **replace the image path** with your own image:
```python
image = plt.imread(r"C:\path\to\your\image.png")
```

You can also **change the number of centroids (clusters)** to control the compression quality:
```python
k = 8  # Number of centroids
```

- Increasing `k` → higher quality, larger file size  
- Decreasing `k` → more compression, lower quality

---

## 🧠 Concept

K-Means image compression reduces color redundancy by representing similar colors with a single centroid value.  
This reduces the number of unique colors while preserving the overall look of the image.

---

## 🖼️ Example

| Original Image | Compressed Image |
|----------------|------------------|
| ![original](assets/original.png) | ![compressed](assets/compressed.png) |

*(You can add your own sample images in an `assets/` folder.)*

---

## ✨ Key Features

- Simple, beginner-friendly implementation of **K-Means for images**
- Users can **customize the number of clusters** for different compression levels
- Works with **any image** from your local system

---

## 🧩 Future Improvements

- Add automatic optimal `k` selection using the **elbow method**
- Implement batch image compression
- Support other color spaces (e.g., HSV, LAB)

---

## 👨‍💻 Author

**Awa**  
*Machine Learning & Computer Vision Enthusiast*  
📧 Contact: [your.email@example.com]  
📦 GitHub: [https://github.com/yourusername](https://github.com/yourusername)

---
