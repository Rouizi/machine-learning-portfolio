## Image Classification of Dog Breeds

The dataset contains over 20,000 images of 120 dog breeds and the task is to build a model that can correctly identify each dog breeds: this a classic classification problem.

For the first part, I tried to build a neural network from scratch but it turns out that the model was too simple for this task (the model underfit the data).

In the second part, I used transfer learning from a pretrained model. I picked MobileNet for this but the model was overfitting, so I had to use data augmentation and dropout. Finally, I tried fine-tuning to increase the performance even further but, unfortunately, that didn't help at all.

After training the model, I analysed the errors that the model made to see how we can improve it.