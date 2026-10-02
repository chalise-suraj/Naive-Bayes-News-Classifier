# Primary dataset provenance

`Fake.csv` and `True.csv` in this folder match the file names, columns, class counts, and contents described by the **ISOT Fake News Dataset** from the Information Security and Object Technology (ISOT) Research Lab at the University of Victoria.

- [ISOT Lab dataset page](https://onlineacademiccommunity.uvic.ca/isot/)
- [ISOT dataset notes and citation instructions](https://onlineacademiccommunity.uvic.ca/isot/wp-content/uploads/sites/7295/2023/02/ISOT_Fake_News_Dataset_ReadMe.pdf)
- [Kaggle mirror](https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset), which lists **CC BY-NC-SA 4.0** for that mirror

The ISOT notes describe the real articles as collected from Reuters and fake articles as collected from sources flagged by Politifact and Wikipedia. The project labels records from their file names (`True.csv` → `real`; `Fake.csv` → `fake`); they are inherited dataset labels, not this project's independent article-by-article fact checks.

The exact download source and license terms for the copies in this project were not recorded. Before public redistribution, verify the applicable terms and attribution. Do not assume the Kaggle mirror's dataset-level license grants rights over every third-party article included in the files. These CSV files are each over 50 MiB; review the repository's large-file policy before pushing them to GitHub.

## Suggested scholarly citation

Ahmed, H., Traore, I., & Saad, S. (2018). “Detecting opinion spams and fake news using text classification.” *Journal of Security and Privacy*, 1(1). The ISOT dataset notes also cite their 2017 paper, “Detection of Online Fake News Using N-Gram Analysis and Machine Learning Techniques.”
