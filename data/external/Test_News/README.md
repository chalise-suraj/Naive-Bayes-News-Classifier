# External test news sample

This folder contains 95 English-language, COVID-19-related news articles from the CrossFake dataset. The text is included locally so the evaluation does not depend on the original pages remaining online.

## Selection and labels

- 20 `fake` and 75 `real` articles.
- English articles only (`type=article`), with the dataset's `mixed?` field marked `no`.
- Articles without cached English text were omitted. Exact title/body duplicates within this sample and exact normalized title/body matches against the project's original `Fake.csv` and `True.csv` were removed; none overlapped the original corpus.
- Labels follow CrossFake's fake/real metadata, which is grounded in existing English fact-checking information. These are inherited dataset labels, not new fact-checks performed for this project.
- This is a deliberately external COVID-19 sample, not a random sample of all world news. It is class-imbalanced and small; use macro F1 and per-class metrics, and interpret scores as a narrow transfer check.

## File

`external_test_news.csv` contains:

- `article_id`: stable source identifier
- `title`, `text`, `label`: model input fields and target (`fake`/`real`)
- `article_type`, `source_type`, `publish_date`: source metadata; exclude these from model input
- `fact_check_url`, `news_url`, `archive_url`: provenance links
- `mixed_content`: retained for audit; all included records are `no`

For inference, form the model input exactly as in Notebook 3: `title + "\n\n" + text`. Do not refit or tune on these examples.

## Attribution

Source: Du, Jiangshu; Dou, Yingtong; Xia, Congying; Cui, Limeng; Ma, Jing; Yu, Philip S. “Cross-lingual COVID-19 Fake News Detection.” ICDMW 2021. Dataset repository: <https://github.com/YingtongDou/CrossFake>. The repository's Apache-2.0 license is included as `LICENSE`. This sample is provided under those dataset terms; original article publishers remain identified in the source metadata/URLs.
