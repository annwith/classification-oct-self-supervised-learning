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
* Why do I need a head for the model? I just dont use the back bone? Is this right? 

### To Do
* Fix number of input channels. OK
* Set a global seed. OK - Check if it works how it is supposed to - Run model two times and see if the result is the same.
* If I train a model more than one time, with the same parameters, the result shouldnt be the same? - Yes
* Improve training of pretext task (prevent overfit). - Hard one
* Check the input size (96 or 224? for pretext training? and for downstream? how is it going to be?)
* Remove the labels of part of the data?
* Evaluate the results of the pretext task with t-SNE. OK - I think (But with real problemas we wont have the labels)
* Reorganizar arquivos e colocar funções repetidas em utils.py

### Doing
* Checking global seed.
* Define one data split and go through with it.
* How to improve documentation of the tests:
1. the model
2. the augmentations 
3. data split and stuff before the training

### Perguntar pro professor
* seed - dois treinamentos com resultados diferentes -> precisa reiniciar o notebook pra dar igual
* overfit e resultados de validação - Regularização -> Augmentation e Dropout
* pra que que serve a cabeça do modelo? Na tarefa pretexto pra nada.
* o que fazer mais... - Tarefa downstream (feeeito... mas tem que treinar e tal, e a tarefa pre texto ta ruim demais. Usar tsne pra avaliar)
* Usar menos dados ainda no supervisionado pra deixar a comparação mais competitiva

### Experimentos:
#### Tarefa pretexto
* RGB (3 canais) x 1 canal (a vdd é que 3 canais tava indo melhor, acho que pq as aumentações estavam mais intensas) - fazer uma branch pra esse teste
* Mais aumentações, mais e mais e mto doidas
* transfer learning x from scratch
* dropout x sem dropout
