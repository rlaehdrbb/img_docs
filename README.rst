imqPreprocessor
===============

A Python library for text preprocessing, specifically designed to clean and process data efficiently for machine learning tasks. This library offers tools for color palette extraction, image filtering, face detection, blurring, and EXIF metadata modification.

Contents
--------

- Installation
- Usage
- Documentation

Installation
------------

To install the package, run:

.. code-block:: bash

   pip install imqPreprocessor

Usage
-----

The `imqPreprocessor` library provides various tools for image preprocessing. Below are some examples:

1. **Extract and Plot Color Palette**

   Extract color palettes from an image and visualize them:

   .. code-block:: python

       from img import extract_color_palette, plot_palette

       plot_palette(extract_color_palette("image_path.jpg"))

2. **Apply Custom Color Filters**

   Use `ColorFilter` to apply custom filters to an image:

   .. code-block:: python

       from imgPreprocessor import ColorFilter

       c = ColorFilter("image_path.jpg")

       user_color = (201, 251, 206)  # (B, G, R)
       c.custom_colorfilter(user_color)
       c.show()

       c.deepskyblue_colorfilter()
       c.show()

3. **Count Faces in an Image**

   Use `CountFace` to count the number of faces in an image:

   .. code-block:: python

       from imgPreprocessor import CountFace

       c = CountFace()
       c.set_image_path("image_path.jpg")
       print(c.count_faces())

4. **Enhance and Blur Images**

   Use `CustomBlurFilter` to enhance and blur images:

   .. code-block:: python

       from imgPreprocessor import CustomBlurFilter

       c = CustomBlurFilter("image_path.jpg")
       c.load_image()
       c.enhance_and_blur(clip_limit=2.0, tile_grid_size=(8, 8), blur_ksize=(15, 15))
       #optional: clip_limit, tile_grid_size, blur_ksize
       c.display_images()

5. **Modify EXIF Data**

   Use `modexif` to update the EXIF metadata of an image:

   .. code-block:: python

       from imgPreprocessor import modexif

       modexif(
           "image_path.jpg",  
           "output_path.jpg", 
           make="samsung",    
           model="S24",      
           datetime="2024:12:05 12:57:54")
        #optional: make, model, datetime
        #datetime format : "year:month:day hour:minute:second"
      
Documentation
-------------

For detailed documentation, visit:
[Link to Documentation](https://pypi.org/project/imgPreprocessor/1.0.0/)
