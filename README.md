# Linguistic Metaphors Shape Attitudes Toward Immigration

This is an ongoing follow-up project to [Chkhaidze et al., 2021](https://escholarship.org/uc/item/1xf1t3vv), exploring how metaphorical framings (e.g., *flood*, *invasion*, *growth*) influence people’s attitudes toward immigration.

## Overview

We combine methods from computational and cognitive linguistics to analyze how language shapes beliefs about immigration.

### Key Components

- **Lexicon-based Analysis**  
  Custom metaphor lexicons are used to quantify metaphor usage in participant responses (both paraphrases and open-ended text).

- **LLM-Assisted Frame Detection**  
  We use zero-shot classification (via `facebook/bart-large-mnli`) and sentence embeddings (`all-MiniLM-L6-v2`) to assign conceptual frames to responses.

- **Sentiment-Aware Modeling**  
  RoBERTa-based sentiment scores are used to bias frame predictions (e.g., negative responses are more likely to reflect negative frames like *Resource Strain*).

- **Statistical Analysis**  
  OLS regression models examine how frame endorsement varies across metaphor conditions and political affiliations.

## Goals

- Understand how metaphors influence reasoning about social issues  
- Investigate how political identity interacts with metaphor framing  
- Build robust NLP pipelines to analyze narrative responses

## References
Chkhaidze, A., Buyruk, M., & Boroditsky, L. (2021). *Linguistic metaphors shape attitudes toward immigration*. Cognitive Science, 45(6), e12981.

Reimers, N., & Gurevych, I. (2019). Sentence-BERT: Sentence embeddings using Siamese BERT-networks. *Proceedings of the 2019 Conference on Empirical Methods in Natural Language Processing (EMNLP)*.

Yin, W., Hay, J., & Roth, D. (2019). Benchmarking zero-shot text classification: Datasets, evaluation and entailment approach. *Proceedings of the 2019 Conference on Empirical Methods in Natural Language Processing (EMNLP)*.

Wolf, T., Debut, L., Sanh, V., et al. (2020). Transformers: State-of-the-art natural language processing. In *Proceedings of the 2020 Conference on Empirical Methods in Natural Language Processing: System Demonstrations* (pp. 38–45).
