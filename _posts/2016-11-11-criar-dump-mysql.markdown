---
published: true
title: Criar dump mysql
layout: post
tags: [dump, mysql, sql, tutorial]
categories: [Tutorial]
---
Para fazer um backup com o mysql, você pode usar o seguinte comando:

>$mysqldump -h localhost -u armenio -pjujuba meuBanco > backup_meuBanco.sql

Onde:

>Database: meuBanco
Host:     localhost
Username: armenio
Password: jujuba

Para restaurar o backup, execute o comando:

>$mysql -h localhost -u armenio -pjujuba meuBanco < backup_meuBanco.sql
