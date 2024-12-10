# Stipple Image Generator with GUI using Weighted Voronoi Stippling

**Weighted Voronoi Stippling** program with custom `customtkinter` GUI allows users to select an image, set stippling parameters, generate weighted Voronoi stippling diagrams, and saving GIF of results evolutionm over iterations.

---

## 🚀 Features

- **File Selection**: Choose an image file (`.png`, `.jpg`, `.jpeg`, `.bmp`, `.tif`, `.tiff`).
- **Parameter Controls**:
- **Stipple Points**: Set the number of points for stippling (100 to 50,000).
- **Lloyd Iterations**: Number of Lloyd relaxation iterations (0 to 100).
- **Quantization Levels** (optional): Set number of gray values to interpret image as
- **Custom Seed** (optional): Set custom seed for testing
- **Random Sampling** (Defualt: True): Compute centroid using random sample instead of all pixels in region
- **Plot** (Defualt: True): Show Voronoi diagram and stipple results
- **Save** (Defualt: False): Save evolution of Voronoi stipple through iterations in a GIF file



  
- **Progress Updates**: Informative status messages during processing.
- **Plot Display**: View the generated stipple diagrams as plots.

---

## 🛠️ Requirements

- Python 3.8 or higher
- Required Python Libraries:
  - `customtkinter`
  - `PIL` (Pillow)
  - `matplotlib`
  - `numpy`
  - `scipy`

---
