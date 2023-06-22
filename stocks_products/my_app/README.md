https://blog.bayrell.org/ru/linux/docker/25-sborka-dockerfile-na-primere-nginx.html
0) systemctl start docker
запуск докера
1) docker pull nginx - Скачайте заранее docker образ nginx
2) docker build -t image_nginx .  - Выполните сборку docker образа:
3) Будет создан docker образ с именем image_nginx. Его можно проверить командой docker images
4) docker run -d --name nginx -p 80:80 image_nginx - Создайте и запустите контейнер из образа
5) curl localhost:80 - проверка
nikita@nikita-R519-R719:~/Python/Netology/Hometasks/Hometask_6.1_docker$ curl localhost:80
<!DOCTTYPE html>
<html>
	<head>
		<title> Hello example </title>
	</head>
	<body>
		<p> Hello World! </p>
	</body>


