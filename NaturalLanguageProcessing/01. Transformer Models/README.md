## [Hugging Face - Transformers Model](https://huggingface.co/docs/transformers/index)

In the [Transformers Model](https://github.com/regmi-saugat/HuggingFace/blob/main/Transformer%20Models/Transformer%20Models.ipynb) notebook, I have listed some common tasks performed using Hugging Face `Transformers` Model. This contains tasks like *Sentiment Analysis*, *Zero-Shot Classification*, *Text Generation*, *Mask Filling*, *Named Entity Recognition*, *Question Answering*, *Summarization* and *Language Translation*.

---

**Natural Language Processing**
- NLP is a field of linguistics and machine learning focused on understanding everything related to human language. The aim of the NLP task is not only to understand single words individually but to be able to understand the context of those words.

*Common NLP Tasks*

- Classifying whole sentences
- Classifying each word in a sentence
- Generating text context
- Extracting an answer from a text
- Generating a new sentence from an input text

**Why it is challenging**

- Computers don’t process information in the same way as humans. For example, when we read the sentence “I am hungry,” we can easily understand its meaning. Similarly, given two sentences such as “I am hungry” and “I am sad,” we’re able to easily determine how similar they are. For machine learning (ML) models, such tasks are more difficult. The text needs to be processed in a way that enables the model to learn from it.

----

![Images](../Images/01.%20transformer_model.png)

**1. Sentiment Analysis**
- It is a branch of natural language processing, which involves the emotional tone or sentiment expressed in text.

**2. Zero-shot classification**
- It is a machine learning technique that is used to classify the input data into multiple categories or classes, even if the model has not been explicitly trained on those categories during training phase.
- It allows the model to make predictions about classes it has never seen before.
- It majorly relies on the idea that language and semantic understanding can help bridge the gap between known and unknown classes

**3. Text Generation**
- The main idea of text generation is that when we provide a prompt and the model will auto-complete it by generating the remaining text.
- It is similar to the predictive text feature that is found on many phones.
- We can give several arguments like `num_return_sequences` and `max_length` to generate any sentences

**4. Mask Filling**
- The idea of mask filling is to fill the blanks in a given text
- The argument `top_k` is to control how many possibilities we want to display. The model fills in the special `<mask>` word, which is often referred as *mask token*.

**5. Named Entity Recognition**
NER pipeline identifies entities such as persons, organizations, or locations in a sentence.
- When we pass `grouped_entities=True` in the pipeline creation function to tell the pipeline to regroup together the parts of the sentences that correspond to the same entity.

**6. Question Answering**
- This pipeline helps answering the questions using information given from the context.

**7. Summarization**
- Summarization helps in the task reducing a text into a shorter text while keeping all of the important aspects referenced in the text

**8. Language Translation**
- This pipeline helps in translating the words or sentences from one langauge to another lanauge
- We can specify `max_length` or `min_length` for the result
