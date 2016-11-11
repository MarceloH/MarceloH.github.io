---
published: true
title: Passo a passo ( Github e TortoiseGit) Windows
layout: post
tags: [github, tortoiseGit]
categories: [Tutorial]
---
1) baixe o tortoiseG - http://code.google.com/p/tortoisegit/downloads/list
2) Instale o Git - http://code.google.com/p/msysgit/downloads/detail?name=Git-1.7.4-preview20110204.exe&can=3&q=
3) Inicia - TortoiseGit - Puttygen
  3.1) Gerar a chave publica(copia - ctrl + c)
  3.2) Salvar a chave publica e a chave privada
4) Acesse sua conta no www.github.com
  4.1) Account settings > SSH Public Key > Add another public key
  4.2) Dê um titulo para sua chave public e cole o código da chave publica gerada no passo 3.1
5) Iniciar > TortoiseGit > Settings
  5.1) Vá no menu Config e preencha o campo Name e Email
6) Vá até o www.github.com, clique em Dashboard e localize na tela o link CREATE REPOSITORY
 6.1) Dê nome ao repositório e confirme sua criação.
  6.2) Copie o link do seu repositório. (Ex: git@github.com:maxanalista/Paciencia_e_a_chave.git)
7) Crie uma pasta em qualquer lugar do seu computador
  7.1) Clique com botão direito na pasta e selecione a opção Git Clone
  7.2) No campo URL, cole o link do seu repository(O link do seu repositorio foi copiado no passo 6.2)
  7.3) No campo Load Putty Key, clique nos link (...) e procure pela chave privada que você salvou no passo 3.2
  7.4) Dê Ok.
8) Abra a pasta criada no passo 7
  8.1) Caso não haja uma pasta chamada .git dentro da pasta com o nome do seu repositorio, configure seu Windows para que ele mostre pastas ocultas.

pronto !!