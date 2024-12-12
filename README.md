
### Гибридная система рекомендаций книг

Данный репозиторий содержит реализацию **гибридной системы рекомендаций книг**, которая сочетает методы коллаборативной фильтрации и контентной фильтрации для создания точных и персонализированных рекомендаций.

## Возможности

- **Коллаборативная фильтрация**:
  Использует взаимодействия пользователей с книгами для нахождения похожих заголовков.
- **Контентная фильтрация**:
  Улучшает рекомендации коллаборативной модели, анализируя метаданные, такие как:
  - Категории книг
  - Авторы
  - Оценки тональности отзывов
- **Гибридный подход**:
  Объединяет оба метода для преодоления таких проблем, как отсутствие данных о новых книгах и недостаток информации о пользователях.

## Основные компоненты

- **Обучение моделей**:
  Использование PyTorch для реализации моделей коллаборативной и контентной фильтрации.
- **Методы рекомендаций**:
  - `get_collaborative_recommendations`: Генерация рекомендаций на основе коллаборативной фильтрации.
  - `get_content_based_recommendations`: Уточнение и сортировка рекомендаций с использованием контентной информации.
- **Предобработка данных**:
  Скрипты для обработки данных о книгах, извлечения метаданных и анализа тональности отзывов.
- **Оценка качества**:
  Тестирование гибридной системы и сравнение с результатами отдельных методов.

## Обущающая выборка

https://www.kaggle.com/datasets/mohamedbakhet/amazon-books-reviews/code?datasetId=2476732&sortBy=voteCount

## Установка

1. Склонируйте репозиторий:
   ```bash
   git clone https://github.com/yourusername/hybrid-book-recommendation.git
   ```
2. Перейдите в директорию:
   ```bash
   cd hybrid-book-recommendation
   ```
3. Установите зависимости:
   ```bash
   pip install -r requirements.txt
   ```

## Использование

1. Подготовьте датасет, соответствующий формату данных (https://www.kaggle.com/datasets/mohamedbakhet/amazon-books-reviews/code?datasetId=2476732&sortBy=voteCount).
2. Обучите или загрузите предобученные модели из репозитория.

## Пример вывода

Для книги *"The Universe and Dr. Einstein"* система предоставляет ранжированный список рекомендованных книг.

## Детали Jupyter Notebook

Файл `Book_recommendation_model.ipynb` содержит:
- Код для обучения и оценки моделей.
- Скрипты для генерации рекомендаций.
- Интерактивные виджеты для исследования результатов.

