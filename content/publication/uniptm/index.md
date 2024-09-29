---
title: 'UniPTM: Multiple PTM site prediction on full-length protein sequence'

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

date: '2024-08-06'
doi: 10.1101/2024.08.03.606471

# Schedule page publish date (NOT publication's date).
publishDate: '2022-11-15T00:00:00Z'

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ['3']

# Publication name and optional abbreviated publication name.
publication: In ***bioRxiv***
publication_short: In **_bioRxiv_** 2024.08.03.606471

Abstract: Post-translational modifications (PTMs) enrich the functional diversity of proteins by attaching chemical groups to the side chains of amino acids. In recent years, a myriad of AI models have been proposed to predict many specific types of PTMs. However, those models typically adopt the sliding window approach to extract short and equal-length protein fragments from full-length proteins for model training. Unfortunately, such a subtle step results in the loss of long-range information from distal amino acids, which may impact the PTM formation process. In this study, we introduce UniPTM, a window-free model designed to train and test on natural and full-length protein sequences, enabling the prediction of multiple types of PTMs in a holistic manner. Moreover, we established PTMseq, the first comprehensive dataset of full-length protein sequences with annotated PTMs, to train and validate our model. UniPTM has undergone extensive validations and significantly outperforms existing models, elucidating the influence of protein sequence completeness on PTM. Consequently, UniPTM offers interpretable and biologically meaningful predictions, enhancing our understanding of protein functionally and regulation. The source code and PTMseq dataset for UniPTM are available at https://www.github.com/TransPTM/UniPTM.

# Summary. An optional shortened abstract.
summary:

tags: []

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org
links:
  - name: bioRxiv
    url: https://www.biorxiv.org/content/10.1101/2024.08.03.606471v1
  - name: Source Code
    url: https://www.uniptm.com
url_pdf: uploads/uniptm.pdf

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  caption: ''
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
<p style='text-align: justify;'> 1. UniPTM takes full-length protein sequence data as input, considering all amino acids across the entire protein that could influence the occurrence of PTMs, even if they are distal. </p>
<p style='text-align: justify;'> 2. PTMseq dataset consists subsets of nine types of PTMed sequences, currently encompassing a total of 34,514 distinct PTM sites annotated across 12,203 full-length protein sequences. </p>
<p style='text-align: justify;'> 3. The pre-trained ESM-2 model embeds contextual information from the entire sequence into each residue, allowing every target amino acid to engage independently. </p>

Supplementary Information can be accessed [**here**](uploads/uniptm-si.pdf).
