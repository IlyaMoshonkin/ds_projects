[посмотреть проект](https://nbviewer.jupyter.org/github/IlyaMoshonkin/ds_projects/blob/master/taxi_timeseries/taxi_timeseries.ipynb)

## Предсказание количества заказов такси (TS)

### Данные 
`datetime` - дата и время заказа  
`num_orders` - количество заказов

### Задача
Построить модель предсказания количества заказов такси используя исторические данные. 

### Описание проекта
Проведен первичный анализ данных. Найден тренд и сезонность временного ряда. Из временного рядя извлечены признаки. Сделано сравнение моделей: линейная регрессия, LightGBM, Prophet. Лучшая метрика достигнута моделью LigthGBM после тюнинга с помощью *RandomizedSearchCV*. Достигнута целевая метрика *RMSE*: 47.8.

### Стек технологий
Pandas, Plotly, Eli5, Sklearn, LightGBM, Prophet

