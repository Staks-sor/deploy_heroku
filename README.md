# deploy_heroku
![#f03c15](https://placehold.it/15/f03c15/000000?text=Деплой бота на хероку на Python) `#f03c15`
Деплой бота на хероку на Python.<br>
В данном случае рассматривается aiogram<br>
1) Пишем бота <br>
2) Создаем requirements.txt - добавляем в него все используемые библиотеки.<br>
3) Создаем runtime.txt - добавляем версию python которую использовали. Но хероку поддерживает не все версии python. Посмотреть можно тут https://devcenter.heroku.com/articles/python-support <br>
4) Создаем Procfile Внимание данный фаил не содержит расширения. вписываем туда worker: python bot.py<br>
5) Скачиваем от сюда и устанавливаем  https://devcenter.heroku.com/articles/heroku-cli#download-and-install<br>
6) Скачиваем Git https://git-scm.com/downloads<br>
7) Далее запускаем консоль(терминал) переходим в папку проекта cd ваш путь к проекту.<br>
8) Пишем в консоль нажимаем любую кнопку кроме q, heroku login, откроется браузер где необходимо залогиниться.<br>
9) git init инициализируем.<br> 
10) git add . добавляем все<br> 
11) git commit -m "мой первый комит"<br>
12) Далее создаем апп в хероку heroku create имя бота.<br>
13) git remote -v <br>
14) git push heroku master<br> 
15) далее запускаем heroku ps:scale worker=1, чтобы отключить heroku ps:scale worker=0, посмотреть состояние heroku ps, посмотерть логи heroku logs<br>
Все ваш бот задепоин можно переходить в телеграм и играться с ботом.<br>

Внимание!!!<br>
Регистрация на хероку в данный момент невозможна из России, для того, что бы преодолеть данный барьер необходимо установить VPN.<br> 
После регистрации можно пушить файлы и с России. <br>





Initialise with git: git init<br>

Get the app name: heroku apps<br>

Add remote:<br>

heroku git:remote -a your_app_name<br>
Edit: You can also run commands without permanently adding the app<br>

heroku run -a your_app_name
