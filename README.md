
## О проекте:
Учебный проект в ЯндексПрактикуме по основам бэкэнда (node.js) - промежуточный этап изучения node.js.
Темы API.REST и базы данных.
Итоговые наработки по node.js в репозитории https://github.com/Itauiti/mesto_deploy 

## Основной функционал: 
1. Создан сервер для проекта Mesto (вебпак проекта https://github.com/Itauiti/webpack-project.git)
2. Работа с БД - MongoDB (включая связи между схемами)
3. Роуты: 
- GET /users — возвращает всех пользователей
- GET /users/:userId - возвращает пользователя по _id
- POST /users — создаёт пользователя
- GET /cards — возвращает все карточки
- POST /cards — создаёт карточку
- DELETE /cards/:cardId — удаляет карточку по идентификатору
- PATCH /users/me — обновляет профиль
- PATCH /users/me/avatar — обновляет аватар
- PUT /cards/:cardId/likes — поставить лайк карточке
- DELETE /cards/:cardId/likes — убрать лайк с карточки

## Добавленные наработки:
- в .eslintrc добавлено исключение для _id;
- Node.js приложение подключается к серверу Mongo;
- созданы схема и модель пользователя с полями name, about и avatar, поля корректно валидируются;
- созданы схема и модель карточки с полями name, link, owner, likes и createdAt, поля корректно валидируются;
- запрос на GET /users возвращает всех пользователей из базы;
- запрос GET /users/:userId возвращает конкретного пользователя;
- запрос POST /users создаёт пользователя;
- запрос GET /cards возвращает все карточки всех пользователей;
- запрос POST /cards создаёт карточку;
- если в любом из запросов что-то идёт не так, сервер возвращает ответ с ошибкой и соответствующим ей статусом;

## Стэк технологий:
Node.js, express.js, MongoDBб, ES6, OOP, CSS3, HTML5, BEM

## Пакеты, которые используются в сборках:
- [body-parser](https://www.npmjs.com/package/body-parser)
- [express](https://expressjs.com)
- [validator](https://www.npmjs.com/package/validator)
- [helmet](https://helmetjs.github.io/)
- [express-rate-limit](https://www.npmjs.com/package/express-rate-limit)
- mongoose

## Инструкции по запуску:
- Скачать или склонировать репозитори
- Установить зависимости при помощи npm - `npm i`
- Подключиться к mongo `npm i mongoose`
- Запустить сервер на localhost:3000 - `npm run start`

