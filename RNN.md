### RNN ###

1. Definition

An RNN (Recurrent Neural Network) is a type of neural network designed to handle sequential data — data where the order matters.

2. It’s commonly used in:
   

-> Speech recognition

-> Text generation

->  Music prediction

-> Time-series forecasting


-> How does it work?


Unlike traditional neural networks (which treat all inputs independently), RNNs remember past information using a loop inside their architecture. Here's the idea:

       Output at time t = f(current input at time t + memory from time t-1)
So, what you input before affects the output now.

3.  **Example:**
Let’s say you’re trying to predict the next word in this sentence:

"I am going to the ___"

A regular neural network would just look at “the”.
But an RNN remembers what came before (“I am going to the”) — so it can guess something like “store”, “gym”, etc.

4.  **Memory Flow**
   
At every step:

->It takes the current input

->Combines it with the previous hidden state (memory)

->Outputs a prediction and updates its memory

5.  **RNN Limitations**
    
-> Forgets long-term information (early words are "forgotten" over time)

-> Training can be slow due to issues like vanishing gradients

-> To fix this, advanced versions like LSTM and GRU were created, which have better memory handling.


### What is Augmentation of Duplicated Rows? ###

In natural language processing (NLP) or machine learning in general, augmentation refers to creating new, slightly modified versions of existing data to improve model training.

So, when someone says:

"Augmentation of duplicated rows"

They might mean one of two things, depending on context:

 **1. Replacing or Modifying Duplicate Rows to Create Variants**
Instead of just deleting duplicate rows, you apply text augmentation techniques to turn them into new, slightly different samples — to retain data quantity but avoid exact repetition.

Example:
Original duplicated post:

“I love this community. You guys are awesome!”

Augmented variants:

“This community is amazing. I love you all!”

“You folks are incredible — I really enjoy being here.”

“This is such a great place! Everyone is awesome.”

This could be done using:

Synonym replacement

Back translation (translate to another language and back)

Random word deletion/insertion

Paraphrasing using NLP models


