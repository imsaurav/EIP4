
 Decreased the no of parameters from 15k to 14k by minimising the no of channels used.
 With 20 epochs found that there was a lot of gap between training and testing accuracy(99.67 to 99.05), 
 so had to batch normalize  and saw that the parameters have increased a little bit.(99.72 to 99.13).
 The gap was still similar post batch notmalization...so tried adding dropout for regularization
 Changed the drop out value from 0.25 to 0.1 to increase accuracy and added a few small layers too.
Changing the batch size from 512 to 256 resulted in better learning and accuracy.

Anf observed 99.4 in 18 epochs with almost no gap between training and testing accuracy.




Train on 60000 samples, validate on 10000 samples
Epoch 1/20

Epoch 00001: LearningRateScheduler setting learning rate to 0.003.
60000/60000 [==============================] - 10s 175us/step - loss: 0.0622 - acc: 0.9800 - val_loss: 0.0612 - val_acc: 0.9820
Epoch 2/20

Epoch 00002: LearningRateScheduler setting learning rate to 0.0022744503.
60000/60000 [==============================] - 10s 166us/step - loss: 0.0450 - acc: 0.9859 - val_loss: 0.0338 - val_acc: 0.9890
Epoch 3/20

Epoch 00003: LearningRateScheduler setting learning rate to 0.0018315018.
60000/60000 [==============================] - 10s 171us/step - loss: 0.0353 - acc: 0.9885 - val_loss: 0.0525 - val_acc: 0.9844
Epoch 4/20

Epoch 00004: LearningRateScheduler setting learning rate to 0.0015329586.
60000/60000 [==============================] - 10s 169us/step - loss: 0.0319 - acc: 0.9898 - val_loss: 0.0379 - val_acc: 0.9882
Epoch 5/20

Epoch 00005: LearningRateScheduler setting learning rate to 0.0013181019.
60000/60000 [==============================] - 10s 165us/step - loss: 0.0290 - acc: 0.9906 - val_loss: 0.0258 - val_acc: 0.9924
Epoch 6/20

Epoch 00006: LearningRateScheduler setting learning rate to 0.0011560694.
60000/60000 [==============================] - 10s 169us/step - loss: 0.0285 - acc: 0.9913 - val_loss: 0.0263 - val_acc: 0.9923
Epoch 7/20

Epoch 00007: LearningRateScheduler setting learning rate to 0.0010295127.
60000/60000 [==============================] - 10s 169us/step - loss: 0.0273 - acc: 0.9913 - val_loss: 0.0290 - val_acc: 0.9919
Epoch 8/20

Epoch 00008: LearningRateScheduler setting learning rate to 0.0009279307.
60000/60000 [==============================] - 10s 165us/step - loss: 0.0240 - acc: 0.9924 - val_loss: 0.0272 - val_acc: 0.9924
Epoch 9/20

Epoch 00009: LearningRateScheduler setting learning rate to 0.0008445946.
60000/60000 [==============================] - 10s 163us/step - loss: 0.0237 - acc: 0.9928 - val_loss: 0.0241 - val_acc: 0.9924
Epoch 10/20

Epoch 00010: LearningRateScheduler setting learning rate to 0.0007749935.
60000/60000 [==============================] - 10s 162us/step - loss: 0.0228 - acc: 0.9930 - val_loss: 0.0269 - val_acc: 0.9927
Epoch 11/20

Epoch 00011: LearningRateScheduler setting learning rate to 0.0007159905.
60000/60000 [==============================] - 10s 166us/step - loss: 0.0223 - acc: 0.9932 - val_loss: 0.0228 - val_acc: 0.9929
Epoch 12/20

Epoch 00012: LearningRateScheduler setting learning rate to 0.000665336.
60000/60000 [==============================] - 10s 165us/step - loss: 0.0208 - acc: 0.9934 - val_loss: 0.0236 - val_acc: 0.9927
Epoch 13/20

Epoch 00013: LearningRateScheduler setting learning rate to 0.0006213753.
60000/60000 [==============================] - 10s 162us/step - loss: 0.0209 - acc: 0.9932 - val_loss: 0.0227 - val_acc: 0.9932
Epoch 14/20

Epoch 00014: LearningRateScheduler setting learning rate to 0.0005828638.
60000/60000 [==============================] - 10s 173us/step - loss: 0.0198 - acc: 0.9941 - val_loss: 0.0239 - val_acc: 0.9929
Epoch 15/20

Epoch 00015: LearningRateScheduler setting learning rate to 0.0005488474.
60000/60000 [==============================] - 10s 167us/step - loss: 0.0198 - acc: 0.9937 - val_loss: 0.0224 - val_acc: 0.9937
Epoch 16/20

Epoch 00016: LearningRateScheduler setting learning rate to 0.0005185825.
60000/60000 [==============================] - 10s 171us/step - loss: 0.0198 - acc: 0.9937 - val_loss: 0.0231 - val_acc: 0.9931
Epoch 17/20

Epoch 00017: LearningRateScheduler setting learning rate to 0.000491481.
60000/60000 [==============================] - 10s 169us/step - loss: 0.0187 - acc: 0.9942 - val_loss: 0.0230 - val_acc: 0.9929
Epoch 18/20

Epoch 00018: LearningRateScheduler setting learning rate to 0.0004670715.
60000/60000 [==============================] - 10s 172us/step - loss: 0.0183 - acc: 0.9943 - val_loss: 0.0222 - val_acc: 0.9943
Epoch 19/20

Epoch 00019: LearningRateScheduler setting learning rate to 0.0004449718.
60000/60000 [==============================] - 10s 166us/step - loss: 0.0177 - acc: 0.9940 - val_loss: 0.0242 - val_acc: 0.9926
Epoch 20/20

Epoch 00020: LearningRateScheduler setting learning rate to 0.000424869.
60000/60000 [==============================] - 10s 165us/step - loss: 0.0184 - acc: 0.9939 - val_loss: 0.0217 - val_acc: 0.9938
<keras.callbacks.History at 0x7f9d4eac80b8>
