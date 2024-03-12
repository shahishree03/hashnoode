---
title: "Recurrent Neural Networks"
datePublished: Wed Jan 18 2023 06:14:42 GMT+0000 (Coordinated Universal Time)
cuid: cld19ri8h000308jnc4u36yco
slug: recurrent-neural-networks
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1674022313690/c9cb6d28-57e3-4088-be16-ff9b8bf8102e.jpeg
tags: neural-networks, neural-network, recurrent-neural-network

---

# Introduction

In my previous blog, we discussed briefly [artificial neural networks](https://blog.techlearnindia.com/artificial-neural-network-in-a-nutshell) and their types.

[![](https://cdn.hashnode.com/res/hashnode/image/upload/v1674020139663/4b243315-559f-4b49-bb9b-f2b15069bd4b.png align="center")](https://app.techlearnindia.com/introduction-to-neural-network)

A recurrent network is a kind of artificial neural network *containing loops, allowing information to be stored within the network*. The output from the previous step is fed as input to the current step within the network. It uses sequential or time series data.

Recurrent Neural Network is derived from feed-forward neural networks. RNNs can use their internal state (memory) to process variable-length sequences of inputs. This makes them applicable in deep learning and in the development of models that simulates human brains. Mainly used in **speech recognition** and **natural language processing** (NLP).

# Why recurrent network is used? 💡

We know that in traditional neural networks, all the inputs and outputs are independent of each other. But when it is required to predict the next word of a sentence, the previous words are required and hence there is a need to remember the previous words. Thus, RNN came into existence, which solved this issue with the help of a Hidden Layer.

# How feedforward network is converted to a recurrent neural network? 🛠️

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1674020529006/019f9c1a-6e36-480e-b80f-96cdc7153594.png align="center")

In the Recurrent Neural Network principle, it combines all the hidden layers with the same weights and bias in a single recurrent layer. It’s like supplying the input to the hidden layer. At all times step weights of the recurrent neuron would be the same since it's a single neuron now. So a recurrent neuron stores the state of a previous input and combines it with the current input thereby preserving some relationship between the current input with the previous input.

# Applications of RNN 🎌

* Image capturing
    
* Machine Translation
    
* Speech Recognition
    
* Language Modelling and Generating Text
    
* Video Tagging
    
* Text Summarization
    
* Call Center Analysis
    
* Face detection, 
    
* Other applications also
    

We will discuss some major applications here-

### **Image capturing:**

RNN can detect the images and provide their descriptions in the form of tags.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1674021133368/21fdbc27-da50-4d04-b85e-5a3f50229cff.png align="left")

###  **Machine translation:**

RNNs can be used for translating text from one language to other. Currently one of the most popular and prominent machine translation applications is Google Translate. ECommerce application like Flipkart, Amazon, and eBay uses machine translation in many areas and it also helps with the efficiency of the search results.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1674021308475/0fbbb73c-0bf1-4bff-81af-524217771ea8.png align="center")

### **Speech recognition :**

Recurrent Neural Networks have replaced the traditional speech recognition models that made use of Hidden Markov Models. It can be used for predicting phonetic segments considering sound waves from a medium as an input source.

### **Sentiment analysis:**

RNNs are most adept at handling data sequentially to find the sentiments of the sentence.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1674021592123/030a6758-9df2-4412-95d6-13c7d7db58ea.png align="center")

### **Text summarization:**

RNN helps in summarizing content from literature and customizing them for delivery within applications that cannot support large volumes of text. For example, if a publisher wants to display the summary of one of his books on its back page to help the readers get an idea of the content present within, Text Summarization would be helpful.

# Types of RNN

1. **One to One -**
    
    It has a single input and a single output.
    
    Uses in simple machine learning problems.
    
2. **One to Many** \-
    
    It has a single input and multiple outputs.
    
    Example – image capturing.
    
3. **Many to One -**
    
    It takes a sequence of inputs and generates a single output. Example – sentiment analysis.
    
4. **Many to Many -**
    
    It takes a sequence of inputs and generates a sequence of outputs.
    
    Example – machine translation.
    

# Challenges faced by RNN 🤔

RNN is supposed to carry the information in time. However, it is quite challenging to propagate all this information when the time step is too long. When a network has too many deep layers, it becomes untrainable. This problem is called the vanishing gradient problem.

While training a neural network, if the slope tends to grow exponentially instead of decaying, this is called an Exploding Gradient. This problem arises when large error gradients accumulate, resulting in very large updates to the neural network model weights during the training process.

So readers, today we learned the basics about the recurrent neural network. I hope you enjoyed it. See you in the next blog. 😊