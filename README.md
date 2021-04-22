# Análise de sentimento com Word2Vec

Modelo criado para consolidar conhecimentos e estudos a respeito de word2vec.

Os dados obtidos através da api do kaggle contém reviews do IMDB com labels, essas reviews passam por um processo de data cleanning onde é retirado tags html, numeros, acentos, etc. Após isso, as reviews são transformadas em vetores através do modelo [en_core_web_sm'](https://spacy.io/models/en) do spacy. Esses vetores são analisados com um modelo [LogisticRegression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html) afim de identificar se o sentimento é positivo ou negativo.


Classification Report on Test Split:

| Precision  | Recall | F1-Score | Support | Data |
|---|---|---|---|---|
| Negative |0.70|0.71|0.71|5000|
| Positive |0.71|0.70|0.70|5000|
| Accuracy |   |   |0.70|10000|
| Macro AVG |0.70|0.70|0.70|10000|
| Weighted AVG |0.70|0.70|0.70|10000|


### Alguns Links:

[Dataset](https://www.kaggle.com/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews?rvi=1)<br>
[Documentação Spacy](https://spacy.io/)<br>
[Documentação Scikit-Learn](https://scikit-learn.org/stable/)<br>
[Sentiment Analysis with word2vec Word Embedding - KGP Talkie](https://www.youtube.com/watch?v=vF_qrJ0qHkg&ab_channel=KGPTalkie)
