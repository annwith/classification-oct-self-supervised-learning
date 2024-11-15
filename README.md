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
* Fix number of input channels.
* Set a global seed.
* Improve training of pretext task (prevent overfit).
* Evaluate the results of the pretext task with t-SNE.