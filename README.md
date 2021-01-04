# Digital_image_processing_convert-one-file-format-to-other.

# AIM: WAP to convert one file format to other

# Requirements: setting up all the libraries after installing Python.

# Source code:

# Converting from one file format to another


im = Image.open("../images/parrot.png")

print(im.mode)

im.save("../images/parrot.jpg")

RGB



im = Image.open("../images/hill.png")

print(im.mode)

# RGBA

im.convert('RGB').save("../images/hill.jpg") # first convert to RGB mode

RGBA

Converting from one image mode into another


im = imread("../images/parrot.png", as_gray=True)

print(im.shape)

im = imread("../images/Ishihara.png")

im_g = color.rgb2gray(im)

plt.subplot(121), plt.imshow(im, cmap='gray'), plt.axis('off')

plt.subplot(122), plt.imshow(im_g, cmap='gray'), plt.axis('off')

plt.show()

(340, 453)

