# Анализ бизнес-показателей

## Цель исследования:
Выяснить, почему средства, выделенные на привлечение пользователей приложения не окупаются.

## Ход исследования:
1. Загрузить данные и подготовить их к анализу.
2. Задать функции для расчета и анализа LTV, ROI, удержания и конверсии.
3. Провести исследовательский анализ данных, выделить профили пользователей и выяснить:

- Из каких стран приходят посетители? Какие страны дают больше всего платящих пользователей?
- Какими устройствами они пользуются? С каких устройств чаще всего заходят платящие пользователи?
- По каким рекламным каналам шло привлечение пользователей? Какие каналы приносят больше всего платящих пользователей?.

4. Провести маркетинговое исследование и выяснить:
- Сколько денег потратили? Всего / на каждый источник / по времени
- Сколько в среднем стоило привлечение одного покупателя из каждого источника?

5. Оценить окупаемость рекламы для привлечения пользователей с помощью LTV и ROI:
- Проанализировать общую окупаемость рекламы;
- Проанализировать окупаемость рекламы с разбивкой по устройствам;
- Проанализировать окупаемость рекламы с разбивкой по странам;
- Проанализировать окупаемость рекламы с разбивкой по рекламным каналам.

6. Выводы:
- Выделить причины неэффективности привлечения пользователей;
- Сформировать рекомендации для отдела маркетинга для повышения эффективности.

##  Описание данных:

Таблица visits_log_short (лог сервера с информацией о посещениях сайта):

    User Id — уникальный идентификатор пользователя
    Device — категория устройства пользователя
    Session start — дата и время начала сессии
    Session End — дата и время окончания сессии
    Channel — идентификатор рекламного источника, из которого пришел пользователь
    Region - страна пользователя

Таблица orders_log_short (информация о заказах):

    User Id — уникальный id пользователя, который сделал заказ
    Event Dt — дата и время покупки
    Revenue — выручка

Таблица costs_short (информация о затратах на маркетинг):

    Channel — идентификатор рекламного источника
    Dt — дата
    Costs — затраты на этот рекламный источник в этот день
    
## Использованные библиотеки
pandas, numpy, matplotlib, seaborn
