# HECTA-UoM-Synthetic4Health
A system to generate synthetic, de-identified clinical letters while protecting entities and document structure. 

This work presents a system for generating synthetic, de-identified clinical letters that are distinguishable from the originals, while preserving entities and document structures. We employed a hybrid approach, combining rule-based methods and named entity recognition (NER), to safeguard necessary information while exploring different models. We investigated various masking ratios and strategies based on token types (e.g., POS tags, stopwords) to balance diversity and similarity in synthetic letters. Our results demonstrate that this system produces high-quality synthetic clinical letters and is effective in protecting key information using encoder-only models, based on NER, POS tags, and stopword status.

Pre-print paper: [https://arxiv.org/abs/2409.09831](url)
