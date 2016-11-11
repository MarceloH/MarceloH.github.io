---
published: true
title: Exportar dados do PostgreSQL
layout: post
tags: [postgresql, psql, sql]
categories: [PostgreSQL]
---
Colunas com inserts:
pg_dump -U user_name -h localhost -t table_name --data-only --column-inserts        db_name > data_dump.sql

Tabelas apenas:
pg_dump -s -U postgres adminsicom  | awk 'RS="";/CREATE TABLE[^;]*;/'

Sequenciais apenas: 
pg_dump -s -U postgres adminsicom  | awk 'RS="";/CREATE SEQ[^;]*;/'