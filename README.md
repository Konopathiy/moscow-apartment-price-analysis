# Анализ цен на квартиры в Москве

Учебный проект Data Science
Цель — понять, какие характеристики квартиры связаны с ценой, и построить простую модель предсказания цены.

## Вопрос проекта

**Какие факторы сильнее всего влияют на цену квартиры в Москве и насколько точно можно предсказать цену по её характеристикам?**

## Данные

Используется публичный датасет Kaggle: [Prices of Moscow apartments](https://www.kaggle.com/datasets/ivan314sh/prices-of-moscow-apartments).

Скачай файл `moscow_flats_dataset_eng.csv` и положи его в папку `data/`.

## Что сделано

- Загрузка и первичный осмотр данных
- Проверка пропусков, дубликатов и типов данных
- Обработка выбросов по цене и площади
- Создание признака «цена за квадратный метр»
- Разведочный анализ данных (EDA)
- Визуализация распределения цен и связей между признаками
- Обучение моделей Linear Regression и Random Forest
- Оценка качества моделей: MAE, RMSE, R²
- Сравнение с baseline-моделью, которая всегда предсказывает медианную цену

## Как запустить

1. Установи Python 3.10+.
2. Создай виртуальное окружение:

```bash
python -m venv .venv
```

3. Активируй окружение:

Windows:

```bash
.venv\Scripts\activate
```

macOS / Linux:

```bash
source .venv/bin/activate
```

4. Установи библиотеки:

```bash
pip install -r requirements.txt
```

5. Положи датасет в `data/moscow_flats_dataset_eng.csv`.
6. Запусти Jupyter Notebook:

```bash
jupyter notebook
```

7. Открой `notebooks/analysis.ipynb` и запусти все ячейки: `Run All`.

## Структура проекта

```text
moscow-apartment-price-analysis/
├── README.md
├── requirements.txt
├── .gitignore
├── data/
│   └── moscow_flats_dataset_eng.csv
├── notebooks/
│   └── analysis.ipynb
└── figures/
```

## Что можно улучшить

- Добавить район, расстояние до метро, этаж и год постройки.
- Проверить несколько моделей и подобрать гиперпараметры.
- Сделать интерактивный дашборд в Streamlit.
