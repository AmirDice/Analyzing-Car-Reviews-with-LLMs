# Analyzing-Car-Reviews-with-LLMs
![car](https://github.com/user-attachments/assets/7dc811c0-6362-4aaf-9781-4e7353608314)

## Project Description

The task is to implement pre-trained large language model (LLM) use cases for tasks such as analyzing and classifying customer reviews on cars, responding to inquiries about available car models, and translating the company's English text data into other languages.

## Instructions and Steps

The CTO of *Car-ing is Sharing*, a car sales and rental company, has enlisted my expertise to prototype a chatbot application leveraging LLMs for diverse customer inquiries. As part of the pilot, i will complete the following tasks:  

- Utilize a pre-trained LLM to classify the sentiment of five car reviews in the `car_reviews.csv` dataset. Evaluate the classification accuracy and F1 score of the predictions.  
- Store the model outputs in `predicted_labels`, then map them to a binary list `{0,1}` named `predictions`.  
- Save the calculated metrics in `accuracy_result` and `f1_result`.  

To accommodate the company's growing Spanish customer base:  
- Extract the first two sentences of the first review and translate them from English to Spanish using an LLM.  
- Assess translation quality with the BLEU score, using `reference_translations.txt` as a reference.  
- Store the translated output in `translated_review` and the BLEU score in `bleu_score`.  

For brand-related insights:  
- Use an extractive QA LLM, such as `"deepset/minilm-uncased-squad2"`, to answer the question, *"What did he like about the brand?"* based on the second review.  
- Store the question and review text in `question` and `context`, respectively.  
- Save the extracted answer in `answer`.  

Lastly, summarize the final review in the dataset into approximately 50-55 tokens and store it in `summarized_text`.
