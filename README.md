# learning_devops
Первый урок: установка ubuntu + git + docker , первоначальаня настройка
step-by-step: 
1. Стягиваем себе приложение : git clone https://github.com/ChillTurtl3/learning_devops.git
2. Переходим в директорию с проектом: cd learning_devops/myapp/
3. Запускаем сборку образа : docker build -t myapp . \\ на основе вложенного докерфайла создается образ приложения, который впоследствии можно запустить
4. Запускаем контейнер на порту 8000 с именем test-app из полученного образа : docker run -d -p 8000:8000 --name test-app myapp
