# Stipple Image Generator App with GUI using Weighted Voronoi Stippling

**Weighted Voronoi Stippling** application with custom `customtkinter` GUI allows users to select an image, set stippling parameters, generate weighted Voronoi stippling diagrams, and save GIF of centroid evolution

---

## 🌟 **Features**

- **File Selection**:
  - Supports different dimmensions
  - Supports different image types (Gray, Color etc)
  - file types (`.png`, `.jpg`, `.jpeg`, `.bmp`, `.tif`, `.tiff`).
- **Plot Outputs**:
  - Produce weighted Voronoi diagram based on input image and paramerters
  - Produce stipple image based on the weighted Voronoi and input paramerters
- **Evolution GIF**:
  - Saves every iteration of image generation as a seemless GIF file showcasing centroid evolution
- **Quantization Levels**:
  - Can reduce the number of gray value outputs that are being used during computiation
- **Two Voronoi Region Centroid Computation Methods**:
  - Random sampling (Recommended):
    - Uses random sample of  `(max_x - min_x) * (max_y - min_y) * 10` size to find contained pixels, and uses those to compute gray value density centroid
    - Relativly faster Iterations
    - Introduces jitter, which is able to dislodge points that were previously stuck in an un-optimal space
  - Original Lloyd's Method:
    - Uses all pixels within region to compute gray value density centroid
    - Need fewer iterations to get to final Voronoi points
    - Final Voronoi points may be unevenly concentrated and result in some areas containing dense clusters of stuck points


---

## 🚀 **Parameter Controls**

- **Select Image**:
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
