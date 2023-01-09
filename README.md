# super-resolution-using-CNN
Summary of the project is as described below:
we have a hyper-spectral image of balloons, each image is of dimension 512 x 512 and we have 31 such images.
Stack all the images to create a hyper-spectral image of dimension 512x512x31.
Then using this stacked hyper-spectral image, divide into 64 patches of 64x64x31.
Ground truth dataset will be then 64 patches (small image) of 64x64x31 dimensions.
downsample groud-truth dataset into two sub-datasets
a). High resolution RGB (64 images of size 64x64x3)
b). Low resolution multispectral imaages (64 images of size 8x8x31)

# CNN model:
created a CNN model to combine these two inputs (64x64x3 and 8x8x31) and give and output of image having dimensions of 64x64x31.

#SuperResolutionCNN.ipynb file is the finalized version of implementing all the above mentioned steps in the summary.
rest of the file are the intermediate versions while improving the model accuracy by altering different hyper-parametes of the CNN model.


