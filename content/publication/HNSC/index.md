---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "[IJCANN 2020] Hubness-based Sampling Method for Nystrom Spectral Clustering
"
authors: [Hongmin Li, Xiucai Ye, Akira Imakura, Tetsuya Sakurai]
date: 2020-10-14T17:58:00+09:00
doi: "10.1109/IJCNN48605.2020.9207089"

# Schedule page publish date (NOT publication's date).
publishDate: 2020-07-19T17:58:00+09:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "2020 International Joint Conference on Neural Networks (IJCNN)"
publication_short: "HNSC"

abstract: "Nyström method is widely used for spectral clustering to obtain low-rank approximations of a large matrix. Sampling is crucial to Nyström method, since selecting the representative sample points that can reflect the data structure is important for obtaining good approximation results. To improve the performance of Nyström based spectral clustering, in this paper, we propose a new sampling method by considering the hubness score of sample points. The data points with the high hubness scores, i.e., appearing frequently in the nearest neighbor lists of other data points, have high probabilities to be selected as the sample points. Taking advantage of the topological property of hubs (i.e., data points with high hubness score), the selected sampling points have close relationships with other data points, thus the proposed method is able to achieve scalable and accurate clustering results. We further design fast computation methods, i.e., local hubness approximated methods, to speed up the sampling process. Experimental results on both synthetic and real-world data sets show that the proposed method not only achieves good performance, but also outperforms other sampling methods for Nyström based spectral clustering."

# Summary. An optional shortened abstract.
summary: "An advanced Nyström spectral clustering methods based on Hubness."

tags: [Sampling methods,Matrix decomposition,Clustering methods,Sparse matrices,Approximation error,Mathematical model,Computational complexity]
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
