# Список проектов
Привет. Здесь вы можете ознакомиться с некоторыми моими DS и DA проектами.

## Kaggle

[HSE | 2nd Step In NLP | Salary prediction](https://www.kaggle.com/code/olgatretyakova/3rd-w2v-tf-idf-countvectorizer)  3|55

## Проекты Яндекс.Практикума

### ML и NLP проекты

| Проект | Цели и задачи | Описание работы |
| :-------------------- | :--------------------- | :--------------------- |
| [ML: Оптимизация производственного процесса легирования стали](https://github.com/TretyakovaOlga/Data-Science-Projects/blob/main/Steel%20alloying%20optimization/Prom_optimization_final_github.ipynb) | На базе исторических данных о процессах легирования сталей необходимо построить модель, которая будет прогнозировать температуру конечного расплава в зависимости от заданных параметров производственного процесса. Оптимизация достигается путем снижения энергозатрат за счёт предварительного подбора условий легирования. | Проведен исследовательский анализ данных, предобработка и объединение данные, созданы новые признаки. Рассмотрены два набора признаков для обучения. Рассмотрена линейная модель с регуляризацией, случайный лес, CatBoost и LGBM. Целевой признак изменяется в диапазоне от 1500 до 1704 градусов Цельсия. Используется метрика МАЕ, на финальной модели получен результат 5,68. Лучшая модель - Catboost. </br> Использованы библиотеки: sklearn, lightgbm, catboost |
| [NLP: Определение токсичности комментариев](https://github.com/TretyakovaOlga/Data-Science-Projects/blob/main/Toxic%20comments/Toxic_comments_predict.ipynb) | Необходимо построить модель для отсева токсичных комментариев. Метрика f1 - не менее 0.75. | Для создания словаря используется размеченный набор с комментариями. Лемматизация проводится с помощью nltk. Для получения признаков использованы мешок слов, TF-IDF, биграммы и word2vec.</br> Использованные модели: логистическая регрессия, LGBM, LinearSVC, метод ближайших соседей. Лучший результат получен на CountVectorizer + bigrams + LogisticRegression. На базе трёх лучших моделей составлен решающий ансамбль, проведено тестирование. Итоговое f1 - 0.77.</br> Использованы библиотеки: nltk, sklearn, gensim, lightgbm |
| [Исследование технологического процесса очистки золота](https://github.com/TretyakovaOlga/Data-Science-Projects/blob/main/Gold%20recovery/Gold_recovery_final.ipynb) | По данным с параметрами добычи и очистки нужно подготовить прототип модели машинного обучения для предсказания коэффициента восстановления золота из золотосодержащей руды. | Предоставленные данные имеют 87 признаков, включая целевой, разбиты на обучающую и тестовую выборки. Проведено исследование данных, составлена таблица признаков, обработаны пропуски и выборсы. Применен метод PCA для снижения размерности. Изучено несколько моделей - линейная регрессия, ElasticNet, Lasso, Ridge, метод ближайших соседей, метод опорных векторов, градиентный бустинг. Использована метрика SMAPE. </br> Использованы библиотеки: numpy, scipy, matplotlib, seaborn, sklearn |
| [ML: Определение рыночной стоимости автомобиля](http://github.com/TretyakovaOlga/Data-Science-Projects/blob/main/Predict%20of%20car%20prices/car_price_predict_final.ipynb) | Необходимо построить модель, которая будет предсказывать рыночную автомобиля в зависимости от его характеристик (сервис по размещению объявлений о продаже авто). | Модель разрабатывается на базе исторических данных о продажах автомобилей. Проведено исследование данных и предобработка: заполнение пропусков и удаление некорректных данных. Метрика RMSE. Рассмотрены линейные модели, метод ближайших соседей, CatBoost и LGBM, точность работы, скорость обучения и предсказания. </br> Использованы библиотеки sklearn, lightgbm, catboost |
| [ML Time Series: Прогнозирование заказов такси на следующий час](http://github.com/TretyakovaOlga/Data-Science-Projects/blob/main/Taxi%20orders%20predict/Taxi_predict.ipynb) | По историческим данным о заказах такси в аэропортах нужно построить модель прогнозирования количества заказов на следующий час для привлечения большего числа водителей в периоды пиковой нагрузки. | Были исследованы данные о заказах такси в аэропортах в перод с марта по август 2018 года. Были выделены признаки для прогнозирования временного ряда, в т.ч. тренд и сезонность. Проведено исследование и обучение моделей для прогнозирования - линейная регрессия, ElasticNet, Lasso, Ridge, метод ближайшх соседей. Изучена значимость признаков для каждой модели. Проведено финальной тестирование. Лучший результат показала Ridge регрессия с метрикой RMSE = 45,3. </br> Использованы библиотеки: numpy, scipy, statsmodels, matplotlib, seaborn, sklearn|
| [Определение наиболее прибыльного региона для нефтедобычи](http://github.com/TretyakovaOlga/Data-Science-Projects/blob/main/Lets%20find%20the%20well/Lets_find_the_well_final.ipynb) | На основании предсказаний модели машинного обучения и анализа финансовых показателей необходимо выбрать наиболее выгодный регион для развертывания нефтедобычи. | Нам предоставлены пробы нефти в трёх регионах. Были изучены данные по каждому региону; построены гистограммы. С помощью линейной регрессии получены предсказания о среднем объеме добычи в каждом из них. Проведен расчет прибыли, которую можно получить, если исследовать 500 случайных точек в регионе и выбрать 200 лучших. С помощью бутстрепа проведена оценка средней прибыли, 95% доверительного интервала и риска убытков. </br> Использованы библиотеки: numpy, scipy, matplotlib, seaborn, sklearn |
[Прогнозирование оттока клиентов банка](http://github.com/TretyakovaOlga/Data-Science-Projects/blob/main/Bank%20customer%20outflow/Bank_customer_outflow.ipynb) | По историческим данным о поведении клиентов и расторжении договоров с банком необходимо спрогнозировать, уйдёт клиент из банка в ближайшее время или нет. | Были изучены данные, проведена предобработка и заполнение пропусков. Изучены модели машинного обучения библиотеки sklearn: логистическая регрессия, дерево решений, случайный лес, метод ближайших соседей, метод опорных векторов, наивный Байес. Используемые метрики: F1 и ROC-AUC score. Рассмотрение проводилось с учетом дисбаланса классов. Лучшее решение дает случайный лес при использовании метода upsample.|

### DA проекты

| Проект | Цели и задачи | Описание работы |
| :-------------------- | :--------------------- | :--------------------- |
| [EDA: Исследование рынка недвижимости в Санкт-Петербурге 2014-2019 гг](http://github.com/TretyakovaOlga/Data-Science-Projects/blob/main/EDA%20Real%20Estate/EDA_Real_estate_final.ipynb) | На базе архива сервиса Яндекс.Недвижимость в Санкт-Петербурге и соседних населённых пунктах определить, от чего зависит рыночная стоимость квартир и выделить параметры типичной квартиры. | Изучены параметры квартир - площадь, цена, число комнат, высота потолков, этаж - и их влияние на цену. Создан портрет типичной квартиры. Рассмотрено время продажи квартиры и определены критерии слишком быстрых и слишком медленных продаж. Изучена стоимость квартир в различных населённых пунктах Ленинградской области. Выделен сегмент квартир в центре и проанализирована взаимосвязь цены и параметров квартир на этой территории. |
| [Игры: выявление закономерностей](http://github.com/TretyakovaOlga/Data-Science-Projects/blob/main/Games%20research/Smthng_about_games_final.ipynb) | Используя файл с историческими данными о продажах игр с 1980 по 2016 год, оценках пользователей и экспертов, жанрами и платформами, необходимо выявить закономерности, определяющие успешность игры  </br> | На примере наиболее успешных платформ изучен их типичный жизненный цикл. Рассмотрены актуальные растущие платформы, для них сформирован топ-10 игр. Рассмотрено, как влияют на продажи отзывы пользователей и критиков. Изучено общее распределение игр по жанрам и по жанрам внутри платформ. Составлен портрет пользователя по регионам: Северная Америка, Европа, Япония; для каждого региона определен топ-5 платформ и топ-5 жанров. Изучено влияние возрастного рейтинга ESRB на продажи в отдельном регионе. Проверены гипотезы о пользовательских рейтингах отдельных платформ и жарнов. |
| [Стат анализ: Анализ тарифов для оператора связи](http://github.com/TretyakovaOlga/Data-Science-Projects/blob/main/Telecom%20tariffs%20analysis/Telecom_tariffs_analysis.ipynb) | Необходимо проанализировать поведение пользователей и определить более прибыльный тариф. </br> | Проведен анализ поведения пользователей при пользовании услугами связи. Проверены гипотезы о различии средней выручки тарифов, а также о различии выручки в Москве и других регионах. |


