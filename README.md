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
- specify the labels he/she wants to add
- visualise one image at time
- input the value and submit
- go to next image and repeat
- save and eventually continue from this step

### We want the user to inspect images and return

| **im_id**     | overall          | light                      |...|focus|
| ------------- |:-------------:| ---------------------------:|---|---------|
| im1     | 0.1     | 0.1 |...|0.3|
| im2     | 0.9     | 0.6               |...|1|
| im3     | 0.7     | 0.6                       |...|0.5|



### In the backhand...
When the user defines the list of images a database have to be created.
When the user defines the labels, they should be added as new column in the db.
When the user inputs his values, they should be added to the images on the db.


## To keep in mind (not mandatory at the beginning)
- Number and name of the metrics could vary depending on the need
