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

- Podemos **enviar nossos projetos** para o GitHub e disponibilizá-lo para outros desenvolvedores;

- O GitHub é gratuito tanto para projetos públicos como **privados**;

## Enviando repositórios para o GitHub

- Precisamos criar o projeto no GitHub, inicializar o mesmo no git em nossa máquina, sincronizar com o GitHub e enviar;

1. Utilize o comando `git init` para começar o processo

2. Adicione os arquivos que deseja subir para o repositório com o comando `git add (nome-do-arquivo)` ou `git add .` para adicionar todos os arquivos

3. Utilize o `git commit -m "first commit"` para criar um commit no seu repositório Git com a mensagem que desejar dentro dos aspas.
'
4. Utilize o comando `git remote add origin https://github.com/seu-usuario/nome-do-repositorio.git` para sincronizar o repositório no GitHub com o repositório local

5. Por fim, utilize o `git push -u origin master` para subir o seu projeto ao GitHub.

## Verificando mudanças no projeto

- As mudanças do projeto podem ser verificados por: **`git status`**;

- Aqui serão mapeadas todas as alterações do projeto;

- Como: **arquivos não monitorados** e **arquivos modificados**;

- Podemos também dizer a **diferença** do que já está enviado ao servidor ou salvo no projeto;

## Recebendo as mudanças
- É comum também ter que **sincronizar o local** com as mudanças do remoto;

- Esta ação é feita pelo **`git pull`**;

- Após o comando serão **buscadas atualizações**, se encontradas elas **serão unidas ao código atual** existente na nossa máquina;

## Clonando repositórios

- O ato de baixar um repositório de um servidor remoto é chamado de **clonar repositório**;

- Para esta ação utilizamos o **`git clone`**

- Este comando é utilizado quando **entramos em um novo projeto**;

## Removendo arquivos

- Os arquivos **podem ser deletados da monitoração** do git;

- O comando para deletar é **`git rm`**

- Após deletar um arquivo do git ele não terá mais suas atualizações consideradas pelo git;

- Apenas quando for adicionando novamente pelo **`git add`**

## Histórico de alterações

- Podemos **acessar um log** de modificações feitas no projeto;

- O comando para este recurso é **`git log`**;

- Você receberá uma informação dos **commits realizados** no projeto até então;

## Renomeando arquivos

- Com o comando **`git mv`** podemos renomear um arquivo;

- O mesmo também pode ser movido para outra pasta;

- E isso fará com que este novo arquivo **seja monitorado pelo git**;

- O arquivo anterior é excluído;

## Desfazendo alterações

- O arquivo modificado pode ser **retornado ao estado original**;

- O comando utilizado é o **`git checkout`**;

- Após a utilização do mesmo o arquivo sai do staging;

- Caso seja feita uma próxima alteração, ele entra em staging novamente;

## Ignorando arquivos no projeto

- Uma técnica muito utilizada é **ignorar arquivos no projeto;

- Devemos inserir um arquivo chamado **.gitignore** na raiz do projeto;

- Nele podemos inserir todos os arquivos que nao devem entrar no versionamento;

- Isso é útil para **arquivos gerados automaticamente** ou arquivos que contêm **informações sensíveis**;

## Desfazendo todas as alterações

- Com o comando **`git reset`** podemos resetar todas as mudanças feitas;

- Geralmente é utilizado com a flag **`--hard`**

- Todas as alterações **commitadas** e **também as pendentes** serão **excluídas**;

## O que é um branch

- Branch é a forma que o git **separa as versões dos projetos**;

- Quando um projeto é criado ele inicia na branch **master** ou **main**;

- Geralmente cada nova feature de um projeto **fica em um branch separado**;

- Após a finalização das alterações os **branchs são unidos** para ter o código-fonte final; 