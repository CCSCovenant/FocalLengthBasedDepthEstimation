# FocalLengthBasedDepthEstimation
## idea:
with multiply imgs taking from single camera in different focal length. we can estimate the distance of a object to the camera
with thier frequency imformation. 

-> due to taking multiply imgs from the single camera at same time is not very practical in many case, we may taking a video sequence 
with focal length being a periodic function and use tempoal method to recover depth infromation in a small range of frame.

-> here we introduced an assumption that object in our sence is not moving very quick. 

## Step 1 
taking multiply imgs from single camera.
use large aperture and low exposure time so that we can making sure that 
1. Depth of field is small
2. Camera can take img as fast as possible. 

## Step 2
calculate gradient map for all frame.

## Step 3
for each pixel, search for the highest gradient magnitude in the nearby frame.
Since we know the focal length F in that frame and this pixel is highly likely focused in this focal length,
we can get a estimate distance range for this pixel.

