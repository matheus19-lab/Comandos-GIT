# Git Commands Roadmap 🛣️

Um guia completo para iniciantes e usuários intermediários do Git, organizado por etapas do fluxo de trabalho.

---

## 1. Configuração Inicial
Antes de começar a usar o Git, configure seu usuário:
```bash
git config --global user.name "SeuNome"    # Define seu nome
git config --global user.email "seuemail@exemplo.com"  # Define seu e-mail
git config --list                           # Verifica configurações

git init                     # Cria um repositório Git local
git clone <url-do-repositorio> # Clona um repositório remoto


git branch                   # Lista branches locais
git branch <nome-da-branch>  # Cria uma nova branch
git switch <nome-da-branch>  # Muda para a branch
git switch -c <nome-da-branch> # Cria e muda para uma branch
git branch -d <nome-da-branch>   # Deleta branch local
git push origin --delete <nome-da-branch> # Deleta branch remota


git status                    # Verifica o estado dos arquivos
git add <arquivo-ou-pasta>    # Adiciona arquivos ao próximo commit
git add .                      # Adiciona todos os arquivos
git commit -m "Mensagem do commit" # Cria um commit
git commit -am "Mensagem"     # Atalho: adiciona arquivos rastreados e commita


git fetch                     # Baixa alterações do remoto sem aplicar
git pull                      # Baixa e aplica alterações do remoto



git push origin <nome-da-branch>      # Envia commits locais
git push -u origin <nome-da-branch>   # Push e define branch remota padrão


git merge <outra-branch>       # Mescla outra branch na atual
git rebase <outra-branch>      # Reaplica commits em cima de outra branch


# Editar arquivos manualmente para resolver conflitos
git add <arquivo-resolvido>    # Marca como resolvido
git commit                     # Finaliza o merge ou rebase


git log                         # Mostra histórico de commits
git log --oneline               # Histórico resumido
git diff                        # Mostra diferenças não commitadas
git show <commit>               # Mostra detalhes de um commit específico
git remote -v                   # Mostra URLs remotas


git rm <arquivo>                # Remove arquivo do Git e do disco
git mv <arquivo> <novo-nome>    # Renomeia ou move arquivo
git clean -f                    # Remove arquivos não rastreados
git tag <nome-tag>              # Cria uma tag
git tag -d <nome-tag>           # Deleta uma tag local
git push origin <nome-tag>      # Envia tag para remoto
