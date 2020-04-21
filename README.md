# curso-git

CURSO DE GIT

### Comandos: 
`git init` - inicia um repositório <br>
`git remote add origin <link_repositorio>` - Faz o link entre o repositório local e o do GitHub <br>
`git add README.md` - Adiciona o arquivo readme do repositório <br>
`git status` - Mostra a estado atual do repositório <br>
    - "Untracked Files" - São arquivos que não estão sendo versionados <br>
    - "Changes to be commited" - Arquivos que estão commitados, alterações feitas localmente que já foram preparadas para           serem "versionadas" <br>
`git add <nome_arquivo>` - Prepara um arquivo ou todos (.) para serem commitados <br>
`git rm --cached <nome_arquivo>` - Remove o arquivo desse commit atual <br>
`git commit -m "comentario"` - Confirma o commit, e coloca o comentário sobre o que foi adicionado ou alterado <br>
`git restore <nome_arquivo>` - Descarta as alterações feitas naquele arquivo <br>
`git log` - Mostra todos os commits, o autor e o comentário feito <br>
  **Algumas Opções:** <br>
   - `-p` - Mostra todas as alterações de todos commits
   - `-p -2` - Mostra todas as alterações dos 2 últimos commits
   - `--stat` - Mostra as estatisticas de todos os commits. Exemplo: numero de alterações
   - `--pretty=oneline` - Mostra os commits resumindo em apenas uma linha
   - `--pretty=format: "%h - %an, %ar : %s" ` - Mostra os detalhes do commit no seguinte formato: `688ab35 - Arthur Ferreira,          30 minutes ago : primeiro commit`
   - `--since=2.days` - Mostra todos os commits de até 2 dias atrás
<br><br>
`git reset HEAD <nome_arquivo>` - Altera o status daquele arquivo para 'Untracked Files' <br>
`git branch` - Mostra todas as branchs do repositório e destaca a branch que está atualmente <br>
**Opções:** <br>
- `<nome_branch>` - Muda para a branch especificada
- `-b <nome_branch>` - Cria uma nova branch e já muda para ela
<br><br><br>
`git checkout <nome_branch>` - Muda de uma branch para a outra <br>
`git reset HEAD~<numero_commis>` - Volta a quantidades de commits especificadas <br>
**Opções:** <br>
- `—soft` - Volta os commits e mantém as alterações feitas nele, já preparadas para serem comutadas <br>
- `—hard` - Remove todas as alterações e commits feitos após o commit especificado <br>
<br><br>
`git merge <nome_branch>` - Pega o conteúdo da branch especificada e coloca junto ao conteúdo da branch atual <br>
