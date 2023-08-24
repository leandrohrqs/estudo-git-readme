<h1 align="center">Resumo Estudo Git</h1>

## Controle de Versão

### O que é controle de versão?

- Uma técnica que ajuda a **gerenciar o código-fonte** de uma aplicação;

- Registrando **todas as modificações** de código, podendo também reverter as mesmas;

- Criar versões de um software em diferentes estágios, podendo **alterar facilmente entre elas**;

- Cada membro da equipe pode trabalhar em uma versão diferente;

- Há ferramentas para trabalhar o controle de versão como **git** e SVN;

## O que é Git?

- O sistema de controle de versão **mais utilizado do mundo** atualmente (2023);

- O git é baseado em **repositórios**, que contêm todas as versões do código e também as cópias de cada desenvolvedor;

- Todas as operações do git **são otimizadas para ter alto desempenho**;

- Todos os objetos do git são **protegidos como criptografia** para evitar alterações indevidas e maliciosas;

- O git é um **projeto de código aberto**;

## O que é um repositório?

- é onde o código será **armazenado**;

- Na maioria das vezes cada projeto tem **um repositório**

- Quando criamos um repositório estamos iniciando um projeto;

- O repositório pode ir para servidores que são especializados em gerenciar repos, como: **GitHub** e **Bitbucket**;

- Cada um dos desenvolvedores do time pode baixar o repositório e **criar versões diferentes** em sua máquina;

## Criando repositórios

- Para criar um repositório utilizamos o comando: **`git init`**

- Desta maneira o git vai criar os arquivos necessários para inicializá-lo;

- Os arquivos criados estão na pasta oculta **.git**;

- Após este comando o diretório atual **será reconhecido pelo git como um projeto** e responderá aos seus demais comandos;

## O que é github?

- É um **serviço para gerenciar repositórios**, gratuito e amplamente utilizado;

- Podemos **enviar nossos projetos** para o GitHub e disponibilizá-lo para outros devs;

- O GitHub é gratuito tanto para projetos públicos como **privados**;

## Enviando repositórios para o GitHub

- Precisamos criar o projeto no GitHub, inicializar o mesmo no git em nossa máquina, sincronizar com o GitHub e enviar;

1. Utilize o comando `git init` para começar o processo

2. Adicione os arquivos que deseja subir para o repositório com o comando `git add (nome-do-arquivo)` ou `git add .` para adicionar todos os arquivos

3. Utilize o `git commit -m "first commit"` para criar um commit no seu repositório Git com a mensagem que desejar dentro dos aspas.
'
4. Utilize' o comando `git remote add origin https://github.com/seu-usuario/nome-do-repositorio.git` para linkar o repositório no GitHub com o repositório local

5. Por fim, utilize o `git push -u origin master` para subir o seu projeto ao GitHub.
