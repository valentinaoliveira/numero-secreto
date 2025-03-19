git init: Inicializar o repositório
git add: Adicionar o arquivo alterado/novo no repositório
git add .: Adicionar tudo no repositório
git commit -m "": Adicionar comentário no que foi adicionado
git brach -M main: renomeia sua branch atual para main
git remote add origin <url>: Adicionar os arquivos local no remoto em um novo repositório
git push -u origin main: Enviar commit do local para o remoto
git remote: Listar os repositórios que tem no terminal
git pull: Baixar commits do repositório remoto para o local
git log: Listagem dos commits feitos e quem os fez
git clone <url>: clonar o repositório remoto de outra pessoa
git status: verificar quais arquivos foram modificados
 

Adicionar colaboradores: 
Entrar no gitHub (no repositório criado)
Ir em "Settings" (configuração)
Procurar "Collaborators" no menu à esquerda
Clicar em "Add people" colocando o userName da pessoa que você quer adicionar como colaborador 
Apertar no botão "Add <user> to this repository
A pessoa que foi convidada vai receber um e-mail com o convite, basta ela clicar no "view invitation" e aceitar que estará tendo acesso ao repositório. Ela consiguira fazer mudanças no codigo esubir para o repositório sem problema agora. 
Caso queira adicionar mais de um autor no commit é só preciso dar 
$ git commit -m "Adicionar nova funcionalidade.
>
>
Co-authored-by: NOME <nome@email.com>
Co-authored-by: OUTRO-NOME <outro@email.com>"



Boas práticas: 
-Mantenha a mensagem curta e concisa
-Uso de verbo no infinitivo
-Evite detalhes técnicos

Vs Code : adicionar ou alterar algum arquivo aparece uma sinalização ao lado do nome desses arquivos
-M: Modified, do português modificado.
-U: Untracked, do português não rastreado