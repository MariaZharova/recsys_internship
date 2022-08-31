# Recommender systems research

### Лето 2022, ЦИАН

1). Запуск и исследование оригинальных моделей LightFM и SASRec (Microsoft recommenders):

- Test_LightFM.ipynb - запуск и тестирование модели LightFM

- Our_microsoft_recommender.ipynb - запуск и тестирование модели SASRec

- Compare_LightFM_and_Microsoft.ipynb - сравнение метрик LightFM и SASRec на одинаковых наборах данных

- Prepare data to compare LightFM and SASRec.ipynb - фильтрация данных для оценок в предыдущем файле

2). Подстановка конкретных nontrainable эмбеддингов объектов в SASRec (вместо рандомно генерируемых trainable):

- Embedding.ipynb - составление файла эмбеддингов объектов (415 признаков, категориальные + числовые)

- Embedding_num_only.ipynb - то же самое, но только для числовых признаков (25 шт)

- Merge_interships.ipynb - фильтрация эмбеддингов в соответствии с файлом кликстрима и в нужном порядке

- SASRec_with_embeddings.ipynb - подстановка эмбеддингов в модель

- Evaluate_SASRec_BIG_dataset_noEmb.ipynb и Evaluate_SASRec_BIG_dataset_withEmb.ipynb - оценка на одинаковых наборах данных моделей с эмбеддингами и без

- Change_WarpSampler.ipynb, Change_WarpSampler_2.ipynb - эмбеддинги теперь подаются не через модель, а через батч-итератор

- Bins_embeddings.ipynb - вариант группировки объектов "по бинам" в каждом признаке, составление файлов для этого случая


