[посмотреть проект](https://nbviewer.jupyter.org/github/IlyaMoshonkin/ds_projects/blob/master/select_oilwells/select_oilwells.ipynb)

## Выбор нефтяных скважин (ML in business)

### Данные 
- `id` — уникальный идентификатор скважины;
- `f0, f1, f2` — три признака точек;
- `product` — объём запасов в скважине (тыс. баррелей).

### Задача
Предоставлены данные о качестве нефти и объем ее запасов в трех регионах. Задача построить модель машинного обучения, которая поможет рассчитать прибыль в каждом из трех регионов. Проанализировать возможную прибыль и риски техникой Bootstrap. Выбрать регион с вероятностью убытка меньше 2.5% и наибольшей прибылью.

### Описание проекта
Проведен первичный анализ данных. Построена модель линейной регрессии для каждого региона. Сделано предсказание запаса сырья в каждом регионе. Техникой *Bootstrap* рассчитано распределение прибыли в регионах. Рассчитаны доверительный интервал и вероятность убытков. Выбран лучший регион для разработки скважин.

### Стек технологий
Pandas, Matplotlib, Seaborn, Sklearn
