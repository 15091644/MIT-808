This folder explores an approach that matches the similarity of user queries to abstracts by comparing vector similarity. These vectors are dense vector contextual word embeddings generated from transformers. Thus a user can use natural language in their query.

DistilBERT was investigated. Other transformers can be investigated and experimented with.

The article for this tutorial can be found here: https://towardsdatascience.com/how-to-build-a-semantic-search-engine-with-transformers-and-faiss-dcbea307a0e8

This potentially provides an appropriate means to finding more relevant results, compared to training a classifier. The annotated classification information in the SDG data set can be used in outlier removal after this process has been called.

@Shaun we can think of ways to use the annotation and classification in downstream ranking as well. I potentially see this approach as the first major building block in our algorithm. 
