# tariffs_recomendation
Рекомендация тарифов

## Описание проекта

По данным оператора мобильной связи многие клиенты пользуются архивными тарифами. Компания планирует построить систему, способную проанализировать поведение клиентов и предложить пользователям новый тариф: «Смарт» или «Ультра».
Иммется информация о поведении клиентов, которые уже перешли на эти тарифы (из проекта <a href = "https://github.com/Timur-Chu/Mobile_tariffs_analysis">"Определение перспективного тарифа для телеком компании"</a>).

Необходимо построить модель для задачи классификации, которая выберет подходящий тариф с максимально большим значением accuracy. Долю  правильных ответов нужно довести    до 0.75. и проверьте accuracy на тестовой выборке.

##Описание данных

Каждый объект в наборе данных — это информация о поведении одного пользователя за месяц. Известно:
сalls — количество звонков,
minutes — суммарная длительность звонков в минутах,
messages — количество sms-сообщений,
mb_used — израсходованный интернет-трафик в Мб,
is_ultra — каким тарифом пользовался в течение месяца («Ультра» — 1, «Смарт» — 0).

## Вывод

Наиболее адекватные предсказания делает Random Forest, это видно по точности предсказания на валидационной и на тестовой выборке.

Значения метрики accuracy:

Logistic Regression: 0.70

Random Forest: 0.81

Decision Tree: 0.80
