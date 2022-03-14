This folder explores an approach that matches the similarity of user queries to abstracts by comparing vector similarity. These vectors are dense vector contextual word embeddings generated from transformers. Thus a user can use natural language in their query.

DistilBERT was investigated. Other transformers can be investigated and experimented with.

One can also look at this blog for more information: https://towardsdatascience.com/the-auto-sommelier-how-to-implement-huggingface-transformers-and-build-a-search-engine-9e0f401b1bda

And: https://www.sbert.net/examples/applications/semantic-search/README.html

Sentence transformers are used in:

Repositories using SentenceTransformers (worth checking these libraries out for EDA):

haystack - Neural Search / Q&A

Top2Vec - Topic modeling

txtai - AI-powered search engine

BERTTopic - Topic model using SBERT embeddings

KeyBERT - Key phrase extraction using SBERT

contextualized-topic-models - Cross-Lingual Topic Modeling

covid-papers-browser - Semantic Search for Covid-19 papers

backprop - Natural Language Engine that makes using state-of-the-art language models easy, accessible and scalable.

Note that query length is important: Transformer models like BERT / RoBERTa / DistilBERT etc. the runtime and the memory requirement grows quadratic with the input length. This limits transformers to inputs of certain lengths. A common value for BERT & Co. are 512 word pieces, which corresponds to about 300-400 words (for English). Longer texts than this are truncated to the first x word pieces.

This potentially provides an appropriate means to finding more relevant results, compared to training a classifier. The annotated classification information in the SDG data set can be used in outlier removal after this process has been called.

@Shaun we can think of ways to use the annotation and classification in downstream ranking as well. I potentially see this approach as the first major building block in our algorithm.
