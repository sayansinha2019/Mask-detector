# Mask-detector
It is CNN Deep learning model, to detect wether a person is wearing  mask or not.
So i created a dataset with the help of python script, in which i passed a videostream and by using OpenCV ROI(Region Of Interest), a dataset of  faces collected with respective  directories namely with mask and without mask.

Later this Dataset is passed for fine-tuning using the MobileNet V2 architecture, a highly efficient architecture that can be applied to embedded devices.
During training (train.py), i applied on-the-fly mutations to our images in an effort to improve generalization. This is known as data augmentation, where the random rotation, zoom, shear, shift, and flip parameters are established.Then we loaded he model with pre-trained Imagenet weights.
Nextly,i compiled the model with the Adam optimizer, a learning rate decay schedule, and binary cross-entropy.

So  now run the Detect_mask_video.py , it will run live video feed from the camera and pass it to the deep learning tensorflow  model in order to  run out the frames ovver the video feed and classify  wether the person is using mask or not.
