# OCT Classification Using Self-Supervised Learning

### SimCLR
* Why this method was chosen?
* Images have 1 or 3 channels? How to treat that?
* How to choose which augmentations to do and how they affect the learning?
* How to train? How to adjust hyper parameters?
* How to inspect the training process? Where or how can I check the loss and f_1 score?
* How to evaluate the self-supervised training part? Can I use t-sne?
* Which tests should I do while training? Which pipelines?
* The amount of data splitted between supervised and unsupervised learning should change so that I can analyse how the amout of data impacts?

### To Do
* Fix number of input channels. OK
* Set a global seed. OK - Check if it works how it is supposed to
* If I train a model more than one time, with the same parameters, the result shouldnt be the same? - Check this out
* Improve training of pretext task (prevent overfit).
* Check the input size (96 or 224? for pretext training? and for downstream? how is it going to be?)
* Remove the labels of part of the data?
* Evaluate the results of the pretext task with t-SNE. OK - I think