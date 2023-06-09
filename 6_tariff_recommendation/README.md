# Рекомендация тарифов

## Цель исследования
Построить модель для задачи классификации, которая выберет подходящий тариф.

## Ход исследования
1. Обзор данных. На этом этапе будет проведены обзор, оценка качества данных, оценка возможности использовать данные для машинного обучения. Убедимся в отсутствии необходимости предобработки данных;
2. Разделение исходные данные на обучающую, валидационную и тестовую выборки. На этом этапе будет проведено разделение данных на соответствующие выборки и проверка данных выборок на однородность;
3. Исследование качества моделей. На данном этапе будет предложен ряд алгоритмов машинного обучения, с использованием которых будет проведено обучение моделей, путем подбора гиперпараметров будет осуществляться поиск наиболее точных моделей;
4. Проверка качества модели на тестовой выборке. На этом этапе мы проверим модель, показавшую более точный результат;
5. Проверим модель на вменяемость.

## Стек для работы
pandas, numpy, seaborn, sklearn.model_selection, catboost, sklearn.dummy, sklearn.tree, sklearn.linear_model, sklearn.ensemble, sklearn.metrics, catboost, sweetviz, yellowbrick.classifier, tqdm, matplotlib.pyplot, warnings

## Выводы
- Данный анализ позволил установить, что все модели, кроме LogisticRegression показали хороший результат, относительно порогового значения (0,75). Самый высокий показатель точности достигла модель CatBoost;
- Проверка качества лучшей модели CatBoost на тестовой выборке требовала разделения тестовой выборки на целевой атрибут и атрибуты со свойствами для построение моделей. В результате проверки модель показала высокую точность и подтвердила правильность выбора модели для обучения;
- Полученные результаты свидетельствуют о том, что для задачи классификации, которая требует выбора подходящего тарифа можно использовать модель CatBoost, которая показала высокий уровень точности;
- Исследование модели на вменяемость(адекватность)проводилось с помощью DummyClassifier.  Мы получили максимальное значение 0.707 и значения, полученные с использованием DummyClassifier, не достигли порогового значения(0,75). Точность модели CatBoost оказалась значительно выше - 0.811. Эти данные свидетельствуют о вменяемости(адекватности) модели CatBoost.

## Статус проекта
Завершен.