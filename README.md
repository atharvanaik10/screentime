# ScreenTime

### Project Goals:

A neural network is trained to detect faces in a frame (image) and output the faces in the image. 
* We use `OpenCV` to extract individual frames from the movie clip
* We use `MTCNN` (multitask cascaded convolutional neural network) to extract faces for each frame

Another neural network is trained on a dataset of faces of Bollywood actors to recognize and classify faces. 
* We use `FaceNet` (wrapped in `keras`) to extract face mappings
* We use `scikit-learn` to develop a classifier for our faces

[More information about face recognition](https://docs.google.com/document/d/1598xceIfkDeDQmPRQhCrsC8KbZ0vLFTGVJUl3PAp99o/edit?usp=sharing)

We use this classification of faces for each actor for each frame in the given movie clip to calculate the frequencies (# of frames) each actor appears in. 
* This is done using vanilla `Python` with `Numpy`

We then visualize this data to show actor screentime percentage.
* We use `Numpy` and `matplotlib` to compile and visualize data
