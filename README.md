
# Git Commit Guidelines

> Este guia foi montado baseado em [uma convenção](https://github.com/angular/angular.js/blob/master/DEVELOPERS.md#-git-commit-guidelines) usada em conjunto com [commitizen](https://github.com/commitizen/cz-cli). 
Criei com o objetivo pessoal para melhorar minhas mensagens de commits e coroborar para o(s) projeto(s) para qual possa vir a participar, facilitando o rastreamento de mudanças e elucidando qualquer dúvida. 


## Formato da mensagem
A mensagem de commit possui três partes: 
- `header`
- `body`
- `footer`

Sendo estas partes definidas pelo template abaixo:
```
<type>(<scope>): <subject>
<quebra de linha>
<body>
<quebra de linha>
<footer>
```
Onde:
- *header* - `<type>(<scope>): <subject>`
- *body* - `<body>`
- *footer* - `<footer>`

Tanto o `header` e o `body` são **obrigatórios**, diferente do `footer`, que é **opcional**.
Importante ressaltar que a **mensagem não deve ter mais do que 100 caracteres**, assim a leitura é facilitada tanto no GitHug, quanto em outras ferramentas de versionamento

## Type
Tipos disponíveis:

* **feat**: nova feature
* **fix**: correção de bug
* **docs**: mudança de documentação
* **style**: mudanças que não alteram o funcionamento do código (espaços em branco, formatação, falta de ponto e vírgula e etc)
* **refactor**: mudança de código que não corrige bugs e não implementa feature
* **perf**: melhoria de performance
* **test**: adição ou correção de teste
* **chore**: tarefas de processos ou ferramentas auxiliares
* **revert**: revert de commit

## Scope
O scope é opcional e refere-se a qualquer mudança específica, como: `$location`,
`$browser`, `$compile`, `$rootScope`, `ngHref`, `ngClick`, `ngView` e etc...

Use `*` quando houver multiplos escopos, mas evite, pois definindo o escopo em cada commit você terá commits atômicos, gerando maior flexibilidade.

## Subject
Descrição sucinta da troca. Seguir as seguintes regras:
* use verbos interativos
* não usar letras maiúsculas no início da frase
* não usar ponto final

## Body
Assim como o **subject**, usar as mesmas regras, exceto a mensagem deve ser mais completa, contendo o motivo da alteração.

**OBS.:** o `body`de um type revert deve conter a hash do commit que esta sendo revertido.

## Footer
Deve conter qualquer informação sobre **Breaking Changes** e uma referência a possível *issue*, caso houver. **Breaking Changes** deve começar com o texto `BREAKING CHANGE:`.
