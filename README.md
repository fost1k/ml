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
$ git clone https://github.com/fost1k/ml.git
```
