# Transformer - Attention Mechanism
Attention is all you need (Vaswani, Ashish & Shazeer, Noam & Parmar, Niki & Uszkoreit, Jakob & Jones, Llion & Gomez, Aidan & Kaiser, Lukasz & Polosukhin, Illia. (2017))
## What is attention?
Finding the relationship btw the words. When the words have a similar meaning, they are close in a vector space.

if we look at the word text and message itself, we are not sure it it means texting as an action or text in a newspaper. so, we use attention in order to understand what exactly the words means in a sentence so, we look at all the tokens in the sentence and are able to know what the token(=word) actually means in attention. because we have text and message together in a sentence, we know that text means sending a text actionwise and message is a message we send to the other person.

# GPT-1
- Introduced by OpenAI in 2018
- Unsupervised training
- Predicts the next word from the previous words, great for sentence generation
  - ex) if the input is ‘how are you’, ‘doing’ is predicted in GPT.
- it only uses the decoder part in transformer
- 117 million parameters and 12 Decoder layers 
- 4.5GB BookCorpus dataset is used for pre-training
- left to right direction decoder. 
- input should be a sentence, input maximum is 512 tokens
- human doesn’t need to label the data one by one, we just needs immense amount of data

After GPT-1 was published, BERT was introduced by Google (Google made transformer).
Google points out that GPT-1 has flaws as it is unidirectional. If we want to understand the full context and predict the next words, it should be bidirectional, thus Google introduced BERT(bidirectional encoder representations from transformer). 


# BERT(Bidirectional Encoder Representations from Transformers)
- Introduced by Google in 2018
- predicts the masked words
  - ex) if the input is ‘how are <mask> doing’, ‘you’ is predicted in BERT
- bidirectional (left to right, right to left) encoder.
- input doesn’t have to be a sentence, it can be two sentences as well
- human doesn’t need to label the data one by one, we just needs immense amount of data

After BERT was published, GPT-2 was introduced by OpenAI.
GPT-2 has improved BERT’s accuracy by 4.17~5.31% and training time improved from 104s to 116s.

# GPT-2
- Introduced by OpenAI in 2019
- Same structure as GPT-1 but it has more parameters and decoder layers
- Predicts the next word from the previous words, great for sentence generation
  - ex) if the input is ‘how are you’, ‘doing’ is predicted in GPT.
- has 1.5 billion parameters and 48 Decoder layers 
- bidirectional (left to right, right to left) encoder. 
- Zero-shot Performance: able to categorize a new class that is not seen/labelled during the training. - If the model has learnt about a cow, zebra, the model can label a new object as a horse
- input should be a sentence, input maximum is 1024 tokens
- human doesn’t need to label the data one by one, we just needs immense amount of data

After GPT-2 was published, GPT-3 was introduced by OpenAI.
GPT-3 is significantly larger than GPT-2, GPT-3 is slower than GPT-2. GPT-3 can learn complex relationships between words and sentences. GPT-3 requires more computational resources. 

# GPT-3
- Introduced by OpenAI in 2020
- same structure as GPT-1 but has more transformer layers
- it is a larger model than GPT-2
- predicts the masked words
  -ex) if the input is ‘how are <mask> doing’, ‘you’ is predicted in BERT
- bidirectional (left to right, right to left) encoder. 
- Zero-shot Performance: able to categorize a new class that is not seen/labelled during the training. - If the model has learnt about a cow, zebra, the model can label a new object as a horse
- input should be a sentence, input maximum is 2048 tokens
- Few-shot Performance: able to categorize a class with just a few training dataset
- input doesn’t have to be a sentence, it can be multiple sentences as well
- doesn’t need fine tuning
- human doesn’t need to label the data one by one, we just needs immense amount of data

After GPT-2 was published, DALL-E was introduced by OpenAI.
DALL-E creates an image via text. It is similar to GPT-3 except DALL-E is giving an image as an output and GPT-3 is giving a text as an output

# DALL-E
- Introduced by OpenAI in 2021
- creates an image via text
- text has been changed to pixel in GPT-3
- bidirectional (left to right, right to left) encoder. 
