# Обучение модели классификации комментариев

Интернет-магазин «Викишоп» запускает новый сервис. Теперь пользователи могут редактировать и дополнять описания товаров, как в вики-сообществах. То есть клиенты предлагают свои правки и комментируют изменения других. Магазину нужен инструмент, который будет искать токсичные комментарии и отправлять их на модерацию. 

Надо обучить модель классифицировать комментарии на позитивные и негативные. В нашем распоряжении набор данных с разметкой о токсичности правок.

Постройте модель со значением метрики качества *F1* не меньше 0.75. 

**Инструкция по выполнению проекта**

1. Загрузить и подготовить данные.
2. Обучить разные модели. 
3. Сделать выводы.

**Описание данных**

Данные находятся в файле `toxic_comments.csv`. Столбец *text* в нём содержит текст комментария, а *toxic* — целевой признак.

| text | toxic |
|------|-------|	
|	Explanation\nWhy the edits made under my usern...|	0|
|	D'aww! He matches this background colour I'm s...|	0|
|	Hey man, I'm really not trying to edit war. It...|	0|
|	"\nMore\nI can't make any real suggestions on ...|	0|
|	You, sir, are my hero. Any chance you remember...|	0|

## Сравниваем модели:

| Название |f1 |
|----------|---|		
|LogisticRegression|	0.768711|
|RandomForestClassifier|	0.379209|
|DecisionTreeClassifier	|0.603352|

## Выводы

На первом этапе произведена загрузка данных и их подготовка для обучения моделей. Для анализа данных и построения модели предоставлен датасет с размеченными данными, содержащий комментарии пользователей к товарам, доступным для приобретения в интернет-магазине «Викишоп». Датасет состоит из 2 столбцов с данными и 159292 строк.

Затем тексты комментариев были очищены и лемматизированы. 

В качестве моделей использованы LogisticRegression, RandomForestClassifier, DecisionTreeClassifier. 

По результатам подбора гиперпараметров и обучения моделей наилучший результат показал LogisticRegression, наихудший - RandomForestClassifier. 

Пороговое значение метрики 0.75 преодолено, получено 0.77. 

Лучшая модель - логистическая регрессия с подробранными гиперпараметрами C = 4, penalty = 'l1'.

Модель LogisticRegression подходит для решения поставленной задачи.   

