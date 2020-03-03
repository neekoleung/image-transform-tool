# HSL Image Processing Tool
A project from UIUC CS 400.

## [PNG.cpp](https://github.com/neekoleung/image-transform-tool/blob/master/uiuc/PNG.cpp)
For loading and saving PNG files:
* __bool PNG::readFromFile(const std::string & fileName)__: loads an image based on the provided
file name, a text string. The return value shows success or failure. 
* __bool PNG::writeToFile(const std::string & fileName)__: writes the current image to the provided
file name (overwriting existing files).

For retrieving pixel and image information:
* __unsigned int PNG::width() const__: returns the width of the image.
* __unsigned int PNG::height() const__: returns the height of the image.
* __HSLAPixel & getPixel(unsigned int x, unsigned int y)__: returns a direct reference to a pixel at
the specified location.

Other methods:
* Methods for creating empty PNGs, resizing an image, etc.

## [ImageTransform.cpp](https://github.com/neekoleung/image-transform-tool/blob/master/ImageTransform.cpp)
* __PNG grayscale(PNG image)__: Returns an image that has been transformed to grayscale.
![](https://res.cloudinary.com/dvrxfispp/image/upload/v1583224387/Github/uiuc-cpp/1_vaxkjw.png)
* __PNG createSpotlight(PNG image, int centerX, int centerY)__: Returns an image with a spotlight centered at (centerX, centerY).
![](https://res.cloudinary.com/dvrxfispp/image/upload/v1583224382/Github/uiuc-cpp/2_p72xiu.png)
* __PNG illinify(PNG image)__: Returns a image transformed to Illini Orange (11) or Illini Blue (216).
![](https://res.cloudinary.com/dvrxfispp/image/upload/v1583224380/Github/uiuc-cpp/3_nmadmi.png)
* __PNG watermark(PNG firstImage, PNG secondImage)__: Returns an immge that has been watermarked by another image.
![](https://res.cloudinary.com/dvrxfispp/image/upload/v1583224376/Github/uiuc-cpp/4_mdlc10.png)
