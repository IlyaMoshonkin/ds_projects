## Репозиторий с проектами по Data Science


| Название проекта | Описание | Стек технологий | 
| :---------------------- | :---------------------- | :---------------------- |
| [Кредитный скоринг](credit_scoring) |Задача на основе предоставленных данных построить модель кредитного скоринга. Проведен первичный анализ данных. Добавли данные из внешних источников: данные курса доллара к рублю, как дополнительный фактор. Построили две модели: логистическую регрессию и бустинг над деревьями решений. Лучшей моделью выбрали бустинг. Сделали интерпретацию модели с помощью *Shap-value*. Провели тестирование и оценку модели. Итоговая метрика *ROC-AUC*: 0.95. Подобрали оптимальных порог исходя из наилучшей оценки кредита. |  Pandas, Matplotlib, Seaborn, Sklearn, LightGBM, Shap |
| [Отток клиентов банка](bank_churn) | Задача построить модель для предсказания оттока клиентов банка. Выполнена предобработка данных. Проведен первичный анализ данных. Преобразованы категориальные признаки методом *OneHotEncoding*. Сделано сравнение методов по работе с дисбалансом классов - *weight balanced, upsampling, downsampling*.  Результат: лучшая метрика достигнута после метода *upsampling*. Выбрана лучшая модель случайного леса. Проведена оптимизация гипперпараметров комбинацией методов случайного поиска и поиска по сетке. Посчитана метрика *ROC-AUC*: 0.85. Достигнута целевая метрика *F1*: 0.63. |  Pandas, Matplotlib, Seaborn, Sklearn |
| [Предсказание температуры стали](steel_temperature) | Задача построить модель предсказания температуры стали для оптимизации электропотребления. Выполнена предобработка данных. Заполнены пропуски и удалены аномальные значения. Проведена работа по слиянию нескольких датасетов и извлечению признаков из сырых данных. Построены несколько моделей – линейная регрессия, градиентный бустинг. Выбрана лучшая модель градиентного бустинга. Проведена интерпретация предсказаний модели с помощью *Shap-value*. Достигнута метрика *MAE* на тестовой выборке: 5.75. |  Pandas, Matplotlib, Seaborn, Sklearn, LightGBM, CatBoost, Eli5, Shap |
| [Определение возраста человека (CV)](face_age_define) | Задача построить модель определения возраста человека с помощью компьютерного зрения. Проведен анализ распределения возраста в тренировочной выборке. Проведена работа по аугментации данных: *horizontal_flip, rotation_range*. Построена модель *ResNet-50* методом *transfer learning*. Достигнута целевая метрика *MAE*: 7.46  |  Pandas, Numpy, Matplotlib, Tensorflow, Keras |
| [Предсказание количества заказов такси (TS)](taxi_timeseries) | Задача построить модель предсказания количества заказов такси используя исторические данные. Проведен первичный анализ данных. Найден тренд и сезонность временного ряда. Из временного рядя извлечены признаки. Сделано сравнение моделей: линейная регрессия, LightGBM, Prophet. Лучшая метрика достигнута моделью LigthGBM после тюнинга с помощью *RandomizedSearchCV*. Достигнута целевая метрика *RMSE*: 47.8  |  Pandas, Plotly, Eli5, Sklearn, LightGBM, Prophet |
| [Классификация комментариев (NLP)](toxic_comments) | Задача обучить модель классифицировать комментарии. Нам доступен датасет с размеченными позитивными и негативными комментариями. Целевая метрика качества: *F1* не меньше 0.75. Данные с комментариями предобработаны: очистка текста с помощью регулярных выражения, применена техника стеминга английских текстов. Данные обработаны методом *TF-IDF*, обучена логистическая регрессия, такой пайплайн позволяет получить хороший результат c метрикой качества *F1* более 0.75.  Получилось улучшить результат с помощью предобученной модели *Bert*. Достигнута целевая метрика *F1*: 0.83.  |  Pandas, NLTK, Sklearn, PyTorch, Bert |
| [Выбор нефтяных скважин (ML in business)](select_oilwells) | Предоставлены данные о качестве нефти и объем ее запасов в трех регионах. Задача построить модель машинного обучения, которая поможет рассчитать прибыль в каждом из трех регионов. Проведен первичный анализ данных. Построена модель линейной регрессии для каждого региона. Сделано предсказание запаса сырья в каждом регионе. Техникой *Bootstrap* рассчитано распределение прибыли в регионах. Рассчитаны доверительный интервал и вероятность убытков. Выбран лучший регион для разработки скважин. |  Pandas, Matplotlib, Seaborn, Sklearn |
| [Оптимизация золотодобычи](goldmining_optimization) | Предоставлены данные об добыче и очистке руды. Задача построить модель для предсказания коэффициента восстановления золота из золотосодержащей руды. Проведена подготовка данных. Исследованы концентрации веществ на разных стадиях очистки руды. Данные очищены от аномальных значений. Построили различные модели, сделали оптимизацию гипперпараметров. Выбрали лучшие модели для предсказания эффективности обогащения чернового и финального концентратов. Провели отбор признаков, тем самым улучшили качество модели. Лучшая модель случайного леса протестирована, сделано сравнение с константной моделью. Достигнута целевая метрика *sMAPE*: 6.4. |  Pandas, Matplotlib, Seaborn, Sklearn |

