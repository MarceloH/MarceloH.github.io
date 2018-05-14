---
published: true
title: Retornando a posição dos campos do PostgreSQL
layout: post
tags: [postgresql, psql, sql]
categories: [PostgreSQL]
---
> SELECT c.relname,
       a.attname,
       a.attnum
FROM pg_attribute a
INNER JOIN pg_class c ON c.oid = a.attrelid
AND c.relkind = 'r'
WHERE a.attnum > 0
  AND a.attisdropped <> 't'
ORDER BY 1,
         3

attnum = Número da posição
attname = Nome do campo
relname = Nome da Tabela