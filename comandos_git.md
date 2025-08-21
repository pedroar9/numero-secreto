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
Link para testar comandos git
https://git-school.github.io/visualizing-git

---

### Entenda os comandos git restore e switch
https://unibb.alura.com.br/extra/alura-mais/entenda-os-comandos-git-restore-e-switch-c99

---

Os comandos `pop`, `drop` e `apply` do `git stash` possuem semelhanças e diferenças bem importantes:

### Apply
O comando `git stash apply` espera um índice de um item na stash e o aplica ao repositório,
porém, esse comando não remove o item da stash, ou seja, se após executar o comando `git stash apply 1` você executar `git stash list`, o item referente ao índice 1 continuará na stash.

### Pop
O `git stash pop` faz exatamente a mesma coisa que o `git stash apply`, porém, além de aplicar o item da stash,
ele também o remove de lá. Esse comando, sem nenhum parâmetro extra, vai aplicar o último item adicionado à stash, mas nós também podemos informar um índice para ele, como `git stash pop 1`.

### Drop
O `git stash drop` funciona exatamente como o `pop`, mas com uma simples diferença:
ele apenas remove o item da stash, sem aplicá-lo em nosso repositório. Dessa forma, `git stash drop` remove o último item adicionado à stash,
enquanto o `git stash drop 1` remove da stash o item com índice 1.

---
