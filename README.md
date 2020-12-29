# GestureRecognition

Provided below are details of different models exeuction details for comparison.


| Model | Trainable parameters | Execution time | Best validation loss | Best validation accuracy |
|-------|----------------------|----------------|----------------------|--------------------------|
| Conv3D| 7,722,101            | 94 minutes     | 0.6530               | 0.9040                   |






Additional info:
----------------
All the models were run for 50 epochs.  Data augmentation and optimizer parameters maintained constant for like to like comparison.
Please note the early stopping patience is used at high value of 10, as we can notice from initial 6 to 7 epochs validation loss, smaller patience will result in early stop with in 6 or 7 epochs.

