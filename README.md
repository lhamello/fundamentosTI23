# fundamentosTI23

Passo 1:
Criar a chave SSH

Passo 2:
Cadastrar a chave no servidor do git

Passo 3:
Criar um repositorio no git

Passo 4:
Apos isso,adicionar a chave SSH criada no git

Passo 5:
Vai em settings - new ssh key e adicione sua chave criada

Passo 6:
Criar uma pasta dentro de "Arquivos"

Passo 7: 
Abir um terminal dentro dela 

Passo 8:
Colocar os seguintes codgos no seu terminal:
echo "#<NOME DE USUARIO DA SUA CONTA NO GIT>"
git init
git add README.md
git commit -m "first commit"
git remote add origin git@github.com:<SEU NOME DE LOGIN> & <NOME DO REPOSITORIO GIT>.git
git push -u origin main

Passo 9:
E para criar um branch: abrimos uma pasta criada, clicamos com o botão direito e abrimos o teminal,abrindo o terminal digitamos o codigo;
git checkout -b <o nome da sua branch>

Passo 10:
no terminal,usamos o codigo git add <nome da pasta>

pra sair da branch "main", e entrar na nossa branch criada

Passo 11:

Apos isso utilizamos  o codigo : git commit -m <um nome da sua escolha>

*para subir o arquivo*

Passo 12:
Ainda no terminal usamos o codigo: push --set-upstream origin <nome da sua branch>

Para enviar o arquivo editado para o git

Passo 13:
Caso feita alteraçoes na sua pasta apos feito as etapas a cima , use o codigo git add e em seguida o git commit e depois um git push, para atualizar as alteaçoes feitas

.












 

