---
title: 'TransPTM: a transformer-based model for non-histone acetylation site prediction'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Lingkuan Meng
  - Xingjian Chen
  - admin
  - Nanjun Chen
  - Zetian Zheng
  - Fuzhou Wang
  - Hongyan Sun
  - Ka-Chun Wong

date: '2024-05-09'
doi: 10.1093/bib/bbae219

# Schedule page publish date (NOT publication's date).
publishDate: '2022-11-15T00:00:00Z'

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ['2']

# Publication name and optional abbreviated publication name.
publication: In ***Briefings in Bioinformatics***
publication_short: In **_Brief. Bioinform_** 2024, _25_, bbae219

Abstract: Protein acetylation is one of the extensively studied post-translational modifications (PTMs) due to its significant roles across a myriad of biological processes. Although many computational tools for acetylation site identification have been developed, there is a lack of benchmark dataset and bespoke predictors for non-histone acetylation site prediction. To address these problems, we have contributed to both dataset creation and predictor benchmark in this study. First, we construct a non-histone acetylation site benchmark dataset, namely NHAC, which includes 11 subsets according to the sequence length ranging from 11 to 61 amino acids. There are totally 886 positive samples and 4707 negative samples for each sequence length. Secondly, we propose TransPTM, a transformer-based neural network model for non-histone acetylation site predication. During the data representation phase, per-residue contextualized embeddings are extracted using ProtT5 (an existing pre-trained protein language model). This is followed by the implementation of a graph neural network framework, which consists of three TransformerConv layers for feature extraction and a multilayer perceptron module for classification. The benchmark results reflect that TransPTM has the competitive performance for non-histone acetylation site prediction over three state-of-the-art tools. It improves our comprehension on the PTM mechanism and provides a theoretical basis for developing drug targets for diseases. Moreover, the created PTM datasets fills the gap in non-histone acetylation site datasets and is beneficial to the related communities. The related source code and data utilized by TransPTM are accessible at https://www.github.com/TransPTM/TransPTM.

# Summary. An optional shortened abstract.
summary:
tags: []

# Display this page in the Featured widget?
featured: no

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org
links:
  - name: Oxford University Press
    url: https://academic.oup.com/bib/article/25/3/bbae219/7667560#449115313
  - name: PubMed
    url: https://pubmed.ncbi.nlm.nih.gov/38725156
  - name: Source Code
    url: https://www.github.com/TransPTM/TransPTM
url_pdf: uploads/bbae219.pdf

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  caption: 'Copyright © 2024 Oxford University Press'
  focal_point: ''
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
---

**Highlights:**

<p style='text-align: justify;'> 1. A transformer-based deep learning model is proposed for non-histone acetylation site prediction, which achieves the best performance among the state-of-the-art models. </p>
<p style='text-align: justify;'> 2. The establishment of NHAC, a benchmark dataset specifically designed for non-histone acetylation site prediction, enriches the landscape of lysine acetylation site databases. </p>
<p style='text-align: justify;'> 3. Pre-trained protein language model ProtT5 is employed for generating contextualized representations of protein sequences by capturing dependencies between amino acid residues. </p>
<p style='text-align: justify;'> 4. The self-attention mechanism in TransPTM can reveal key residue positions for non-histone protein acetylation, thereby demonstrating the interpretability of our model. </p>

Supplementary Information can be accessed [**here**](uploads/supplementary_material_bbae219.pdf).
