# UNetX

PyTorch implementation of U-shaped network architecture.  
The implementation offers some architectural flexibility, for example, user can choose number of blocks in the encoding path (simmetrically repeated in the decoder). Also number of kernels in the convolutions defining the blocks are tweakable.  

The class inputs are:
+ (self, inCha, finOutCha, depths, inWidth, inHeight):
+ inpCha: number of channels in the input image.
+ finOutCha: depth of the output tensor.
+ depths: the is a list of integer. The lenght of the list gives the number of blocks in the encoder. Each integer is the number of kernels for the convolutions in the respective blocks.
+ inpWidth: width of the input image.
+ inpHeight: height of the input image.
