Fake News Detection for Financial Risk Management

Project Overview:

This project addresses the material threat that misinformation poses to quantitative trading systems and market sentiment models. When fabricated content enters analytical pipelines, sentiment scores become polluted, leading to alpha signal degradation and misfiring risk models.


I developed and compared two distinct NLP pipelines to determine the most effective way to filter this "noise" in a high-stakes financial environment.

Key Findings:


Model Performance: The "old-school" TF-IDF + Logistic Regression model achieved 98.50% accuracy, handily beating the more complex Sentence-BERT (SBERT) embedding approach which reached 95.52%.




Thematic Risks: Using Non-negative Matrix Factorization (NMF), I identified that misinformation in this dataset (2016-2017) is heavily concentrated in seven political themes, such as Clinton scandals and FBI/Russia investigations.




Operational Advantage: For latency-sensitive trading, the TF-IDF approach is superior as it runs efficiently on commodity hardware without the need for expensive GPU infrastructure.


Methodology:


Data: Analyzed a corpus of 44,898 news articles (approx. 52% fake / 48% real).


Preprocessing: Implemented a pipeline for case normalization, noise removal (URLs, HTML), and title-body concatenation to preserve headline signals.


Classification: Evaluated a sparse lexical-statistical approach (TF-IDF) against dense semantic embeddings (SBERT all-MiniLM-L6-v2).



Topic Modeling:

Deployed NMF with seven components to discover latent thematic structures within the misinformation subset.


Repository Structure:


Fake_News_Analysis.ipynb: Full Python implementation including data splitting, training, and evaluation.


DSK822_FakeNews_Paper_Final.docx: The final strategic analysis prepared for the Risk and Media Analytics Division.

Contact:

Nischal Ranabhat | niran24@student.sdu.dk Prepared for DSK822: News and Market Sentiment Analytics | December 2025
