# iLABEL

The aim of this work is to semi-automatise labelling image process.
We want to achieve this through:
- speeding up the process
- decrease the human error
- make the process reproducible

## Case study

Here we want to label a set of 1k images with some quality measures.
Those labels are:
- overall quality
- light
- growth
- focus

### Starting from this...

| **im_id**     | overall          | light                      |...|focus|
| ------------- |:-------------:| ---------------------------:|---|---------|
| im1     | NA     | NA |...|NA|
| im2     | NA     | NA               |...|NA|
| im3     | NA     | NA                       |...|NA|


### Practically, the user will be asked to:
- load a set of images (specify the path)
- visualise one image at time
- input the value and submit
- go to next image and repeat
- save and eventually continue from this step

### And we get back...

| **im_id**     | overall          | light                      |...|focus|
| ------------- |:-------------:| ---------------------------:|---|---------|
| im1     | 0.1     | 0.1 |...|0.3|
| im2     | 0.9     | 0.6               |...|1|
| im3     | 0.7     | 0.6                       |...|0.5|


### In the backhand
When the user defines the list of images a database have to be created. When the user submit his values, they should be added to the images on the db.

### An idea for the interface

![alt text](https://github.com/apollo994/iLABEL/blob/master/gui.png)

**Some test images to play with can be found [here](https://github.com/apollo994/CMP_images/tree/master/test_data/img_jpg)**

## To keep in mind (not mandatory at the beginning)
- Number and name of the metrics could vary depending on the need

