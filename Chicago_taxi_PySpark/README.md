# Определение количества заказов такси по районам в Чикаго

1) Агрегатор такси в Чикаго хочет прогнозировать количество заказов в каждом районе. Это необходимо, чтобы в моменты пиковой нагрузки привлекать больше водителей, а во время спада оотправлять их в другие места. Необходимо построить модель, которая сможет предсказать количество заказов.

Для обучения модели машинного обучения предоставлены данные о 10 млн заказов такси за 2022 и 2023 год. Информацию собирает регулирующий орган. Из соображений конфиденциальности, идентификатор такси соответствует заданному номеру медальона такси, переписные участки в некоторых случаях скрыты, а время округляется до ближайших 15 минут.

Метриками качества приняты МАЕ и MAPE.

По условиям проекта, необходимо развернуть локальные контейнеры через Docker и произвести большую часть работ в PySpark.

2) Для проекта с помощью Docker был развернут локальный кластер с 4 рабочими контейнерами. Из-за нестабильной работы Docker и ограниченных вычислительных ресурсов, работу разбили на три блокнота по стадиям. 

3) **Этапы проекта**

    - EDA
    - Агрегация данных, выделение целевого показателя
    - Создание дополнительных признаков
    - Выбор и подготовка модели
    - Обучение модели, проверка на валидационных данных, прогноз целевых показателей
    
4) **Итог:**
- Для предсказания  количества заказов предложена модель

    **LinearRegression**
- МАЕ: 1.5161329898172002
- МАРЕ: 39.00934602125235

### Навыки и инструменты
------------------
    * Python
    * PySpark
    * Seaborn
    * FB Prophet
------------------    
