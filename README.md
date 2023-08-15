# LS-Neural-Networks-and-LLMs-Final-Project

This project aims to fight the spread of false information and disinformation in the current digital environment. Leveraging the power of BERT (Bidirectional Encoder Representations from Transformers), a state-of-the-art natural language processing model, this project addresses the critical need for accurate and efficient identification of fake news articles.


Dataset used :- https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset
We have two separate .csv files, one having the real news, called 'true.csv' and another one, having the fake news, called 'fake.csv'.

Then, we obtain the pre-trained BERT model to use as the base of our Fake News Detection Model using HuggingFace’s Transformers library. BERT has insane language comprehension capability. So, it shall make our model better understand news context and hence make intelligent predictions on news being fake or not.

We freeze the weights on the starting layers from BERT, then we create new trainable Layers. To predict the model’s specialized tasks, we must add additional layers on top of them. Additionally, we define a new output layer, as the final output of the pre-trained model will almost certainly differ from the output we want for our model, which is binary 0 and 1.

As the last step we fine-tune our model. And once we are done, we move on to make predictions using our Fake News Detection Model on unseen data.

