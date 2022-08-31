# Recommender systems research

### Лето 2022, ЦИАН

1). Запуск и исследование оригинальных моделей LightFM и SASRec (Microsoft recommenders):

- Test_LightFM.ipynb - запуск и тестирование модели LightFM

- Sequential Recommendation Using Transformer.ipynb - копия эталонного ноутбука от Microsoft с примером запуска SASRec на amazon-датасете

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

3). Получение эмбеддингов пользователей из обычной модели

- SASRec_with_itemEmb_v4.ipynb, SASRec_with_userEmb_v1.ipynb, SASRec_with_userEmb_v3.ipynb - промежуточные результаты построения tsne-разложений эмбеддингов в разных размерностях для объектов и пользователей

- userEmbeddings_XGBoost_прикол.ipynb - код № 1 для итогового получения эмбеддингов пользователей, составление датасета (фичи - эмбеды пользователей, таргет - предпочтения в аренде/продаже) и обучение на нём XGBoost

- Final_user_item_emb.ipynb - финальная версия кода предыдущего назначения:)

- Итоги_стажировки.pdf - вся история кратко в одной презентации



