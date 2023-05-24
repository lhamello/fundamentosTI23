# fundamentosTI23
Crie um tutorial usando o github de como utilizar o git  para desenvolver um projeto para isso é necessário que este documento contenha:

1) Como criar chaves SSH e publicar na máquina;
Passo 1: Abrir o terminal GIT Bash;

Passo 2: Digitar o comando "cd ~/.ssh/";

Passo 3: Digitar o comando "ssh-keygen" e apertar no enter, e em seguida digitar 
o nome da sua chave e apertar enter novamente;  

Passo 4: Em seguida o programa irá pedir para você cadastrar uma chave, caso você queira 
cadastrar uma senha para aquela chave basta digitar a senha e apertar enter, 
caso não queira por uma senha, basta apenas apertar enter duas vezes;   

Passo 5: Após ter criado a chave voce deve digitar o comando "cat<nome da chave>.pub"
 com o nome da chave que voce criou para poder gerar o arquivo que será colado no Github.

Observação: Se voce esquecer o nome da chave, basta você digitar o comando "ls" para mostrar 
todas as chaves cadastradas na sua maquina;


2) Como adicionar a chave SSH pública no servidor do github;

Passo 1: O próximo passo é entrar na sua conta no github(caso você não tenha uma conta, 
será necessário criar uma em github.com),
 
Passo 2: Ir em configurações e ir na opção "SSH and GPG keys" e clicar em "New SSH key"  

Passo 3: Vá no git, copie a chave gerada pelo programa e cole no Github;

passo 4: Feito isso, basta nomear a chave SSH gerada e concluir a criação da chave;



3) Como e onde criar o arquivo de config conforme demonstrado em aula;

Passo 1: Para esse processo, você deve procurar no seu computador a pasta ".ssh" e 
abra a mesma;

Passo 2: Com a pasta aberta, abra o arquivo "config" que está dentro dela com o bloco de notas;

Passo 3: Dentro do arquivo, você encontrará algo semelhante a isso:

Host github.com
User Phill375
Hostname ssh.github.com
PreferredAuthentications publickey
IdentityFile ~/.ssh/id_ed25519
Port 443

Passo 4: Troque o item "IdentityFile ~/.ssh/id_ed25519" ou semelhante por 
"IdentityFile ~/.ssh/<seu nome de usuário>"

Passo 4: Feito todos esses passos, salve o arquivo;



4) Clonar o projeto exemplo no link https://github.com/lhamello/fundamentosTI23

Passo 1: No GitHub.com, navegue até a página principal do repositório.

Passo 2: Acima da lista de arquivos, clique em  Código.

Passo 3: Copie a URL do repositório.

**** Para clonar o repositório usando HTTPS, em "HTTPS", e copie o URL.

**** Para clonar o repositório usando uma chave SSH, clique em SSH e copie o URL .

**** Para clonar um repositório usando a GitHub CLI, clique em GitHub CLI e copie o URL.

Passo 4: no terminal, digite "git clone" e cole o URL copiado no GitHub;
$ git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY

Passo 5: Pressione enter para criar seu clone local.

$ git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY
> Cloning into `Spoon-Knife`...
> remote: Counting objects: 10, done.
> remote: Compressing objects: 100% (8/8), done.
> remove: Total 10 (delta 1), reused 10 (delta 1)
> Unpacking objects: 100% (10/10), done.


5) Criar uma "branch" para edição do readme.md;

CRIANDO NO GITHUB:

Passo 1: No GitHub.com, navegue até a página principal do repositório. 1. Acima da lista de arquivos, clique em  Branches.

Passo 2: Clique em Novo branch;

Passo 3: Em "Nome do branch", digite um nome para o branch;

Passo 4: Em "Origem do branch", escolha uma origem para o branch;

Observação:Se o repositório for um fork, selecione o menu suspenso do repositório 
e clique no fork ou no repositório upstream.

Passo 5: Selecione o menu suspenso do branch e clique em um branch.

Passo 6: Clique em Criar branch.

CRIANDO NO TERMINAL:

Passo 1: Abra o terminal com o repositorio clonado;

Passo 2: Digite "git checkout -b" e depois do "b" digite o nome que você quer que tenha a branch e aperte enter;

Passo 3: Após isso digite "git push --set-upstream origin Phill";

Passo 4: Digite a senha solicitada e aperte em enter.



6) Editar o arquivo readme.md adicionando os passos anteriores;

Passo 1: Abra a pasta clonada no terminal e em seguida abra o arquivo README.md com o bloco de notas;

Passo 2: Faça as alterações que você quer;

Passo 3: Salve o arquivo.



7) Realizar um pull-request solicitando integração ao projeto principal.

Passo 1: Abra o repositorio no Github;

Passo 2: clique em "Pull requests" e em seguida clique em "New Pull requests"

8) Faça o download do projeto usando as opções do github e anexe seu artefato (projeto aqui).
