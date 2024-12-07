.. imgPreprocessor documentation master file, created by
   sphinx-quickstart on Sat Dec  7 14:24:21 2024.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

.. _countface_section:

CountFace
=========

**Functionality**  
Detects and counts faces in an image using OpenCV's Haar Cascade model.

**Input**  
- **Image Path**: Set during initialization or via `set_image_path()`.  
  Example: ``image_path = 'data/gang.jpg'``.

**Output**  
- **Face Count**: Returns the number of detected faces and prints the count.  
- **Visual Display**: Highlights detected faces on the image and displays it in a window.

**Error Handling**  
- Alerts if the image path is missing or invalid.  
- Displays an error if the image cannot be loaded.


