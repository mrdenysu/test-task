# Тестовое задание: JS

## Перед выполнением

- Перейти в `config/env/local.json` и прописать свою строку подключения к БД
- Там же, прописать желаемый порт, на который будет биндиться приложение (Можно оставить и 3010, если в системе нет конфликтов)
- В корне проекта выполнить `npm install`

## Запуск

- `npm run dev` - запустит приложение с помощью nodemon (автоматически перезапустит приложение при изменениях)
- `npm start` - запустит приложение в PROD режиме, приложение не будет перезапущено при изменениях

## Выполнение задания

- Сервер должен отдать список самых длинных дорог, отсортированных по убыванию. Код для этого следует писать в файле `routes/roads/longestRoads.js`
- На клиенте должна отобразиться таблица с списком этих дорог. Файлы для клиентов следует помещать в каталог `public`.
  Эти файлы будут доступны при обращении к ним по `http://localhost:{порт из конфига}/{имя файла}`
- На клиенте разрешается использовать любые библиотеки (использование React будет плюсом)
- Для тестов клиента будет использоваться актуальная версия Firefox ESR (78.3.0)

_PS: Я протестировал серверную часть с помощью Node 8.10 и PostgreSQL 11.9. Если что-то не заработает - можно менять версии зависимостей в package.json_

> Критерии приемки:

- API работает и возвращает правильные данные;
- Клиентская страница открывается и работает в актуальной версии Firefox ESR (78).
