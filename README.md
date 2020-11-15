# GestureRecognition
GestureRecognition with all pre-trained models and exclusive models

I will run through most of the famous pre-trained models and models which we create from scratch.

*** Please note the below results are for a particular data set and will be updated / tuned once I run through all the different models
1. Inception V3 - results - best validation accuracy 69% - best train accuracy 66% - epochs -> 30 with earlystopping - trainable parameters 19,402,757 -> image size 160x160x3
2. MobileNet V2 - results - best validation accuracy 81% - best train accuracy 82% - epochs -> 30 with earlystopping - trainable parameters 33,296,389 -> image size 160x160x3
3. ResNet50 - results - best validation accuracy 50% - best train accuracy 43% - epochs -> 30 with earlystopping - trainable parameters 34,082,821 -> image size 120x120x3
4. VGG16 - results - best validation accuracy 80% - best train accuracy 86% - epochs -> 30 with earlystopping - trainable parameters 13,635,589 -> image size 160x160x3.  VGG16 model's runtime is at least 10 times more than the highest time consuming model we have seen.
5. VGG19 - results - best validation accuracy 72% - best train accuracy 76% - epochs -> 30 with earlystopping - trainable parameters 13,635,589 -> image size 160x160x3.  VGG19 model's runtime too is at least 10 times more than the highest time consuming model we have seen.








Models and/or modifications which did not work well.

a. Inception V3 Fine Tuning V1 - results - best validation accuracy 69% - best train accuracy 66% - epochs -> 30 with earlystopping - trainable parameters 2,625,541 -> image size 160x160x3 -- Replaced Flatten Layer with Global Average Pooling Layer.  We can see the trainable parameters come down from 19 million to 2 million plus.
