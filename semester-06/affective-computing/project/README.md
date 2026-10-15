# Проект · анализ эмоциональной окраски речи и текста

## Реализация

- [voice-emotions.ipynb](./voice-emotions.ipynb) — эксперимент с акустическими признаками и классификацией эмоций на датасете RAVDESS.
- [text-emotions.ipynb](./text-emotions.ipynb) — классификация эмоциональной окраски текстов на внешнем наборе Emotions Dataset for NLP.
- [main.py](./main.py) — прототип Telegram-бота с аудиопризнаками, моделью и PostgreSQL.

## Запуск

Ноутбуки запускаются в Jupyter/Kaggle после подключения датасетов и установки Python-библиотек. Для `main.py` требуются TensorFlow/Keras, librosa, python-telegram-bot и дополнительные библиотеки из импортов. Задайте `BOT_TOKEN` и `DB_DSN` через переменные окружения; модель и датасеты необходимо подготовить отдельно.

