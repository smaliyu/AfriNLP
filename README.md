# AfriNLP

We focused on training four distinct models to analyze tweet datasets in three major Nigerian languages: Hausa, Igbo, and Yoruba. This endeavor involved a standardized PyTorch workflow, complemented by the extensive model repository available on Huggingface. The choice of Huggingface facilitated the use of advanced NLP models, each with its unique architecture but primarily encoder-based, similar to BERT.

To manage our language-specific datasets effectively, we developed a custom dataset class. This class was tailored to the unique characteristics of the Hausa, Igbo, and Yoruba languages, addressing specific text preprocessing and encoding needs. The use of PyTorch’s DataLoader was instrumental in handling the data efficiently in batches, optimizing computational resources.

A critical component of our methodology was leveraging AutoModel and AutoTokenizer from Huggingface. These tools enabled us to accommodate various model architectures seamlessly. AutoModel adapted dynamically to each model’s architecture, while AutoTokenizer ensured consistent and appropriate tokenization and encoding of our multilingual text data. This approach was particularly beneficial given the linguistic nuances of Hausa, Igbo, and Yoruba tweets.

The overarching aim of training these models was to distinguish and learn the class-specific features inherent in the tweet datasets of these three languages. By utilizing pretrained models and fine-tuning them on our datasets, we were able to harness pre-existing knowledge and adapt it to the context of Nigerian languages.

Finally, we evaluated the performance of each model on separate test sets for Hausa, Igbo, and Yoruba tweets. This evaluation primarily measured the models' accuracy, offering vital insights into their effectiveness in classifying tweets accurately across these languages.
