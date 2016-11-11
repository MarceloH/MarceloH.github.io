---
published: true
title: Retornando posição dos campos do banco de dados
layout: post
---
SELECT c.relname,
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