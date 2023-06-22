1) systemctl start docker
запуск докера
2)docker build ./ --tag app_1
сборка образа
3)docker run --name my_app -d -p 8000:6090 app_1
запуск





