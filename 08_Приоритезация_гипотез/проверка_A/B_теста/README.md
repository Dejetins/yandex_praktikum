# Принятие решений в бизнесе

## Задачи проекта
Используя данные интернет-магазина приоритезировать гипотезы, произвести оценку результатов A/B-тестирования различными методами.

## Используемые инструменты
- Python, Pandas, Matplotlib, SciPy, A/B-тестирование, проверка статистических гипотез

## Развитие навыков

- A/B-тест, статистический тест, фреймворк, RICE, ICE

## Описание проекта

В этом проекте я - аналитик крупного интернет-магазина. Вместе с отделом маркетинга мы подготовили список гипотез для увеличения выручки. 
Моя задача - приоритизировать гипотезы, запустить A/B-тест, проанализировать результаты и сделать выводы.

**Основная задача:**

- Принять решение по результатам теста и объяснить его. 
    Варианты решений:
    1. Остановить тест, зафиксировать победу одной из групп.
    2. Остановить тест, зафиксировать отсутствие различий между группами.
    3. Продолжить тест.

## Общий вывод

**Варианты принимаемых решений:**

- **Остановить тест, зафиксировать победу одной из групп.**
- <strike>Остановить тест, зафиксировать отсутствие различий между группами.
- Продолжить тест.</strike>

В итоге, после проведения A/B теста мы получили следующие результаты по кумулятивной метрике: по выручке, среднему чеку и среднему количеству заказов на пользователя, что практически на протяжении всего теста лидирует группа B. Сомнения появились из-за резких колебаний на графике кумулятивного среднего чека в группе B до очистки данных от аномальных пользователей, но после этого разница между средними чеками стала минимальной. По неочищенным данным различий в средних чеках в группах A и B не было, однако после очистки данных разница между средними чеками стала незначительной. 

До и после очистки данных, показатель среднего количества заказов в группе B превосходит показатель в группе A - сначала на 13.8%, а после очистки данных на 17.3%. Данная разница показателей среднего количества заказов между группами является статистически значимой, что позволяет нам сделать вывод о том, что мы можем **остановить наш A/B тест и зафиксировать победу группы B!** Более того, мы исключили возможность подглядывания в результаты и подтвердили корректность размера выборки данных.
