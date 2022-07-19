
# Texture Detection

A brief description of what this project does and who it's for


## How to Use
Add the texture images that you want to be compared in the "Input_images" folder.

Run the "TextureDetectionUsingOpenCV" file and enter the name of the images along with the extension whem prompted.

Run the program and if the correlation function returns a value lesser than 0.4 then the image texture are similar.

The end result along with the correlation value will be dispayed at the end.
## How it works?
We have used Histogram of Oriented Gradients (hog) feature descriptor for normalising the image and generating a texture that is free from effects of local shadowing and illumination variations.
Normalisation introduces better invariance to illumination, shadowing, and edge contrast.

We have used rescale_intensity function which returns image after shrinking its intensity levels.

After this the original and test images are flatten to one dimensional array for comparison and then the correlation function returns the correlation coefficient between the flattened arrays.




For more detailed info please refer the following link of the documentations:

https://scikit-image.org/docs/stable/auto_examples/features_detection/plot_hog.html

https://scikit-image.org/docs/stable/api/skimage.exposure.html#skimage.exposure.rescale_intensity
