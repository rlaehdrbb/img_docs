.. imgPreprocessor documentation master file, created by
   sphinx-quickstart on Sat Dec  7 14:24:21 2024.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

.. _delexif_section:

delexif
=======

**Functionality**  
Modifies or deletes EXIF metadata of images, then saves the updated metadata to a new image file.

**Input**  
- **Path setup:** `image_path` specifies the target image file.  
- **Optional parameters:** Specify metadata fields to modify:  
  - `make`: Camera manufacturer.  
  - `model`: Camera model name.  
  - `datetime`: Date and time of capture.  

**Supported Formats**  
- Works with JPEG and TIFF files.

**Output**  
- Saves the image with updated metadata to the specified `output_path`.

