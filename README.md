# Тестовое Mindbox на позицию "Junior Data Engineer / MLOps"

### Задание №1.

Есть Pandas DataFrame со столбцами [“customer_id”, “product_id”, “timestamp”] , который содержит данные по просмотрам товаров на сайте. Есть проблема – просмотры одного customer_id не разбиты на сессии (появления на сайте). Мы хотим разместить сессии так, чтобы сессией считались все смежные просмотры, между которыми не более 3 минут.

Написать методом который создаст в Pandas DataFrame столбец session_id и проставит в нем уникальный int id для каждой сессии.

У каждого пользователя может быть по несколько сессий. Исходный DataFrame может быть большим – до 100 млн строк.


### Задание №2.

В SQL базе данных есть продукты и категории. Одному продукту может соответствовать много категорий, в одной категории может быть много продуктов.

Напишите HTTP API через которое можно получить:

список всех продуктов с их категориями,
список категорий с продуктами,
список всех пар «Имя продукта – Имя категории».

Если у продукта нет категорий, то он все равно должен выводиться. Если у категории нет продуктов, то она все равно должна выводиться.

Проект должен содержать docker-compose.yml файл, через который можно запустить сервис и проверить его работу.

---

**P.S. С докером никогда до этого не сталкивался, пока крутил и разбирался, вакансию закрыли. Но тестовые сделал. При поднятии контейнера `docker-compose build` && `docker-compose up`, открывается локальный сервер, но апишки не пробиваются. Причину пока не обнаружил.**
