## Comandos Git

Visualizar nossa lista de commits, o registro de versionamento.
Para sair dessa visualização do `git log`, simplesmente pressionamos a tecla `q`
`git log`


Permitirá visualizar o log de commits de forma muito mais resumida.
`git log --oneline`

Nos fornece, além das informações padrão, o hash completo, o autor ou autora, a data e a mensagem do commit.
`git log -p`

---

Conseguimos visualizar o log de uma forma mais visual.
`git log --graph`

---

O hash do commit e o autor de cada commit é exibido
`git log --format="%H %an"`

---

Temos um manual, uma ajuda desse comando.
`git log --help`

---

`git log --oneline` e copiar o hash da alteração escolhida e inserir no comando `git show hash`
`git show 5880fc1`

---

Quais são as ramificações existentes no nosso trabalho.
`git branch`

---

Se quisermos renomear a master para main
`git branch -m master main`

Se quisermos remover alguma branch, caso tenhamos uma lista de várias branches,
podemos usar o comando `git branch -d` seguido do nome da branch que queremos remover
`git branch -d master`

Basta digitar o comando git branch seguido do nome do ramo que queremos trabalhar.
`git branch gramatica`

---

Alternando entre branches
`git checkout gramatica`

Para criar uma branch e já mover para ela, podemos usar dois comandos.
`git checkout -b nova-funcionalidade`
ou
`git switch -c nova-funcionalidade`

---

### Entenda os comandos git restore e switch
https://unibb.alura.com.br/extra/alura-mais/entenda-os-comandos-git-restore-e-switch-c99

---
