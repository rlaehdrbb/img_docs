.. imgPreprocessor documentation master file, created by
   sphinx-quickstart on Sat Dec  7 14:24:21 2024.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

.. _color_extracter_section:

color_extracter
===============

**Functionality**  
Extracts the dominant color palette from an image and visualizes it.

**Input**  
- **Path setup:** Provide the image file path (`image_path`).  
  Example: ``image_path = './path/to/image.jpg'``

- **Optional parameters:**  
  - `n_colors`: Number of dominant colors to extract (default is 5).

**Output**  
- **Return value:**  
  - `extract_color_palette`: Returns a list of RGB tuples for the extracted colors.  
    Example: ``[(255, 0, 0), (0, 255, 0), (0, 0, 255)]``

- **Visualization:**  
  - `plot_palette`: Displays the extracted colors as a horizontal bar chart using Matplotlib.



