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

## Criando e visualizando os branches

- Para visualizar os branch disponíveis, basta digitar **`git branch`**;

- Para criar um branch, você precisa utilizar o comando **`git branch <nome>`**;

## Deletando branches

- Podemos deletar um branch com a flag **`-d`** ou **`--delete`**;

- Exemplo: **`git branch -d <nome-da-branch>`**

- **Não é comum deletar um branch**, normalmente guardamos os histórico do trabalho;

- Geralmente se usa o delete quando o branch foi criado errado;

## Mundando de branch

- Podemos mudar para outro branch utilizando o comando **`git checkout <nome-da-branch>`**;

- Podemos criar um branch e mudar para ele no mesmo comando apenas adicionando a flag **`-b`** antes do nome da branch;

- Exemplo: **`git checkout -b <nome-da-branch>`**

## Unindo branches

- O código de dois branches distintos pode ser unido pelo comando **`git merge <nome>`**;

- Normalmente é por ele que recebemos as atualizações de outros devs;

## Stash

- Podemos salvar as modificações atuais **para prosseguir com uma outra abordagem de solução** e não perder o código;

- O comando para esta ação é o **`git stash`**;

- Após o comando o branch será resetado para a sua versão de acordo com o repositório;

## Recuperando stash

- Podemos verificar as stashs criadas pelo comando **`git stash list`**;

- Também podemos recuperar a stash com o comando **`git stash <nome>`**;

- Desta maneira podemos continuar de onde paramos com os arquivos adicionados a stash;

## Removendo a stash

- Para limpar totalmente as stash de um branch podemos utilizar o comando **`git stash clear`**;

- Caso seja necessário deletar uam stash específica podemos utilizar o comando **`git stash drop <nome>`;

## Criando tags

- Podemos criar tags nos branches por meio do comando **`git tag -a <nome> -m "<msg>"`

- A tag é diferente do stash, serve como um **checkpoint de um branch**;

- É utilizada para demarcar estágios do desenvolvimento de algum recurso;

## Alterando a tag

- Podemos verificar uma tag com o comando **`git show <nome-tag>`**

- Podemos trocar de tags com o comando **`git checkout <nome-tag>`**

- Desta maneira podemos retroceder ou avançar em checkpoints de um branch;

## Enviando e compartilhando tags

- As tags podem ser **enviadas para o repositório de código** sendo compartilhada entre os devs;

- O comando é **`git push origin <nome>`**;

- Ou se você quiser enviar mais tags **`git push origin --tags`**;

## Encontrando branches

- Branches novos são criados a todo tempo e **o git pode não estar mapeando ele**;

- Com o comando **`git fetch`** você é atualizado de todos os branches e tags que ainda não estão reconhecidos;

- Este comando é útil para utilizar o branch de algum outro dev do time;

## Recebendo alterações

- O comando **`git pull`** serve para recebermos atualizações do repositório remoto;

- Cada branch pode ser atualizado com o `git pull`;

- Utilizamos para atualizar a master do repositório como também quando trabalhamos em conjunto e queremos receber as atualizações de um dev;

## O comando **`git push `** faz o inverso do pull, ele envia as alterações para o repositório remoto;

- Serve também para **enviar as atualizações de um branch específico** para um outro dev;

- Ou quando terminamos uma tarefa e precisamos enviar ao repositório;

## Utilizando o remote

- Com o **`git remote`** podemos fazer algumas ações como: adicionar um repositório para trackear ou remover;

- Quando criamos um repositório remoto, adicionamos ele ao git com **`git remote add origin <link>`;

## Trabalhando com submódulos

- Submódulo é a maneira que temos de possuir **dois ou mais projetos em um só repositório**;

- Podemos adicionar uma dependência ao nosso projeto atual, porém mantendo suas estruturas separadas;

- Para adicionar o submódulo utilizamos o comando **`git submodule add <repositório>`**

- Para verificar os submódulos o comando é **`git submodule`**

## Atualizando submódulos

- Para atualizar um submódulo primeiro devemos **commitar as mudanças**;

- E para enviar para o repo do submódulo utilizamos **`git push --recurse-submodules=on-demand`**

- Este fluxo fará a atualização apenas do submódulo;