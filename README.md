# Processo para criação de chave SSH no GitHub
# é preciso ter o GitBash instalado na maquina e uma conta logada no github

1- crie uma pasta onde ficara salvo seus projetos do git

2- entre na pasta, clique com o direito do mouse e clique em "Git Bash HERE"
   após isso abrira o console do gitbash

3-Digite o codigo "cd ~/.ssh/" e em seguida o codigo "ls" que sera lista todas as chaves ja cadastradas

4- digite "ssh-keygen", em seguida o console ira pedir para digitar o nome da sua chave
Exemplo: Enter file in which to save the key (/home/vitor/.ssh/id_rsa): "digite o nome da chave"

5-logo em seguida sera necessario digitar uma senha para a sua chave e confirmala pela segunda vez

6- logo em seguida voce pode digitar o comando "ls" para conferir se sua chave foi criada

7- com o comando "cat + nome da chave.pub" voce tera acesso a chave publica

8- em seguida vamos ao github, aba "configurações" depois em "SSH and GPG keys".

9- em seguida na opção "new SSH key"

10- de um nome a sua chave novamente, e em seguida cole a chave publica do seu gitbash

11- em seguida voltamos no console do gitbash e usamos o comando "ssh-add (nome da sua chave)

12- apos isso vamos no diretorio "C:\Users\Tecnico - TI\.ssh" lá contem todas suas chaves .ssh e um arquivo chamado "config"

13- abra o arquivo "config" com o bloco de notas, ele deve conter as seguintes informações :
Host github.com
User (nome da sua chave)
Hostname ssh.github.com
PreferredAuthentications publickey
IdentityFile ~/.ssh/(nome da sua chave)
Port 443

exemplo:

Host github.com
User VitorAlicer
Hostname ssh.github.com
PreferredAuthentications publickey
IdentityFile ~/.ssh/VitorAlicer
Port 443

# Como clonar um projeto do github

1- acesse no github o projeto a ser clonado
2- em seguida va em "Codigo" apos em "SSH" e copie o codigo
3- entre na pasta aonde ficara salvo os projetos, clique com o direito do mouse e em seguida "Git Bash HERE"
4- apos abrir o console digite o comando "Git clone (e a chave ssh retirada do github)"
5- depois disso o programa ira criar o clone do projeto

# Criar uma "branch" para edição do readme.md;

1- No Github, navegue até a página principal do repositório. Acima da lista de arquivos clique em  Branches
2- Clique em Novo branch
3- apos isso, digite um nome para o branch
4- Em "Origem do branch", escolha uma origem para o branch.
   Se o repositório for um fork, selecione o menu suspenso do repositório e clique no fork ou no repositório upstream.
5- Clique em Criar branch.

# Realizar um pull-request solicitando integração ao projeto principal.
1- No GitHub, vá até a página principal do repositório
2- No menu "Branch", escolha o branch que contém seus commits
3- Acima da lista de arquivos, clique em  Solicitação de pull
4- Use o menu suspenso do branch base para selecionar o branch no qual deseja mesclar as alterações e use o menu suspenso do branch de comparação para escolher o branch do tópico no qual você fez as alterações
5- Digite um título e uma descrição para a pull request

# Faça o download do projeto usando as opções do github e anexe seu artefato (projeto aqui).
1- No Github, navegue até a página principal do repositório. Abaixo do nome do repositório, clique em  Actions
2- Na barra lateral esquerda, clique no fluxo de trabalho que deseja ver
3- Na lista de execuções de fluxo de trabalho, clique no nome da execução para ver o resumo da execução do fluxo de trabalho
4- Na seção "Artefatos", clique no artefato que deseja baixar