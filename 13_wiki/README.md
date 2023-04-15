# Проект для «Викишоп»

## Цель исследования
Обучить модель классифицировать комментарии на позитивные и негативные, чтобы отправлять токсичные комментарии на модерацию. 

## Ход исследования
- Подготовка данных. Загрузим данные для ознакомления. На данном этапе будет выполнен анализ данных;
- Обучение моделей. На данном этапе обучим разные модели с различными гиперпараметрами: LogisticRegression, DecisionTreeClassifier, CatBoostClassifier, SGDClassifier;
- Анализ модели. Проанализируем данные и делаем вывод о том, какая модель подходит лучше для выполнения задачи.

## Стек для работы
pandas, numpy, matplotlib.pyplot, yellowbrick.classifier, re, pymystem3, nltk, nltk.corpus, sklearn.feature_extraction.text, sklearn.model_selection,  sklearn.linear_model, sklearn.tree, sklearn.metrics, sklearn.utils, catboost, nltk, nltk.stem, nltk.tokenize, nltk.corpus, nltk.stem.porter, string, sklearn.pipeline, warnings 

## Выводы
Для оценки модели на тестовых данных мы исследовали наилучшую модель - LogisticRegression.

Полученный результат значения F1 = 0.765 удовлетворяет требованию технического задания. Данную модель можно использовать для классификации комментариев на позитивные и негативные, чтобы отправлять токсичные комментарии на модерацию. 

## Статус проекта
Завершен.