# Nlp_Project

Dataset to be used:
https://huggingface.co/datasets/squad
In this project, I utilized the Hugging Face Transformers library to implement a 
question-answering system. The model used was "deepset/bert-base-cased-squad2", which was 
pretrained on the SQuAD v2 dataset.
Installing required packages
First installed the transformers package using !pip install transformers.
Importing a Question Answering Class from Transformers
The BertForQuestionAnswering class was imported from the transformers package to initialize 
the model for question answering.
Importing the Model
Imported the "deepset/bert-base-cased-squad2" model and used it to answer 
questions based on a given context.
Defining Context and Questions
The context and questions were defined using data from Imran Khan's Wikipedia page.
Tokenizer
The tokenizer was initialized using AutoTokenizer.from_pretrained('deepset/bert-base-casedsquad2'). The tokenizer is responsible for converting strings of questions and answers into a 
format understandable by the BERT model.
Set Up Tokenizer and Model into a Q&A Pipeline
Set up a pipeline using the transformers library that takes an input dictionary 
containing a question and context, and returns an output dictionary with the model's confidence 
score, start and end indices of the answer in the context, and the answer itself.
Testing on All Questions
Finally, tested our question-answering system on all questions using the given 
context. The model returned answers along with confidence scores for each question.
Output:
Question: Who is Imran Khan?
Answer: a Pakistani politician
Score: 0.455
Question: What are Imran Khan's achievements?
Answer: Considered one of cricket's greatest all-rounders
Score: 0.3033
Question: What is Imran Khan's political party?
Answer: Pakistan Tehreek-e-Insaf
Score: 0.5698
Question: When did Imran Khan graduate from the University of Oxford?
Answer: 1975
Score: 0.9702
Question: Which cricket team did Imran Khan captain?
Answer: Pakistan Tehreek-e-Insaf (PTI
Score: 0.0024
Question: When did Imran Khan retire from cricket?
Answer: 1996
Score: 0.6242
Question: How many runs and wickets did Imran Khan achieve in Test cricket?
Answer: 362
Score: 0.9134
Question: What social initiatives did Imran Khan establish?
Answer: poverty alleviation programs
Score: 0.758
Question: When was Imran Khan elected as the Prime Minister of Pakistan?
Answer: August 2018 until April 2022
Score: 0.5098
Question: What were Imran Khan's main focuses during his tenure as Prime 
Minister?
Answer: anti-corruption measures, education, healthcare, and poverty 
alleviation programs
Score: 0.719
