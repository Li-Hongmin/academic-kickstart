---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "[ICMD 2020] Ensemble Learning for Spectral Clustering"
authors: [Hongmin Li, Xiuca Ye, Akira Imakura, Tetsuya Sakurai]
date: 2020-10-14T18:06:04+09:00
doi: "10.1109/ICDM50108.2020.00131"

# Schedule page publish date (NOT publication's date).
publishDate: 2020-10-14T18:06:04+09:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: ""
publication_short: ""

abstract: "Ensemble clustering has attracted much attention in machine learning and data mining for the high performance in the task of clustering. Spectral clustering is one of the most popular clustering methods and has superior performance compared with the traditional clustering methods. Existing ensemble clustering methods usually directly use the clustering results of the base clustering algorithms for ensemble learning, which cannot make good use of the intrinsic data structures explored by the graph Laplacians in spectral clustering, thus cannot obtain the desired clustering result. In this paper, we propose a new ensemble learning method for spectral clustering-based clustering algorithms. Instead of directly using the clustering results obtained from each base spectral clustering algorithm, the proposed method learns a robust presentation of graph Laplacian by ensemble learning from the spectral embedding of each base spectral clustering algorithm. Finally, the proposed method applies k-means on the spectral embedding obtain from the learned graph Laplacian to get clusters. Experimental results on both synthetic and real-world datasets show that the proposed method outperforms other existing ensemble clustering methods."

# Summary. An optional shortened abstract.
summary: ""

tags: []
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
