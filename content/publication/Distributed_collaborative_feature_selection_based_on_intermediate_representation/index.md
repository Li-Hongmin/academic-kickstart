---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "[IJCAI 2019] Distributed collaborative feature selection based on intermediate representation"
authors: [Xiucai Ye, Hongmin Li, Akira Imakura, Tetsuya Sakurai]
date: 2019-12-21T12:17:54+09:00
doi: "10.24963/ijcai.2019/575"

# Schedule page publish date (NOT publication's date).
publishDate: 2019-08-10T12:17:54+09:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: ""
publication_short: ""

abstract: "Feature selection is an efficient dimensionality reduction technique for artificial intelligence and machine learning. Many feature selection methods learn the data structure to select the most discriminative features for distinguishing different classes. However, the data is sometimes distributed in multiple parties and sharing the original data is difficult due to the privacy requirement. As a result, the data in one party may be lack of useful information to learn the most discriminative features. In this paper, we propose a novel distributed method which allows collaborative feature selection for multiple parties without revealing their original data. In the proposed method, each party finds the intermediate representations from the original data, and shares the intermediate representations for collaborative feature selection. Based on the shared intermediate representations, the original data from multiple parties are transformed to the same low dimensional space. The feature ranking of the original data is learned by imposing row sparsity on the transformation matrix simultaneously. Experimental results on real-world datasets demonstrate the effectiveness of the proposed method."

# Summary. An optional shortened abstract.
summary: "A novel distributed method which allows collaborative feature selection for multiple parties without revealing their original data."

tags: [Unsupervised Learning,Feature Selection,Learning Sparse Models,Dimensionality Reduction and Manifold Learning]
categories: []
featured: true

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_pdf:
url_code:
url_dataset:
url_poster:
url_project:
url_slides:
url_source:
url_video:

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: [research_paper]

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---
