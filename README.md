# GestureRecognition

Provided below are details of different models exeuction details for comparison.


| Model                | Trainable parameters | Execution time | Best validation loss | Best validation accuracy |
|----------------------|----------------------|----------------|----------------------|--------------------------|
| Conv3D with softmax  | 7,722,101            | 94 minutes     | 0.6530               | 0.9040                   |
|----------------------|----------------------|----------------|----------------------|--------------------------|
| Conv3D with sigmoid  | 7,722,101            | 90 minutes     | 0.6023               | 0.8920                   |




Additional info:
----------------
1. All the models were run for 50 epochs.  Data augmentation and optimizer parameters maintained constant for like to like comparison.
2. Please note the early stopping patience is used at high value of 10, as we can notice from initial 6 to 7 epochs validation loss, smaller patience will result in early stop with in 6 or 7 epochs.
3. As we have 30 frames in each sequence I have taken frames at odd number position to minimize the training time with no performance loss

Points noted:
-------------
1. We can notice that for Conv3D model, we have different performance for different activation functions softmax and sigmoid. Softmax activation function gave slightly better performance where as sigmoid on slightly overfitting side.  This might just be a one-off case.
