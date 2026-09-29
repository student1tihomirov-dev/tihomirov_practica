Ответы на задачи Web3–Web12

Web3
Метод: GET
Статус: 304
Type: document
Количество пользователей: 10
Запрос со статусом не 200: нет

Web4
Вернулось комментариев: 5

Web5
Вернулось 3 обьекта 
 "albumId": 1,
        "id": 1,
        albumId": 1,
        "id": 2,
         "albumId": 1,
        "id": 3,

Web6
Количество ответов для postId=3:5
Количество ответов для postId=4:5
это погинация показывает на какой странице находиться user

Web7
Гипотеза: Думаю, что параметр _limit задает ограничение возвращаемых объектов в ответе.
Что потверждает ввод ссылки 
https://jsonplaceholder.typicode.com/posts?_limit=2
https://jsonplaceholder.typicode.com/posts?_limit=7

Web8

https://jsonplaceholder.typicode.com/comments?postId=7&_limit=4,

Часть Значение
Схема https
Хост jsonplaceholder.typicode.com
Порт не написан, подразумевается 443
Путь -
Query postId=7&_limit=4

http://localhost:8080/tasks?page=2&sort=date

Часть Значение
Схема http
Хост localhost:
Порт 8080
Путь -
Query page=2&sort=date

https://api.example.com:3000/users/42/posts?status=active.

Часть Значение
Схема https
Хост api.example.com:
Порт 3000
Путь /users/42/
Query status=active.

Web9
Объектов в 10 (https://jsonplaceholder.typicode.com/posts?userId=2) 
Объектов в 10 (https://jsonplaceholder.typicode.com/users/2/posts) 
Результат один и тот же , данные добыты разнами путями 

Web10
Статус 200 GET (https://jsonplaceholder.typicode.com/users/1) (Вывел 1 из user)
Статус 404 GET(https://jsonplaceholder.typicode.com/users/11) (Не найдено)
Статус 200 GET (https://jsonplaceholder.typicode.com/users/1?foo=bar.) (Вывел 1 из user)
Сломалось при выводе /users/11 тк только 10 юзеров в одном id

Web11
Content-Type 	application/json; charset=utf-8
Content-Length 1847

Web12
Первая страница (_page=1): 5 объектов, id первого объекта - 1
Вторая страница (_page=2): 5 объектов, id первого объекта - 6
Параметр _page указывает номер отображаемой страницы при пагинации, сдвигая последовательность id дальше.
