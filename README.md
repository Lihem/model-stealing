# Model Stealing with Wise Query Selection
## Abstract:
Model stealing is an important field of data privacy and machine learning, where an attacker replicates the functionality of a target model by querying it and using the responses to train a clone model. This work aims to improve the efficiency of model stealing by reducing the number of queries required. Traditional model stealing approaches rely heavily on extensive querying, which can be costly and risk detection. We propose two novel heuristics to optimize query selection: one that encourages dissimilarity with previous queries to ensure diverse coverage of the input space, and another that targets similarity with queries that the clone model predicts poorly to improve areas where the clone model previously underperformed.

Our methodology involves maintaining a comprehensive table of past queries, their embeddings, and the outputs from both the target and clone models. By calculating an effectiveness score for each candidate query based on these heuristics, we select the optimal queries to send to the target model. This approach aims to minimize the number of queries while maintaining the effectiveness of the cloned model. Experimental results demonstrate that our heuristic-driven query selection reduces the query load compared to traditional methods, achieving comparable accuracy, loss, and F1 score metrics. This work highlights the potential of heuristic-based query optimization for increasing the stealth and efficiency of model stealing.

For more details, you can read our [project report](./Report.pdf).

---


<img width="1263" height="463" alt="train" src="https://github.com/user-attachments/assets/c22d5fc7-d14b-4ddc-b81a-ce7b1b33c69b" />
