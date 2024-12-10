# Stipple Image Generator App with GUI using Weighted Voronoi Stippling

**Weighted Voronoi Stippling** application with custom `customtkinter` GUI allows users to select an image, set stippling parameters, generate weighted Voronoi stippling diagrams, and save GIF of centroid evolution

---

## 🚀 **Parameter Controls**

- **File Selection**:
  - Choose an image file (`.png`, `.jpg`, `.jpeg`, `.bmp`, `.tif`, `.tiff`).
- **Stipple Points**:
  - Set the number of points for stippling (100 to 50,000).
- **Lloyd Iterations**:
  - Number of Lloyd relaxation iterations (0 to 100).
- **Quantization Levels** (optional):
  - Set number of gray values to interpret image as
- **Custom Seed** (optional):
  - Set custom seed for testing
- **Random Sampling** (Defualt: True):
  - Compute centroid using random sample instead of all pixels in region
- **Plot** (Defualt: True):
  - Show Voronoi diagram and stipple image results
- **Save** (Defualt: False):
  - Save evolution of Voronoi stipple through iterations in a GIF file


---

## 🛠️ Requirements

- Built and Tested using Python 3.13.1
- Required Python Libraries:
  - `skimage`
  - `PIL`
  - `matplotlib`
  - `numpy`
  - `scipy`
  - `customtkinter`

---

## 📋 References

The following were influencial to the creating of this application
- Weighted Voronoi Stippling, Adrian Secord
  - https://www.cs.ubc.ca/labs/imager/tr/2002/secord2002b/secord.2002b.pdf
- `customtkinter` GUI library
  - https://github.com/TomSchimansky/CustomTkinter
- The Conding Train's P5.js that also references Adrian Secord's paper
  - https://www.youtube.com/watch?v=Bxdt6T_1qgc
 
---
