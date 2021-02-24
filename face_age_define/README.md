[посмотреть проект](https://nbviewer.jupyter.org/github/IlyaMoshonkin/ds_projects/blob/master/face_age_define/face_age_define.ipynb)

### Данные 
- file_name — имя файла с изображением объекта
- real_age — фактический возраст объекта


### Задача
Построить модель определения возраста человека с помощью компьтерного зрения.

### Описание проекта
Проведен анализ распределения возраста в тренировачной выборке. Проведена работа по аугментации данных: *horizontal_flip, rotation_range*. Построена модель *ResNet-50* методом *transfer learning*. Достигнута целевая метрика *MAE*: 7.46

### Стек технологий
Pandas, Numpy, Matplotlib, Tensorflow, Keras 

