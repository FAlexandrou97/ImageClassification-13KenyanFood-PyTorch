# ImageClassification-13KenyanFood-PyTorch
### [Image Classification Task which is part of the Deep Learning with PyTorch OpenCV course.](https://www.kaggle.com/c/pytorch-opencv-course-classification)
The [dataset](https://www.kaggle.com/c/pytorch-opencv-course-classification/data) consists of 8,174 images in 13 Kenyan food type classes from which the 20% was used for validation.

The input image size is 224 by 224 pixels and I have used several [Data Augmentation](https://pytorch.org/docs/stable/torchvision/transforms.html) techniques, such as Random Vertical/Horizontal Rotation and Color Jitter (brightness, contrast).

I have used pretrained Resnet50 ([wide_resnet50_2](https://pytorch.org/docs/stable/torchvision/models.html#wide-resnet)) 
and froze 60% of the parameters, leaving the last 40% of the network parameters trainable. The model was trained for 30 epochs and achieved 94% training and 75% validation accuracy. The highest score of my Kaggle submission is currently at 73.5% accuracy.

Initial training Tensorboard logs: https://tensorboard.dev/experiment/VtMb0okWSXCqv3nPSZyHRw/

#### -Todo
1. Modularize the training pipeline to allow for rapid experimentation.
1. Refactor code to increase readability.
1. Try ensemble learning to achieve higher accuracy.
1. Update tensorboard logs.
