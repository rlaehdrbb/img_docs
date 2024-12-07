.. imgPreprocessor documentation master file, created by
   sphinx-quickstart on Sat Dec  7 14:24:21 2024.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

.. _CustomBlurFilter_section:

CustomBlurFilter
================

**Functionality**  
Processes an input image with various preprocessing techniques such as CLAHE (Contrast Limited Adaptive Histogram Equalization), histogram equalization, and Gaussian blur.

**Input**  
- **Path setup:**  
  Provide the image path (`image_path`) when initializing the class.  
  Example: ``image_path = os.path.join("example.jpg")``  
  Incorrect paths raise a `FileNotFoundError`.

- **Supported formats:**  
  Supports common formats like `.jpg`, `.png`, `.jpeg`.  
  Invalid formats or unreadable files raise a `ValueError`.

**Output**  
- **Processed image:**  
  Stored in `self.enhanced_blurred_image` after running `enhance_and_blur()`.

**Display**  
- Shows the original and processed images in separate windows using `cv2.imshow()`.  
- Resizes larger images to fit the display.  
- Closes windows with `cv2.destroyAllWindows()` after `cv2.waitKey(0)`.




