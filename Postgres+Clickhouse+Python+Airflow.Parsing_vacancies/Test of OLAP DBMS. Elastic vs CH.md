## Концепция 
В проекте будет использовано 2 СУБД: транзакционная (Postgres) и аналитическая.
В качестве аналитической СУБД рассматриваются 2 варианта: Elastic И ClickHouse. 

Концептуальная схема по работе с данными
![image](https://github.com/Nastya224/Elastic1/assets/94219446/c1f10422-32fc-4c9c-b051-fd16497e1c4b)

## Описание теста
Проведено тестирование скорости вывода данных из аналитической БД. 
Сравниваются 2 вариантов: 
* 1 вариант) транзакционная Postgres + аналитическая Clickhouse (синхронизация через движки Clickhouse: PostgreSQL и MaterializedPostgreSQL). Ссылка на файлы по Clickhouse: https://github.com/Nastya224/1_T_Data_Data_engineer/tree/0f8285729f20d0d52266c0d11f1c40360d92c6f9/Postgres%2BElastic%2Bpgsync%2BPython%2BAirflow.%20Parsing_vacancies
* 2 вариант) транзакционная Postgres + аналитическая Elastic (синхронизация через сервис Pgsync)

## Результаты

По результатам выбрана СУБД Elastic

![image](https://github.com/Nastya224/Elastic1/assets/94219446/aef62d25-4160-43ca-a56a-fd9a3decc23d)
