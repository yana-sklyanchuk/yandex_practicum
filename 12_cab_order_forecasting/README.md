# Прогнозирование заказов такси

## Ход исследования
1. Подготовка данных. Загрузим данные и выполнить их ресемплирование по одному часу для ознакомления с данными;
2. Анализ данных. На данном этапе будет выполнен анализ данных;
3. Обучение моделей. На данном этапе мы cделать тестовую выборку размером 10% от исходных данных и обучим разные модели с различными гиперпараметрами: LinearRegression, DecisionTreeRegressor, RandomForestRegressor, CatBoostRegressor, SARIMA;
4. Анализ моделей. Проанализируем данные и делаем вывод о том, какая модель подходит лучше всего.

## Стек для работы
pandas, numpy, seaborn, matplotlib, time, datetime, os, math, yellowbrick.classifier, pandas_profiling, pandas.api.types, statsmodels.tsa.seasonal, sklearn.linear_model, sklearn.tree import, sklearn.ensemble, sklearn.preprocessing, sklearn.pipeline, sklearn.metrics, sklearn.model_selection, xgboost.sklearn, lightgbm, catboost, pmdarima.arima, statsmodels.tsa.statespace

## Выводы
Худшее значение RMSE было получено на тренировочных данных при обучении модели LinearRegression - 32.790.

Лучшее значение RMSE было получено на тренировочных данных при обучении модели SARIMA - 17.690.

На тестовых данных RMSE было получено при обучении модели SARIMA - 28.460. Данный результат удовлетворяет условию: значение метрики RMSE на тестовой выборке должно быть не больше 48. 

Модель SARIMA может быть использована для прогнозирования количества заказов такси на следующий час, чтобы привлекать больше водителей в период пиковой нагрузки.

## Статус проекта
Завершен.
