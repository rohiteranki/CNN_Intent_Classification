# Intent classification for a chatbot using Convolutional Neural Networks

This is a Keras implementation for the task of sentence classification using CNNs. This work was done as a part of [Midterm Assignment](https://github.com/llSourcell/AI_for_Resumes) given by Siraj Raval. Here's his great [video](https://youtu.be/p3SKx5C04qg) explaining Natural Language Processing applied to resume screening.

Dataset for the above task was obtained from the project [Natural Language Understanding benchmark ](https://github.com/snipsco/nlu-benchmark/tree/master/2017-06-custom-intent-engines)

Text used for the training falls under the six categories namely, AddToPlaylist, BookRestaurant, GetWeather , RateBook , SearchCreativeWork, SearchScreeningEvent each having nearly 2000 sentences.

To prepare the dataset, from the main project's directory, open terminal and type:

```bash
$ python prepare_data.py
```

Check [Intent_Classification_Keras_Glove.ipynb](https://github.com/ajinkyaT/CNN_Intent_Classification/blob/master/Intent_Classification_Keras_Glove.ipynb) for the model building and training part.

I was able to achive 99% accuracy on training and validation dataset within a minute after 3 epochs when trained on a regular i7 CPU.

#### What lies ahead?

Intent classification and named entity recognition are the two most important parts while making a goal oriented chatbot.

There are many open source python packages for making  a chatbot, Rasa  is one of them. The cool thing about Rasa is that every part of the stack is fully customizable and easily interchangeable. Although Rasa has an excellent built in support for intent classification task but we can also specify our own model for the task, check [Processing Pipeline](https://nlu.rasa.com/pipeline.html) for more information on it. 


## Resources

[Using pre-trained word embeddings in a Keras model](https://blog.keras.io/using-pre-trained-word-embeddings-in-a-keras-model.html)

[Convolutional Neural Networks for Sentence Classification
](https://arxiv.org/abs/1408.5882)

[A Sensitivity Analysis of (and Practitioners' Guide to) Convolutional Neural Networks for Sentence Classification
](https://arxiv.org/abs/1510.03820)




