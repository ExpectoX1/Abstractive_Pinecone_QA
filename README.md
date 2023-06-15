# Abstractive_Pinecone_QA
An Abstractive Question Answering Software that uses Pinecone and Haystack to Generate answers to Questions.
Abstractive question generation creates new questions based on a dataset/context. It goes beyond the existing text, utilizing NLP and machine learning to generate coherent, relevant questions. It expands the question range and explores hypothetical scenarios. It’s almost the same as the generative method but here in this model, I used a model called “bart_lfqa”. One of the reasons GPT4All is slow is that it has to go through a lot of data and it is all done by the local machine, so a Library was used called “Pinecone”, Pinecone is a software that helps store vector images of all the data on a cloud platform and is fast in information retrieval. In terms of security, Pinecone is awarded a SOC 2 Type II Certificate. Again here as in the Extractive method, I am using Haystack for Document Store and document retrieval. This method can provide answers in less than 10 seconds (Tested on a Machine with Intel i7 and 32 GB RAM No GPU) with GPU the answers are almost instantaneous. To make the vector images for 47K documents it takes around 20 mins with a colab GPU. 



## Environment Setup 
if running on a local machine, make sure the following dependencies are installed.
To install run in the shell:

`pip install -U pinecone-client`
`pip install -U 'farm-haystack[pinecone]'>=1.8.0`
`pip install datasets`
`pip install torch`
`pip install transformers`

if you are trying to run the embedding function, be aware that it would be recommended to use a CUDA enables GPU as on CPU the Estimated Time of Completion is around 7 hours, with a GPU it's around 20 mins. 

Pinecone account and their free API is also required here to run the code. I have put a placeholder for it. 





