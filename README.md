# Spring Boot Application Demo

> Supervisor Configuration Example

```
$ sudo touch /etc/supervisor/conf.d/demo.config
```

**content**    

```
[program:demo]
command=java -jar /home/ubuntu/demo.jar
autostart=true
autorestart=true
stderr_logfile=/var/log/demo.err.log
stdout_logfile=/var/log/demo.out.log
```

> Enable Supervidor Interface Web

```
$ sudo vim /etc/supervisor/supervisord.conf 
```

**add content**   

```
[inet_http_server]
port = 9001
username = ubuntu
password = 123456
```
