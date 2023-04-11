# yandex_practicum

Данные проекты были выполнены в ходе обучения в Яндекс.Практикуме, профессии "Аналитик данных" / "Специалист по Data Science".

[![Typing SVG](https://readme-typing-svg.herokuapp.com?color=%2336BCF7&lines=The+projects+are+complete!)](https://git.io/typing-svg)

| Наименование  | Цель проекта     | Библиотеки    | Выводы       |
| ------------- | ------------- | ------------- | ------------- |
| [1. Яндекс Музыка](./1_yandex_music/1_yandex_music.ipynb) | Проверка трех гипотез: <ul><li>Активность пользователей зависит от дня недели. Причём в Москве и Петербурге это проявляется по-разному.</li><li>В понедельник утром в Москве преобладают одни жанры, а в Петербурге — другие. Так же и вечером пятницы преобладают разные жанры — в зависимости от города.</li><li>Москва и Петербург предпочитают разные жанры музыки. В Москве чаще слушают поп-музыку, в Петербурге — русский рэп.</li></ul> | pandas | Мы проверили три гипотезы и установили: <ul><li>Первая гипотеза полностью подтвердилась.</li><li>Вторая гипотеза подтвердилась лишь отчасти - этот результат мог оказаться иным, если бы не пропуски в данных.</li><li>Третья гипотеза не подтвердилась. Если различия в предпочтениях и существуют, на основной массе пользователей они незаметны.</ul></li>|
| [2. Исследование надёжности заёмщиков](./2_borrower_reliability/2_borrower_reliability.ipynb) |Выяснить влияет ли семейное положение и количество детей клиента на факт погашения кредита в срок. |pandas|На возврат кредита в срок влияют следующие данные о клиентах банка:<ul><li>Количеством детей.C увеличением количества детей мы видим увеличение количества просроченных задолженностей. Бездетные клиенты банка реже опаздывают с внесением оплаты по кредиту, чем люди с детьми; </li><li>Семейное положение. Клиенты банка не состоящие в браке и клиенты, состоящие в гражданском браке,чаще опаздывают с внесением оплаты по кредиту (или не платят по кредиту).Овдовевшие клиенты банка и клиенты, состоящие в разводе, чаще вовремя вносят оплату по кредиту;</li><li> Цели кредита.Клиенты банка, взявшие кредит на операции с автомобилем и получение образования, чаще опаздывают с внесением оплаты по кредиту (или не платят по кредиту). Чаще всего клиенты банка платят в срок по кредиту взятого на операции с недвижимостью и проведение свадьбы. На возврат кредита в срок не влияет уровнень дохода клиентов банка.</ul></li>|
|[3. Исследование объявлений о продаже квартир](./3_apartment_sales_research/3_apartment_sales_research.ipynb) | Определить факторы, которые влияют на формирование стоимости жилья.| pandas, matplotlib, seaborn|Определены показатели, которые больше всего на стоимость объектов недвижимости:<ul><li> стоимость квадратного метра, на которую влияет удаленость от центра города;</li><li>общая площадь , т.к. видна линейная зависимость: с ростом общей площади увеличивается и стоимость квартиры. Жилая площадь, влияет на стоимость, так как напрямую зависит от общей площади; </li><li> cтоимость квартир напрямую зависит от числа комнат: чем их больше, тем квартира дороже. Но это верно, пока число комнат не превышает 4, далее видим спад стоимости жилья. Возможная причина - отсутствием спроса; </li><li>квартиры на первом или последнем этаже продаются по более низкой цене, чем квартиры на других этажах; </li><li> день недели и месяц публикации объявления не играют значимой роли на стоимость, по которой объект недвижимости будет продан; </li><li> квартиры продавались по более высоким ценам в 2014 году - с точки зрения экономической ситуации. Начиная с 2018г. наблюдается постепенный рост стоимости жилья.</ul></li>|
|[4. Анализ тарифов сотовых операторов](./4_analysis_of_tariffs_of_mobile_operators/4_analysis_of_tariffs_of_mobile_operators.ipynb)|Проанализировать поведение клиентов и сделать вывод — какой тариф лучше: «Смарт» или «Ультра».|pandas, numpy, seaborn, matplotlib, scipy| </li><li>Средняя длительность разговоров у абонентов тарифа Ultra больше, чем у абонентов тарифа Smart. В течение года пользователи обоих тарифов увеличивают среднюю продолжительность своих разговоров. Рост средней длительности разговоров у абонентов тарифа Smart равномерный в течение года. Пользователи тарифа Ultra не проявляют подобной линейной стабильности. Стоит отметить, что феврале у абонентов обоих тарифных планов наблюдались самые низкие показатели. </li><li>В среднем количество сообщений пользователи тарифа Ultra отправляют больше - почти на 20 сообщений больше, чем пользователи тарифа Smart. Количество сообщений в течение года на обоих тарифак растет. Динамика по отправке сообщений схожа с тенденциями по длительности разговоров: в феврале отмечено наименьшее количество сообщений за год и пользователи тарифа Ultra также проявляют нелинейную полодительную динамику. </li><li>Меньше всего пользователи использовали интернет в январе, феврале и апреле. Чаще всего абоненты тарифа Smart тратят 15-17 Гб, а абоненты тарифного плана Ultra - 19-21 ГБ. </li><li>Отвергли гипотезу о том, что выручка пользователей  "Ультра" равна выручке пользователей "Смарт". </li><li>Не получилось отвергнуть гипотезу о том, что выручка пользователей из Москвы равна выручке пользователей не из Москвы.</ul></li>|
|[5. Исследование рынка производителей видеоигр](./5_research_on_video_game/5_research_on_video_game.ipynb) |</li><li>На основании закономерностей, определяющих успешность видеоигры, выявить потенциально популярный продукт для размещения в интернет-магазине «Стримчик».</li><li> На основании анализа целевой аудитории и ее предпочтений, спланировать рекламные кампании на 2017-й год для каждого региона.</ul></li>|pandas, matplotlib, scipy, seaborn |Составление портрета пользователя для каждого региона(NA, EU, JP) показало следующие наборы характеристик:</li><li>для пользователей региона - Северная-Америка, интересны игры на платформ ps4 и xone, жанров action и shooter, с рейтингом игры M (старше 17 лет);</li><li>для пользователей региона - Европа, интересны игры на платформе ps4, жанра action, с рейтингом игры M (старше 17 лет);</li><li>для пользователей региона - Япония, интересны игры на платформе 3ds, жанра role-playing, с рейтингом игры: - в регионе - Япония - лидирует по прадажам игры в категории:Т и Е(для всех и для всех от 10 лет и старше).</li><li>Регион Японии выделяется среди прочих значительно, при желании развития платфомы в данном регионе следует обратить особое внимание на культурные особенности данного региона. В данном исследовании отсутствовала значительная часть данных в части рейтинга игр и требуется проведение дополнительного анализа при наличии данных с меньшим колличеством пропущенных значений.</ul></li>|
|[6. Рекомендация тарифов](./6_tariff_recommendation/6_tariff_recommendation.ipynb)|Построить модель для задачи классификации, которая выберет подходящий тариф. |pandas, numpy, sklearn, sweetviz, pandas_profiling, seaborn, matplotlib, yellowbrick classifier|Для задачи классификации, которая требует выбора подходящего тарифа можно использовать модель CatBoost, которая показала высокий уровень точности - 0.811. Модель прошла проверку на вменяемость(адекватность).|
|[7. Отток клиентов](./7_customer_churn/7_customer_churn.ipynb)|Построить модель для задачи классификации, которая спрогнозирeт, уйдёт клиент из банка в ближайшее время или нет. |pandas, numpy, yellowbrick classifier, pandas_profiling, matplotlib, sklearn, imblearn undersempling, phik report, catboost|По итогам тестирования модель  CatBoostClassifier показала удовлетворительный результат: F1 = 0.6. Значение AUC-ROC = 0.77 показала нам, что площадь под кривой намного выше площади дефолтной модели. Обученная нами модель прошла проверку на адекватность. Данная модель может быть использована для задачи классификации, которая спрогнозирeт, уйдёт клиент из банка в ближайшее время или нет.|
|[8. Восстановление золота из руды](./8_recovery_of_gold/8_recovery_of_gold.ipynb)|Подготовить прототип модели машинного обучения для компании, которая разрабатывает решения для эффективной работы промышленных предприятий. |pandas, numpy, yellowbrick, pandas_profiling, matplotlib, sklearn, seaborn |Лучший результат показала модель Lasso(random_state=42, lasso__alpha = 0.5). На тренировочной выборке было получено the_total_sMAPE = -7.879; на тестовой выборке the_total_sMAPE = 6.357. Значение метрики получилась ниже, чем на константной модели the_total_sMAPE = 7.473. Делаем вывод о том, что данную модель можно использовать для  оптимизировать производства.|
|[9. Выбор локации для скважины](./9_choosing_a_location_for_the_well/9_choosing_a_location_for_the_well.ipynb)|Построить модель машинного обучения, которая поможет определить регион, где добыча принесёт наибольшую прибыль.|pandas, numpy, sklearn, matplotlib, seaborn|В результате проделанной работы была построена модель машинного обучения LinearRegression, которая помогла определить регион, где добыча принесёт наибольшую прибыль. Таким регионом на основании расчетов выбран регион 2.|
|[10. Защита персональных данных клиентов](./10_data_privacy/10_data_privacy.ipynb) |Предложить алгоритм преобразования для защиты данные клиентов страховой компании «Хоть потоп». Который не позволит восстановить персональную информацию клиентов.|pandas, numpy, sklearn, yellowbrick classifier, pandas_profiling, matplotlib, seaborn|Был сформулирован алгоритм преобразования исходной матрицы признаков:</li><li> Генерация матрицы обратимой матрицы.</li><li> Вычисление определителя (детерминанта) обратимой матрицы.</li><li> Создание закодированной матрицы признаков.</li><li> Нахождение метрик: модели, обученнойна исходных признаках, и модели, обученнойна на закодированных признаках.</li><li> Сравнение метрик между собой.<ul><li>В результате проверки алгоритма преобразования нами были получены одинаковые значения R^2( до 13 знака после запятой) как для модели обученной на исходных наборах данных, так и на закодированных.На основании полученных данных, был сделан вывод о том, что алгоритм работает и подтверждает алгебраический вывод в отношении неизменности предсказаний в отношении закодированной матрицы признаков по отношению к исходной. Алгоритм кодирования предполагает умножение исходной матрицы признаков на произвольно сгенерированную обратимую матрицу признаков.</ul></li>|
|[11. Определение стоимости автомобилей](./11_vehicle_valuation/11_vehicle_valuation.ipynb)| Построить модель для определения стоимости автомобилей с пробегом. Модель должна показывать высокое качество предсказания, высокую скорость предсказания и малое количество времени обученя.|pandas, numpy, matplotlib, seaborn, catboost, lightgbm| Дольше всех обучается модель catboost: 8 min 31 s. Дольше всех предсказывает модель LightGBM 3,07 s. Значение rmse мы получили самые высокие для этих моделей. Быстрее всех обучается и предсказывает модель Дерева принятия решений, но значение rmse достаточно низкое.Больше всего соответствует требованиям заказчика модель catboost, которая обладает  высоким качеством предсказания (на тесте 1737.33), так является и одной из самых быстрых по скорости предсказания, но у модели  catboost самая малелькая скоростью обучения. Заказчик может обратить внимание и на модель LightGBM, которая чуть хуже предсказывает и дольше предсказывает, но достаточно быстро обучается.|
|[12. Прогнозирование заказов такси](./12_cab_order_forecasting/12_cab_order_forecasting.ipynb)| Построить модель предсказания, которая спрогнозирует количество заказов такси на следующий час, чтобы привлекать больше водителей в период пиковой нагрузки.|pandas, numpy, yellowbrick, pandas_profiling, matplotlib, sklearn, seaborn|Модель SARIMA может быть использована для прогнозирования количества заказов такси на следующий час, чтобы привлекать больше водителей в период пиковой нагрузки.|
|[13. Проект для «Викишоп»](./13_wiki/13_wiki.ipynb)|Обучить модель классифицировать комментарии на позитивные и негативные, чтобы отправлять токсичные комментарии на модерацию.|matplotlib, numpy, pandas, re, pymystem3, nltk, sklearn, catboost, yellowbrick | Лучший результат показала модель LogisticRegression. На тестовых данных получено значения F1 = 0.765, которое удовлетворяет требованию технического задания. Данную модель можно использовать для классификации комментариев на позитивные и негативные, чтобы отправлять токсичные комментарии на модерацию.| 
|[14. Базовый SQL](./14_sql/14_sql.ipynb)|Проанализировать данные о фондах и инвестициях и написать запросы к базе. | SQL| В результате выполнения работы отработаны следующие навыки:</li><li>писать SQL-запросы разной сложности;</li><li>получать срезы данных и составлять подзапросы;</li><li>применять агрегирующие и оконные функции;</li><li>объединять таблицы разными методами.|
|[15. Определение возраста покупателей](./15_determining_customer_age/15_determining_customer_age.ipynb)|Построить модель, которая по фотографии определит приблизительный возраст человека.  | pandas, tensorflow, matplotlib| В результате обучени модели нам удалось достигнуть поставленной цели: по фотографии определять приблизительный возраст человека. Получено значение метрики MAE - 6.1233 на тестовой выборке, что удовлетворяет условию поставленной задачи.|
|[16. Телеком](./16_telecom/16_telecom.ipynb)|Определить факторы, которые влияют на лояльность клиентов. Обучить модель машинного обучения, способную предсказать отток клиентов.| pandas, numpy, yellowbrick, pandas_profiling, matplotlib, seaborn, lightgbm, phik, sklearn, catboost, functools| Лучший результат показала модель CatBoost. </li><li>Параметры модели: random_state=270323, auto_class_weights='Balanced', depth = 6 , iterations = 250, learning_rate = 0.1, loss_function = 'Logloss'.</li><li>Качество модели: roc_auc - 0.909339; accuracy - 0.839296; precision - 0.919665; recall - 0.854588; quality - 0.894686.</li><li> Выбранная модель справляется с поставленой задачей: способна предсказать отток клиентов или лояльность клиентов.|