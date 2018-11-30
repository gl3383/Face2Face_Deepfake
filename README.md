# Face2Face_Deepfake

1. Dataset

The video file of Angela Merkel (German Chancellor) was used to create the dataset. The number of training data required should be mentioned. In this case 400 images were considered. To detect the facial landmarks used shape_predictor_68_face.landmarks.dat file. Two folders, original and landmarks will be created. The original folder containing the actual image and the landmarks folder contains facial landmarks.

2. Pix2Pix

The original and landmark images are resized and then combined. The combined images are split as training and validation dataset. The model is trained with different number of epochs (10,133,200) to check the performance of the model.

3. Reduced model

The trained model is reduced to have a less file size. The reduced model is freezed to a single file.

4. Output

Input to run the demo- camera device index(default=0), show to display the normal input (default = 0), landmark model and frozen model.

Reference:
https://github.com/datitran/face2face-demo
https://github.com/affinelayer/pix2pix-tensorflow
