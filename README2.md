# Meu-primeiro-repo
## Sobre este README
**Repositório da Aula 10** — _DevOps I_ (Univertix 2026).
Contém anotações, comandos e experimentos da disciplina.

## Conteúdo
**Comandos GIT:**
git init	
git clone [url]	
git status	
git add [arquivo]	
git commit -m "mensagem"	
git branch	
git checkout -b [nome]	
git pull	
git push	
git merge [branch]

**Chave SSH:**
Gerar o par de chaves: Abra seu terminal e digite:
_ssh-keygen -t ed25519 -C "seu_email@exemplo.com"_
(Pressione Enter para aceitar o local padrão e opcionalmente adicione uma passphrase).

Adicionar ao agente SSH:
_eval "$(ssh-agent -s)"_
ssh-add ~/.ssh/id_ed25519

Copiar a chave pública:
_cat ~/.ssh/id_ed25519.pub_
(Copie todo o conteúdo exibido que começa com ssh-ed25519).

Adicionar ao serviço (GitHub/GitLab):

Vá em Settings > SSH and GPG keys.

Clique em New SSH Key, cole o conteúdo copiado e salve.

**Boas práticas de versionamento:**
Commits Atômicos: Faça commits pequenos que resolvam apenas uma tarefa ou funcionalidade por vez. Evite "megacommits" com mudanças em 20 arquivos diferentes.

Mensagens Descritivas: Use o padrão Imperativo (ex: "Adiciona funcionalidade de login" em vez de "Adicionei" ou "Adicionando").

Use .gitignore: Nunca suba arquivos sensíveis (credenciais, .env) ou arquivos temporários do ambiente (node_modules, pastas __pycache__, binários) para o repositório.

## Autor

Matheus Heringer Dutra | Turma DevOps I 2026
