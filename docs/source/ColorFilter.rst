.. imgPreprocessor documentation master file, created by
   sphinx-quickstart on Sat Dec  7 14:24:21 2024.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

.. _ColorFilter_section:

ColorFilter
===========

**Functionality**  
Applies various color filters (e.g., grayscale, custom, specific filters) to the input image.

**Input**  
- **Path setup:**  
  Pass the image path (`image_path`) when initializing the class.  
  Example: ``image_path = './imagePreprocessor/picture/100.jpg'``  
  Incorrect paths return `None` from `cv2.imread()`.

- **Supported formats:**  
  Accepts common formats like `.jpg`, `.png`, `.jpeg`.

**Output**  
- **Filtered images:**  
  Stored in `self.image` after applying filters.

- **Display:**  
  - Uses `cv2.imshow()` to display images in a window.  
  - Windows remain open until a key press (`cv2.waitKey(0)`).  
  - Closes windows with `cv2.destroyAllWindows()`.



