# :octocat: Oficina de Git e Github SchumannLabs [:link:](https://github.com/schumannlabs/oficina-git) #

Este repositรณrio foi criado para servir como material de apoio em uma oficina sobre Git e Github feita na [@schumannlabs](https://github.com/schumannlabs).

[Guia de bolso](guia-de-bolso.md)

## ๐ Sumรกrio ##

- [:octocat: Oficina de Git e Github SchumannLabs :link:](#octocat-oficina-de-git-e-github-schumannlabs-link)
  - [๐ Sumรกrio](#-sumรกrio)
  - [๐ฐ Iniciando](#-iniciando)
    - [โ๏ธ Configurando Git](#๏ธ-configurando-git)
    - [๐ฅ Baixando um repositรณrio](#-baixando-um-repositรณrio)
      - [๐ฅ๐ฉโ๐ป Via terminal](#-via-terminal)
      - [๐ฅ๐บ Via Github Desktop](#-via-github-desktop)
    - [๐ฒ Branches](#-branches)
      - [๐๐ฒ Alternando entre branches](#-alternando-entre-branches)
        - [๐๐ฒ๐ฉโ๐ป Via terminal](#-via-terminal-1)
        - [๐๐ฒ๐บ Via Github Desktop](#-via-github-desktop-1)
      - [โ๐ฒ Criando um novo branch localmente](#-criando-um-novo-branch-localmente)
        - [โ๐ฒ๐ฉโ๐ป Via terminal](#-via-terminal-2)
        - [โ๐ฒ๐บ Via Github Desktop](#-via-github-desktop-2)
      - [๐ค๐ฒ Subindo um branch Local para o remote](#-subindo-um-branch-local-para-o-remote)
        - [๐ค๐ฒ๐บ Via Github Desktop](#-via-github-desktop-3)
      - [๐ฎ๐ฒ๐  Deletando um branch Local](#-deletando-um-branch-local)
        - [๐ฎ๐ฒ๐ ๐บ Via Github Desktop](#-via-github-desktop-4)
      - [๐ฎ๐ฒ๐ Deletando um branch remoto](#-deletando-um-branch-remoto)
        - [๐ฎ๐ฒ๐๐บ Via Github Desktop](#-via-github-desktop-5)
    - [๐ Manipulando arquivos no git](#-manipulando-arquivos-no-git)
      - [โ๐ Adicionando arquivos novos ou modificados](#-adicionando-arquivos-novos-ou-modificados)
        - [Um arquivo](#um-arquivo)
        - [Todos novos arquivos e mudanรงas](#todos-novos-arquivos-e-mudanรงas)
        - [โ๐๐บ Via Github Desktop](#-via-github-desktop-6)
      - [๐ฆ๐ Adicionando eles de fato ao repositรณrio local](#-adicionando-eles-de-fato-ao-repositรณrio-local)
        - [๐ฆ๐๐บ Via Github Desktop](#-via-github-desktop-7)
      - [๐ค๐๐ Enviando as mudanรงas para o repositรณrio remoto](#-enviando-as-mudanรงas-para-o-repositรณrio-remoto)
        - [๐ค๐๐๐บ Via Github Desktop](#-via-github-desktop-8)
      - [๐๐ Verificando o status do repositรณrio local](#-verificando-o-status-do-repositรณrio-local)
        - [๐๐๐บ Via Github Desktop](#-via-github-desktop-9)
      - [๐ฅ๐๐ Trazendo mudanรงas do repositรณrio remoto](#-trazendo-mudanรงas-do-repositรณrio-remoto)
        - [๐ฅ๐๐๐บ Git Pull via Github Desktop](#-git-pull-via-github-desktop)
        - [๐ฅ๐๐๐บ Git Fetch via Github Desktop](#-git-fetch-via-github-desktop)
    - [โ๐๐ฒ Criando repositรณrios Git](#-criando-repositรณrios-git)
      - [โ๐๐ฒ๐บ Criar repositรณrio local pelo Github Desktop](#-criar-repositรณrio-local-pelo-github-desktop)
      - [โโ๏ธ๐๐ฒ Tรก eu tenho um repositรณrio local mais e o remoto ?](#๏ธ-tรก-eu-tenho-um-repositรณrio-local-mais-e-o-remoto-)
      - [โโ๏ธ๐๐ฒ๐บ Via Github Desktop](#๏ธ-via-github-desktop)
      - [๐ป Ok, agora eu tenho um repositรณrio local referenciado ร  um remoto, qual o prรณximo passo ?](#-ok-agora-eu-tenho-um-repositรณrio-local-referenciado-ร -um-remoto-qual-o-prรณximo-passo-)
  - [๐ฃ FAQ](#-faq)
    - [โ Git e Github sรฃo a mesma coisa ?](#-git-e-github-sรฃo-a-mesma-coisa-)
  - [๐ Going Deeper](#-going-deeper)
  - [๐ฅ Autores](#-autores)
    - [๐ฆ Ruan Pato](#-ruan-pato)
  - [๐ Referรชncias](#-referรชncias)

## ๐ฐ Iniciando ##

1. Instale o [Git](https://git-scm.com/downloads/) em seu computador: <https://git-scm.com/downloads/>, caso queira utilizar uma interface grรกfica para usar o Git, recomendo o [Github Desktop](https://desktop.github.com/): <https://desktop.github.com/>.
2. [Crie uma conta](https://github.com/join) no Github - <https://github.com/join>;
3. Caso esteja usando Github Desktop, faรงa login que ele irรก configurar o git com suas credenciais;
4. Caso esteja usando o Git via CLI na prรณxima secรงรฃo tem os comandos que serรฃo necessรกrios;

Como funcionam repositรณrios git ?
Local รฉ a versรฃo do repositรณrio que estรก baixada na mรกquina (e.g. Seu Computador), Remote รฉ o repositรณrio que estรก no servidor (e.g. Github);

![Git Local Remote](imagens/gitLocalRemote.jpg)
Ref: <https://phpenthusiast.com/blog/the-essentials-of-git-and-github-for-web-developers>

![Git Areas](imagens/gitAreas.jpg)
Ref: <https://www.slideshare.net/tchelinux/git-em-pequenos-projetos-sandro-custdio-tchelinux-livramento-2019>

Veja: <https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control>

### โ๏ธ Configurando Git ###

Ao modificar configuraรงรตes do git, pode-se escolher o escopo destas, seja no repositรณrio onde a pasta .git/ estรก, ou para todos os repositรณrios git no computador;

E.g. Configurando um mesmo user.name para todos repositรณrios git no computador:

```bash
> git config --global user.name "exemploschumann"
```

No exemplo acima todos repositรณrios git usaram o user.name exemploschumann para se comunicar com o repositรณrio origem.

E.g. Configurando um email para apenas um repositรณrio:

```bash
C:/Users/exemplo/Documents/oficina-git> git config user.email "exemplo1@schumann.com.br"
```

O user.name e user.email sรฃo obrigatรณrios para usar o git, porรฉm existem vรกrias outras configuraรงรตes que podem ser alteradas, pode-se vรช-las usando:

```bash
git config --list
```

Veja: <https://git-scm.com/docs/git-config>

### ๐ฅ Baixando um repositรณrio ###

Para baixar um repositรณrio git para sua mรกquina รฉ precisar fazer um Git Clone, que cria uma versรฃo do que estรก na nuvem em sua mรกquina local.

Veja: <https://git-scm.com/docs/git-clone>

#### ๐ฅ๐ฉโ๐ป Via terminal ####

Apรณs isso, abra o terminal (cmd, powershell, ...) navegue atรฉ onde tu quer baixar este repositรณrio e rode o seguinte comando:

Para poder baixar repositรณrios privados, e realizar mudanรงas no repositรณrio remoto, รฉ necessรกrio se autenticar, recomendo criar e adicionar uma chave SSH ao Github: <https://docs.github.com/pt/github/authenticating-to-github/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent>
> <http://guides.beanstalkapp.com/version-control/git-on-windows.html>

```bash
git clone git@github.com:schumannlabs/oficina-git.git
```

#### ๐ฅ๐บ Via Github Desktop ####

1. Vรก em File -> Clone Repository (Ou pressione: *Ctrl + Shift + O*);
2. Selecione URL -> Adicione a URL deste repositรณrio, escolha o local onde o repositรณrio serรก baixado.

### ๐ฒ Branches ###

![Imagem1](imagens/branches.png)

Pode se definir cruamente, como se Branches fossem 'cรณpias' do projeto de um determinado ponto (commit)

>Mas isso significa que o projeto vai ter tamanho de multiplicado pelo nรบmero de branches que ele tiver ?
>
>Nรฃo. Pois o git trabalha com referรชncias.
>
> Veja:
>
> <https://git-scm.com/book/en/v2/Git-Internals-Git-References>
>
> <https://www.freecodecamp.org/news/git-internals-for-curious-developers-a1e44e7ecafe/#:~:text=In%20other%20words%2C%20Git%20copies,what%20makes%20Git%20so%20quick.>

Veja:

- Site para treinar uso de branches: <https://learngitbranching.js.org/?locale=pt_BR>
- <https://git-scm.com/docs/git-branch>
- <https://git-scm.com/docs/git-checkout>
- <https://git-scm.com/docs/git-switch>
- <https://git-scm.com/docs/git-merge>
- <https://git-scm.com/docs/git-mergetool>
- <https://git-scm.com/docs/git-log>
- <https://git-scm.com/docs/git-stash>
- <https://git-scm.com/docs/git-tag>
- <https://git-scm.com/docs/git-worktree>

#### ๐๐ฒ Alternando entre branches ####

Suponde que vocรช estรก em um repositรณrio que possui vรกrios branches, pode-se alterar localmente a versรฃo dos arquivos de acordo com o branch usando o seguinte comando:

##### ๐๐ฒ๐ฉโ๐ป Via terminal #####

```bash
git checkout homologation
```

##### ๐๐ฒ๐บ Via Github Desktop #####

![Switch branch Github Desktop](imagens/GithubDesktopSwitchBranch.png)

#### โ๐ฒ Criando um novo branch localmente ####

Quando vai se criar um novo branch, deve-se dizer ร  partir de qual este serรก criado.

##### โ๐ฒ๐ฉโ๐ป Via terminal #####

Pode-se utilizar o checkout para criar um novo branch a partir do atual:

```bash
git checkout -b feature/9221
```

##### โ๐ฒ๐บ Via Github Desktop #####

1. Vรก em Branch -> New Branch (Ou pressione: *Ctrl + Shift + N*);
2. Digite o nome do novo branch, ex: feature/nomeBranch e selecione a partir de qual branch esse serรก criado.

#### ๐ค๐ฒ Subindo um branch Local para o remote ####

```bash
git push -u origin HEAD
```

**-u** = --set-upstream

##### ๐ค๐ฒ๐บ Via Github Desktop #####

![Github Desktop Publish Local Branch](imagens/GithubDesktopPublishLocalBranch.png)

#### ๐ฎ๐ฒ๐  Deletando um branch Local ####

```bash
git branch -d feature/9221
```

##### ๐ฎ๐ฒ๐ ๐บ Via Github Desktop #####

1. Vรก em Branch -> Delete Branch (Ou pressione: Ctrl + Shift + D);
2. Confirme na caixa de dialogo que quer deleter.

#### ๐ฎ๐ฒ๐ Deletando um branch remoto ####

```bash
git push origin --delete feature/9221
```

##### ๐ฎ๐ฒ๐๐บ Via Github Desktop #####

1. Vรก em Branch -> Delete Branch (Ou pressione: Ctrl + Shift + D);
2. Digite o nome do novo branch, ex: feature/nomeBranch e selecione a partir de qual branch esse serรก criado.

### ๐ Manipulando arquivos no git ###

Para explicar manipulaรงรฃo de arquivos vou usar a forma que este [artigo](https://dev.to/sublimegeek/git-staging-area-explained-like-im-five-1anh#:~:text=You%20can%20take%20stuff%20out,that%20box%20are%20your%20changes.) fez.

#### โ๐ Adicionando arquivos novos ou modificados ####

Imagine que a รกrea de staging do git รฉ como uma caixa que estรก na sua mesa, onde tu pode adicionar objetos, seja um por vez, ou todos, para isso usamos o **git add**.

Veja: <https://git-scm.com/docs/git-add>

##### Um arquivo #####

```bash
git add gambiarra/4952.cpp
```

##### Todos novos arquivos e mudanรงas #####

```bash
git add .
```

ou

```bash
git add -A
```

##### โ๐๐บ Via Github Desktop #####

O equivalente ao git add, sรฃo as caixas de seleรงรฃo dos arquivos:

![Github Desktop Git add](imagens/GithubDesktopGitAdd.png)

Os que estรฃo selecionados irรฃo para staging area, como se fosse um git add nestes.

#### ๐ฆ๐ Adicionando eles de fato ao repositรณrio local ####

Quando vocรช tem uma caixa que estรก com objetos, para envia-las para o depรณsito se faz necessรกrio fecha-la e rotular a mesma, para isso usa-se o git **commit**.

```bash
git commit -m "Tรญtulo do Rรณtulo da caixa" -m "Mais informaรงรตes sobre a caixa no rรณtulo" -m "Pode-se usar o -m vรกrias vezes, ele cria como se fossem paragrรกfos a cada novo -m" -m "Lembre-se de escrever tรญtulos curtos e descritivos no tรญtulo do commit"
```

**Hack:**
Vocรช pode tambรฉm simplesmente ao invรฉs de usar o git add para adicionar cuidadosamente os itens na "caixa" usar a flag -a no commit sem ter usado o git add antes, que รฉ como se vocรช passasse o braรงo na mesa jogasse todos os itens dela na caixa, jรก colocar fechar e rotular ela.

```bash
git commit -a -m "Jogando tudo da mesa na caixa" -m "Literalmente adicionando toda e qualquer mudanรงa que ocorreu no Working Directory para o repositรณrio"
```

Veja: <https://git-scm.com/docs/git-commit>

##### ๐ฆ๐๐บ Via Github Desktop #####

Para realizar um commit, basta preencher a mensagem de commit, colocar descriรงรฃo ou co-autor caso queira e entรฃo clicar em commit:

![Github Desktop Git Commit](imagens/GithubDesktopGitCommit.png)

Os que estรฃo selecionados irรฃo para staging area, como se fosse um git add nestes.

#### ๐ค๐๐ Enviando as mudanรงas para o repositรณrio remoto ####

ร como se vocรช pegasse todas as caixas que estรฃo prontas para serem transportadas e as entregasse para um serviรงo que vai "magicamente" criar cรณpias delas e leva-las ao seu depรณsito, para fazer isso deve-se usar o **git push**

```bash
git push
```

Obs. O serviรงo que vai entregar essas mudanรงas vai conferir primeiro se o que enviou pode ser entregue, pois pode ser que exista conflitos.

##### ๐ค๐๐๐บ Via Github Desktop #####

Para realizar um commit, basta preencher a mensagem de commit, colocar descriรงรฃo ou co-autor caso queira e entรฃo clicar em commit:

![Github Desktop Git Commit](imagens/GithubDesktopGitCommit.png)

Os que estรฃo selecionados irรฃo para staging area, como se fosse um git add nestes.

#### ๐๐ Verificando o status do repositรณrio local ####

Para ver o que tem na caixa que estรก na sua mesa, nas caixas que estรฃo ao seu redor, ou em ambas usa-se o comando **git status**:

```bash
git status
```

Veja: <https://git-scm.com/docs/git-status>

##### ๐๐๐บ Via Github Desktop #####

As mudanรงas no seu repositรณrio, sรฃo visรญveis na barra lateral esquerda, no mesmo local onde tu escolhe se vai adicionar ou nรฃo a mudanรงa do arquivo ao prรณximo commit:

![Github Desktop Git Status](imagens/GithubDesktopGitStatus.png);

#### ๐ฅ๐๐ Trazendo mudanรงas do repositรณrio remoto ####

Lembra do depรณsito que foi comentado antes (repositรณrio remoto), quando รฉ preciso trazer as coisas que estรฃo nele para vocรช (repositรณrio local) pode-se usar dois comandos **git fetch** ou **git pull**, mas qual a diferenรงa ?

O **git fetch** verifica as mudanรงas que ocorreram no depรณsito, e traz apenas as que nรฃo vรฃo conflitar com as locais, รฉ como se as caixas que estรฃo aqui, apenas fossem ganhar novos objetos, e nรฃo perder nenhum.

Veja: <https://git-scm.com/docs/git-fetch>

Jรก o **git pull** traz todas as mudanรงas que ocorreram lรก, podendo remover objetos, ou mudar estes que estรฃo localmente.

Veja: <https://git-scm.com/docs/git-fetch>

##### ๐ฅ๐๐๐บ Git Pull via Github Desktop #####

1. Vรก em Repository -> Pull (Ou pressione: *Ctrl + Shift + P*);

##### ๐ฅ๐๐๐บ Git Fetch via Github Desktop #####

Basta clicar em Fetch:

![Github Desktop Fetch](imagens/GithubDesktopGitFetch.png)

### โ๐๐ฒ Criando repositรณrios Git ###

Como eu crio um repositรณrio Git local ๐  ?
Para isso utiliza-se o comando **git init** dentro de uma pasta, que irรก "transformar" essa em um repositรณrio Git.

```bash
git init
```

#### โ๐๐ฒ๐บ Criar repositรณrio local pelo Github Desktop ####

1. Vรก em File -> New Repository (Ou pressione *Ctrl + N*)
2. Preencha as informaรงรตes, e seleciona as opรงรตes que deseja.

#### โโ๏ธ๐๐ฒ Tรก eu tenho um repositรณrio local mais e o remoto ? ####

Devemos seguir a arquitetura do Git, para isso รฉ necessรกrio um repositรณrio remoto, como estamos usando Github nesta oficina, deve-se criar um repositรณrio lรก e dizer para nosso repositรณrio local que aquele รฉ o remoto, para isso usamos o **git add remote**:

```bash
git add remote https://github.com/nomeDoSeuUsuario/nomeDoRepositorioRemoto
```

#### โโ๏ธ๐๐ฒ๐บ Via Github Desktop ####

Com o repositรณrio local criado e selecionado pelo Github Desktop, serรก possรญvel criar o Remoto usando o atalho *Ctrl + P*, ou clicando em uma das opรงรตes de publicar o mesmo:

![Gituhub Desktop Create Remote Repository](imagens/GituhubDesktopCreateRemoteRepo.png)

#### ๐ป Ok, agora eu tenho um repositรณrio local referenciado ร  um remoto, qual o prรณximo passo ? ####

Agora tu pode jรก manipular os arquivos, por exemplo adicionando ([*git add*](#-adicionando-arquivos-novos-ou-modificados)) algo ao repositรณrio local, commitando ([*git commit*](#-adicionando-eles-de-fato-ao-repositรณrio-local)) e entรฃo enviando eles ao remoto ([*git push*](#-enviando-as-mudanรงas-para-o-repositรณrio-remoto)).

## ๐ฃ FAQ ##

### โ Git e Github sรฃo a mesma coisa ? ###

>Nรฃo

- **Git:** Uma ferramenta de controle de versรฃo distribuรญdo;
- **Github:** Plataforma de hospedagem de cรณdigos fontes/arquivos que usa o Git para controle de versรฃo, alรฉm de servir tambรฉm como um comunidade.

## ๐ Going Deeper ##

- Explicaรงรฃo das estruturas computacionais/matemรกticas que o git usa em sua construรงรฃo: <https://stackoverflow.com/a/18588431>;
- Pรกgina estilo slide de Conceitos do Git Simplificados: <https://gitolite.com/gcs#(1)>;
- Git for Computer Scientists <https://eagain.net/articles/git-for-computer-scientists/>.

## ๐ฅ Autores ##

### ๐ฆ Ruan Pato ###

Criador da primeira versรฃo do material da primeira oficina sobre o assunto.

- [Perfil pessoal do Github](https://github.com/ruanpato);
- [Perfil da schumannlabs do Github](https://github.com/ruanpatoschumann).

Caso tenha alguma dรบvida basta mandar um email ou me contatar pelos meios de comunicaรงรฃo usados pela SchumannLabs, basta pesquisar por Ruan Pato ou Ruan Guerra.

## ๐ Referรชncias ##

- [Git Docs](https://git-scm.com/docs) - <https://git-scm.com/docs>;
- [Github Docs](https://docs.github.com/pt/github/getting-started-with-github/quickstart) - <https://docs.github.com/pt/github/getting-started-with-github/quickstart>;

**Imagens:**

- [Imagem 1](https://stackoverflow.com/a/20755706) - <https://stackoverflow.com/a/20755706>;

**Links Uteis:**

- Cursos sobre uso de Git e Github: <https://lab.github.com/>;
