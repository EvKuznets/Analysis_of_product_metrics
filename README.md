# Анализ продуктовых метрик 

# Стек:
<div>
  <img src="https://img.shields.io/badge/python-white?logo=python&style=for-the-badge" title="Python" alt="Python" height="40"/>&nbsp;
  <img src="https://img.shields.io/badge/pandas-white?logo=pandas&logoColor=blue&style=for-the-badge" title="Pandas" alt="Pandas" height="40"/>&nbsp;
  <img src="https://img.shields.io/badge/numpy-white?logo=numpy&logoColor=black&style=for-the-badge" title="Numpy" alt="Numpy" height="40"/>&nbsp;
  <img src="https://img.shields.io/badge/scipy-white?logo=scipy&logoColor=black&style=for-the-badge" title="Scipy" alt="Scipy" height="40"/>&nbsp;
  <img src="https://img.shields.io/badge/matplotlib-white?logo=matplotlib&logoColor=black&style=for-the-badge" title="Matplotlib" alt="Matplotlib" height="40"/>&nbsp;
  <img src="https://img.shields.io/badge/pingouin-white?logo=pingouin&logoColor=black&style=for-the-badge" title="Pingouin" alt="Pingouin" height="40"/>&nbsp;
</div>

## Описание:

Аналитический проект для стартапа-маркетплейса, специализирующегося на товарах из Бразилии. Цель — выявить точки роста выручки и конверсии через анализ пользовательского поведения, ассортимента и воронки продаж. Задачи: аудит данных, сегментация аудитории, тестирование гипотез, разработка дашбордов.

## Данные:

 olist_customers_dataset.csv — таблица с уникальными идентификаторами пользователей
| Название поля | Описание |
|:---------------|:----------------------------------|
| customer_id | позаказный идентификатор пользователя |
|customer_unique_id|  уникальный идентификатор пользователя (аналог номера паспорта) |
|customer_zip_code_prefix | почтовый индекс пользователя |
| customer_city | город доставки пользователя |
| customer_state | штат доставки пользователя |

olist_orders_dataset.csv —  таблица заказов
| Название поля | Описание |
|:---------------|:----------------------------------|
|order_id |  уникальный идентификатор заказа (номер чека) |
| customer_id | позаказный идентификатор пользователя |
| order_status | статус заказа |
| order_purchase_timestamp | время создания заказа |
| order_approved_at | время подтверждения оплаты заказа |
| order_delivered_carrier_date | время передачи заказа в логистическую службу |
| order_delivered_customer_date |  время доставки заказа |
| order_estimated_delivery_date | обещанная дата доставки |

olist_order_items_dataset.csv — товарные позиции, входящие в заказы
| Название поля | Описание |
|:---------------|:----------------------------------|
|order_id | уникальный идентификатор заказа (номер чека) |
| order_item_id | идентификатор товара внутри одного заказа |
| product_id | id товара (аналог штрихкода) |
| seller_id | id производителя товара| 
| shipping_limit_date | максимальная дата доставки продавцом для передачи заказа партнеру по логистике |
| price | цена за единицу товара |
| freight_value | вес товара |

## Результаты проекта:

1. Проведена предобработка данных.
2. Оценен месячный retention в оформление заказа с помощью когортного анализа.
3. Определены 5 основных метрик, на которых продакту можно сконцентрироваться, чтобы максимизировать прибыль компании.
4. Выбрана одна из 3 основных гипотез с помощью фреймворка ICE.
5. Сформулированы нужные метрики, на которые ваша гипотеза должна повлиять.
6. Сформулированы выводы о проделанной работе и составлен отчет.
