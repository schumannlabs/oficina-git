# Guia de bolso Git #

Local onde pode-se localizar fácilmente comandos do Git.

## Guia ##

| Comando | ação |
|:-|:-|
| git add . | Adiciona todas as mudanças à staging area |
| git commit -m "message" | Adiciona as mudanças que estão na staging area no repositório local |
| git commit -a -m "message" | Adiciona todas mudanças no repositório local (substitui git add . && git commit -m "message") |
| git checkout feature/nome-do-branch | Troca de branch |
| git push | Envia as mudanças no repositório local para o remoto |
| git checkout -b feature/new-branch | Cria um novo branch a partir do atual |
| git push -u origin feature/new-branch | Enviar um branch local para o Repositório remoto |
| git branch -d feature/new-branch | Deletar um branch local |
| git push origin --delete feature/new-branch | Deletar um branch remoto |
| git fetch | Verifica se houve alteração no Repositório Remoto e traz apenas aquelas que nçao gerem conflitos |
| git status | Verifica se houve mudanças no Repositório Local |
| git pull | Traz as mudanças do remoto para o local |
| git diff | Mostra todas linhas que mudaram, pode ser usado com --staged, ou apenas para um arquivos (coloca-se o caminho do mesmo após git diff) |
| git init | Instanciar um repositório git localmente |
| git add remote <https://repo_here> | Adicionar repositório remoto |
| git config user.name "exemplo" | Configurar username para um repositório local (para aplicar a todos repositórios em seu computadorusar a flag --global logo antes da configuração que quer mudar, e.g. git config --global user.name "exemplo") |
| git config user.email "exemplo@lorem.ipsum" | Configurar email para um repositório local |
| git config --global init.defaultBranch "main" | Troca o nome padrão do branch de repositórios criados localmente |
