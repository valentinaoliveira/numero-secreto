# Guia de Comandos Git e Boas Práticas

## 📌 Comandos Essenciais do Git

- `git init`: Inicializa um repositório Git na pasta atual.
- `git add <arquivo>`: Adiciona um arquivo novo ou modificado ao stage.
- `git add .`: Adiciona **todos** os arquivos modificados ao stage.
- `git commit -m "mensagem"`: Cria um commit com uma mensagem descritiva.
- `git branch -M main`: Renomeia a branch atual para `main`.
- `git remote add origin <url>`: Conecta o repositório local a um repositório remoto.
- `git push -u origin main`: Envia seus commits locais para o repositório remoto.
- `git remote`: Lista os repositórios remotos configurados.
- `git pull`: Baixa as alterações do repositório remoto para o local.
- `git log`: Mostra o histórico de commits com autor e mensagem.
- `git clone <url>`: Clona um repositório remoto para sua máquina.
- `git status`: Mostra o estado atual dos arquivos (modificados, adicionados, etc.).
- `git branch`: Lista todas as branches do repositório.
- `git checkout -b <nova-branch>`: Cria e troca para uma nova branch.
- `git checkout <branch>`: Alterna para a branch especificada.
- `git merge <branch>`: Mescla a branch especificada na branch atual.
- `git rebase <branch>`: Move os commits da branch atual para a frente dos commits da branch especificada.
- `git stash`: Guarda temporariamente as alterações sem commit.
- `git stash pop`: Recupera as alterações salvas com `stash`.
- `git reset --hard HEAD~1`: Remove o último commit (⚠️ irreversível!).
- `git revert <commit>`: Reverte um commit específico sem remover histórico.
- `git tag -a v1.0 -m "Versão 1.0"`: Cria uma tag anotada.
- `git push origin --tags`: Envia as tags para o repositório remoto.

---

## 👥 Adicionar Colaboradores

1. Acesse o repositório no GitHub.
2. Vá em **Settings**.
3. No menu à esquerda, selecione **Collaborators**.
4. Clique em **Add people** e insira o nome de usuário GitHub da pessoa.
5. Aperte o botão **Add <user> to this repository**.
6. O colaborador receberá um convite por e-mail e, após aceitar, terá acesso ao repositório.

### ✅ Commit com vários autores

Se várias pessoas contribuíram para uma modificação, adicione co-autores ao commit:

```bash
$ git commit -m "Adicionar nova funcionalidade."
>
>
Co-authored-by: Nome <nome@email.com>
Co-authored-by: Outro-Nome <outro@email.com>
```

---

## 🔧 Lidando com Conflitos

Se houver conflitos ao fazer `git pull` ou `git merge`, siga estes passos:

1. O Git mostrará quais arquivos têm conflitos.
2. Abra o arquivo e procure algo assim:

   ```bash
   <<<<<<< HEAD
   (Seu código)
   =======
   (Código do repositório remoto)
   >>>>>>> branch-remota
   ```

3. Edite o arquivo, resolvendo o conflito (escolha ou misture as partes).
4. Após resolver:
   ```bash
   git add <arquivo>
   git commit -m "Resolver conflito no arquivo X"
   git push
   ```

---

## 🛠️ Boas Práticas

- **Mantenha mensagens de commit curtas e claras.**
- **Use verbos no infinitivo** (Exemplo: "Adicionar funcionalidade", "Corrigir erro").
- **Evite detalhes técnicos complicados nas mensagens de commit.**
- **Crie branches para cada funcionalidade ou correção.**
- **Faça commits pequenos e frequentes para facilitar o rastreamento.**
- **Sempre faça `git pull` antes de iniciar mudanças para evitar conflitos.**

---

## 🔥 VS Code e Git

No VS Code, ao alterar ou adicionar arquivos, ele exibe ícones ao lado dos arquivos:

- **M:** Modified (modificado)
- **U:** Untracked (não rastreado)

Assim, fica mais fácil ver o que foi alterado antes de fazer o commit.

---

Agora seu fluxo de trabalho com Git tá mais organizado e profissional! 🚀

