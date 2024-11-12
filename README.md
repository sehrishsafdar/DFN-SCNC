DFN-SCNC: Detecting Fake News based on Social Context and News Content: A Hybrid Approach using BERT and Bi-GRU
**Dataset**
The dataset was gathered using a combination of scraping techniques and tools.Due to the large size of the Facebook data, a subset was created please email at sehrishsafdar3@gmail.com for the complete dataset.
**Tools and Libraries Used**
**Selenium**: Used to navigate and interact with PolitiFact's website, enabling automated data extraction for posts.
**BeautifulSoup**: Parsed the HTML content collected by Selenium to efficiently extract post details.
**Apify**: A powerful tool for scraping comment threads, used to collect all comments associated with each PolitiFact post.
**Methodology**
we present the explanation of our proposed DFN-SCNC model. We start by extracting the title and comments from the news.
Next, the BERT model tokenizes the title and comments, with each token represented as w, and feeds it to the fine-tuned
BERT model to extract contextual features. Later, A BiGRU layer processes these embeddings, reading the sequence in both
forward and backward directions and capturing dependencies from previous and future contexts. The BiGRU layer's outputs
are pooled in a hidden layer and sent through a softmax layer to generate a probability distribution over potential
classifications, such as true or false news. The class with the highest probability is selected as the prediction.
The combination of deep contextual knowledge from BERT and sequential processing from BiGRU allows the model to 
efficiently distinguish between authentic and fraudulent news, improving the reliability and accuracy of fake news detection systems
**BERT + Bi-GRU Model for Text Classification**
The Bert+bi-gru.py guides building a BERT + Bi-GRU model for text classification.
In this process we applying the BERT + Bi-GRU model for classification.




