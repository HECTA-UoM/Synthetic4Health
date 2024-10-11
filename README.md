# Synthetic4Health: Generating Annotated Synthetic Clinical Letters

A system to generate annotated, synthetic, de-identified clinical letters while protecting entities and document structure. 

This work presents a system for generating synthetic, de-identified clinical letters that are distinguishable from the originals, while preserving entities and document structures. We employed a hybrid approach, combining rule-based methods and named entity recognition (NER), to safeguard necessary information while exploring different models. We investigated various masking ratios and strategies based on token types (e.g., POS tags, stopwords) to balance diversity and similarity in synthetic letters. Our results demonstrate that this system produces high-quality synthetic clinical letters and is effective in protecting key information using encoder-only models, based on NER, POS tags, and stopword status.

# Abstract 
Since clinical letters contain sensitive information, clinical-related datasets can not be widely applied in model training, medical research, and teaching. This work aims to generate reliable, various, and de-identified synthetic clinical letters. We explored different pre-trained language models (PLMs) for masking and generating text to achieve this goal. After that, we worked on Bio\_ClinicalBERT, a high-performing model, and experimented with different masking strategies. Both qualitative and quantitative methods were used for evaluation. A downstream task, Named Entity Recognition (NER), was also implemented to assess the usability of these synthetic letters.
The results indicate that 1) encoder-only models outperform encoder-decoder models. 2) Among encoder-only models, those trained on general corpora perform comparably to those trained on clinical data when clinical information is preserved. 3) Additionally, preserving clinical entities and document structure better aligns with our objectives than simply fine-tuning the model. 4) Furthermore, different masking strategies can impact the quality of synthetic clinical letters. Masking stopwords has a positive impact, while masking nouns or verbs has a negative effect. 5) For evaluation, BERTScore should be the primary quantitative evaluation metric, with other metrics serving as supplementary references. 6) Contextual information does not significantly impact the models' understanding, so the synthetic clinical letters have the potential to replace the original ones in downstream tasks.

# cite us:
@misc{ren2024synthetic4healthgeneratingannotatedsynthetic,
      title={Synthetic4Health: Generating Annotated Synthetic Clinical Letters}, 
      author={Libo Ren and Samuel Belkadi and Lifeng Han and Warren Del-Pinto and Goran Nenadic},
      year={2024},
      eprint={2409.09501},
      archivePrefix={arXiv},
      primaryClass={cs.CL},
      url={ https://arxiv.org/abs/2409.09501 }, 
}

# new hosting repository: please visit
https://github.com/Libo-Ren/HECTA-UoM-Synthetic4Health
