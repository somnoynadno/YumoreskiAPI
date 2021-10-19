# YumoredkiBot

 Бот для ВК, жмыхающий юморесками в беседу.
 
 Он триггерится на любые подстроки "анек" и "юмор" в сообщениях и отправляет случайный анекдот с паблика [Мои любимые юморески](https://vk.com/jumoreski).
 
 Достаточно добавить [бота](https://vk.com/public208001231) в беседу и дать права администратора, чтобы начать с ним работать.
 
 ## Запуск на собственном сервере
 
 Для ручного запуска необходимо:
 
 1. Создать сообщество в ВК, найти его ID, а также получить для него токен для LongPolling и access-токен для ВК API.
 
 2. Установить переменные окружения `ACCESS_TOKEN`, `BOT_TOKEN` и `COMMUNITY_ID` со всем вышеперечисленным.
 
 3. Запустить исполняемый файл: ```$ python3 bot.py```.
 
 Запуск в контейнере:
 
 1. Прописываем переменные окружения в ```.env``` файл корневой директории репозитория.
 
 2. Выполняем ``` $ docker-compose up --build -d``` для старта контейнера в фоновом режиме.
