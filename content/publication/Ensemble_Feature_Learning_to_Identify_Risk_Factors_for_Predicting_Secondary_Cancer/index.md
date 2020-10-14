---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Ensemble Feature Learning to Identify Risk Factors for Predicting Secondary Cancer"
authors: [Xiucai Ye, Hongmin Li, Tetsuya Sakurai, Pei-Wei Shueng]
date: 2019-12-22T18:43:03+09:00
doi: "10.7150/ijms.33820"

# Schedule page publish date (NOT publication's date).
publishDate: 2019-7-22T18:43:03+09:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: ""
publication_short: ""

abstract: "
Background: In recent years, the development and diagnosis of secondary cancer have become the primary concern of cancer survivors. A number of studies have been developing strategies to extract knowledge from the clinical data, aiming to identify important risk factors that can be used to prevent the recurrence of diseases. However, these studies do not focus on secondary cancer. Secondary cancer is lack of the strategies for clinical treatment as well as risk factor identification to prevent the occurrence.


Methods: We propose an effective ensemble feature learning method to identify the risk factors for predicting secondary cancer by considering class imbalance and patient heterogeneity. We first divide the patients into some heterogeneous groups based on spectral clustering. In each group, we apply the oversampling method to balance the number of samples in each class and use them as training data for ensemble feature learning. The purpose of ensemble feature learning is to identify the risk factors and construct a diagnosis model for each group. The importance of risk factors is measured based on the properties of patients in each group separately. We predict secondary cancer by assigning the patient to a corresponding group and based on the diagnosis model in this corresponding group.


Results: Analysis of the results shows that the decision tree obtains the best results for predicting secondary cancer in the three classifiers. The best results of the decision tree are 0.72 in terms of AUC when dividing the patients into 15 groups, 0.38 in terms of F1 score when dividing the patients into 20 groups. In terms of AUC, decision tree achieves 67.4% improvement compared to using all 20 predictor variables and 28.6% improvement compared to no group division. In terms of F1 score, decision tree achieves 216.7% improvement compared to using all 20 predictor variables and 80.9% improvement compared to no group division. Different groups provide different ranking results for the predictor variables.


Conclusion: The accuracies of predicting secondary cancer using k-nearest neighbor, decision tree, support vector machine indeed increased after using the selected important risk factors as predictors. Group division on patients to predict secondary cancer on the separated models can further improve the prediction accuracies. The information discovered in the experiments can provide important references to the personality and clinical symptom representations on all phases of guide interventions, with the complexities of multiple symptoms associated with secondary cancer in all phases of the recurrent trajectory."

# Summary. An optional shortened abstract.
summary: "An effective ensemble feature learning method to identify the risk factors for predicting secondary cancer by considering class imbalance and patient heterogeneity."

tags: [secondary cancer, risk factors, class imbalance, patient heterogeneity, spectral clustering, ensemble learning]
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
