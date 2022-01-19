# ml

Итоговый проект курса "Машинное обучение в бизнесе"

Стек:

ML: sklearn, pandas, numpy
API: flask

Данные: с kaggle - https://www.kaggle.com/jsphyg/weather-dataset-rattle-package

Задача: cрогнозировать дождь на следующий день, целевая переменная "RainTomorrow". Бинарная классификация.

Используемые признаки:

- MinTemp (int)
- Rainfall (int)
- MaxTemp (int)

Преобразования признаков: StandardScaler

Модель: RandomForestClassifier

### Клонируем репозиторий и создаем образ
```
$ git clone https://https://github.com/fost1k/ml/edit/hw_9.git
$ cd hw_9
$ docker build -t fost1k/ml/edit/hw_9 .
```

### Запускаем контейнер

Здесь Вам нужно создать каталог локально и сохранить туда предобученную модель (<your_local_path_to_pretrained_models> нужно заменить на полный путь к этому каталогу)
```
$ docker run -d -p 8180:8180 -p 8181:8181 -v <your_local_path_to_pretrained_models>:/app/app/models fimochka/gb_docker_flask_example
```

### Переходим на localhost:8181
