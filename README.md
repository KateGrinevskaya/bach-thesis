# Автоматическое выделение толкований терминов в текстах
## Выпускная квалификационная работа Гриневской Екатерины Сергеевны

### Последовательное обучение
#### Обучение бинарного классификатора
- `finetune_Bert_multiling_case.ipynb` - обучение и расчёт метрик качества BERT c использованием модели [bert-base-multiligual-cased](https://huggingface.co/bert-base-multilingual-cased)
- `finetune_Bert_multiling_uncase.ipynb` - обучение и расчёт метрик качества BERT c использованием модели [bert-base-multiligual-uncased](https://huggingface.co/bert-base-multilingual-uncased)
- `bertCRF_rubert.ipynb` - обучение и расчёт метрик качества BERT c использованием модели [DeepPavlov/rubert-base-cased](https://huggingface.co/DeepPavlov/rubert-base-cased)
#### Обучение классификатора на 5 классов (разметка последовательности)
- `feats sklearn.ipynb` - обучение и расчёт метрик качества CRF от [sklearn](https://scikit-learn.org/) с текстовыми признаками
- `embs sklearn.ipynb` - обучение и расчёт метрик качества CRF от [sklearn](https://scikit-learn.org/) с эмбеддингами в качестве признаков
- `feats+embs sklearn.ipynb` - обучение и расчёт метрик качества CRF от [sklearn](https://scikit-learn.org/) с текстовыми признаками и эмбеддингами в качестве признаков
- `bertCRF_rubert.ipynb` - обучение и расчёт метрик качества CRF от [pytorch](https://pytorch-crf.readthedocs.io/en/stable/) с эмбеддингами в качестве признаков

### Одновременное обучение

- `bertCrf_2heads.ipynb` - обучение BERT c использованием модели [DeepPavlov/rubert-base-cased](https://huggingface.co/DeepPavlov/rubert-base-cased) и CRF от [pytorch](https://pytorch-crf.readthedocs.io/en/stable/) с эмбеддингами в качестве признаков и расчёт метрик качества
