ELB
Запустить еще один инстанс веб приложения.
Цель: Запустить еще один инстанс веб приложения. Создать балансировщик нагрузки и закрепить его за двумя созданными инстансами, где работает веб приложение.

https://github.com/ugaidmitry/cloud/blob/master/elb/Screenshot%20from%202019-12-29%2020-45-33.png

1 ELB

http://wordpress-1d434fa4ac690c0a.elb.eu-north-1.amazonaws.com/

2 EC2 (httpd)

ec2-13-48-58-22.eu-north-1.compute.amazonaws.com

ec2-13-53-159-88.eu-north-1.compute.amazonaws.com

1 RDS(mysql 5.7)

1 EFS (mounted for each EC2)

 Балансировщик работает на уровне TCP перекидывая запросы на 80 порт на инстансы (round-robin)
 
