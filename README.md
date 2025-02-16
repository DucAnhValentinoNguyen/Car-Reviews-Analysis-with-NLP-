# Car-Reviews-Analysis-with-NLP-

Goal: prototype a chatbot app addressing diverse inquiries using LLMs with car_reviews.csv dataswet

We use a pre-trained LLM to classify the sentiment of the five car reviews in the dataset, then evaluate the classification accuracy and F1 score of predictions.

From new customers in Spain we receive new reviews, where we extract and pass the first two sentences of the first review in the dataset to an English-to-Spanish translation LLMthen calculate the BLEU score to assess translation quality, using the content in reference_translations.txt as references.

The 2nd review in the dataset emphasizes brand aspects, there we want to load an extractive QA LLM (deepset/minilm-uncased-squad2) to formulate the question "What did he like about the brand?" and obtain an answer.

In the end we summarise the last review in the dataset, into approximately 50-55 tokens long.

The idea for this project is from a project in the learning platform Datacamp: https://projects.datacamp.com/projects/2046.
