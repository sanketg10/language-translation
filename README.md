# language-translation

We use an encoder to encode input sentences into a vector. 
This vector is then used by a decoder to create a translated sentence. 
All the weights are basically for word embedding vectors, and the final fully connected layer.

For decoder: 
Every word that is predicted feeds into the next time step (during inference) 
Every target word which should comes next goes into next time step (during training)

Fully connected layer: 
This layer feeds into a softmax function which gives probability of every word in the vocab. 

I tuned the hyper-parameters several times till I got a good response. 
Bigger data might get even better performance, but it came close to 99% for this! 
