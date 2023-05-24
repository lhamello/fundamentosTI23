# fundamentosTI23
1) Como criar chaves SSH e publicar na máquina;
	1.criar uma pasta no seu computador
	2.abrir o git Bash e digitar os seguintes comandos:
		1.cd ~/.ssh/
		2.ls(para saber onde está o arquivo)
		3.ssh.keygen, ele vai pedir para voce escolher uma pasta para salvar a chave ssh, entao voce tem que digitar o nome da pasta e dar enter
		4.dar enter 2 vezes
		5.sua chave ssh foi criada
	3.ls
	4.cat "nome do arquivo" .pub (pegar a informaçao que está no arquivo e retorna a chave SSH que foi gerada)

2) Como adicionar a chave SSH pública no servidor do github;
	1.entrar nas settings/configuraçoes
	2.ir no "SSH and GPG keys"
	3.apertar em "New SSH key"
	4.dar um nome á sua chave
	5.colar a chave que voce criou 
	6.apertar em "Add SSH key" 

3) Como e onde criar o arquivo de config conforme demonstrado em aula;
	1.entar em arquivos
	2.entar no disco
	3.procurar a pasta usuários
	4.entrar na pasta com o nome de usuario do seu computador
	5.entrar na pasta ".ssh"
	6.abrir o arquivo "config"
	7.escrever:
		1. Host github.com
		User (nome do seu usuario no github)
		Hostname ssh.github.com
		PreferredAuthentications publickey
		IdentityFile ~/.ssh/(nome do seu usuario no github)
		Port 443
	
4) Clonar o projeto exemplo no link https://github.com/lhamello/fundamentosTI23
	1.entrar no seu github
	2.criar um novo repositorio
		1.apertar no "+"
		2.selecionar "New repository"
		3.dar um nome ao repositorio
		4. apertar em "Create repository"
	3.criar uma pasta com o mesmo nome do seu repositório 
	4.entrar no link 
	5.apertar em "<> Code"
	6.copiar a chave SSH
	7.abrir o git Bash dentro da pasta que voce criou
	8.colocar o seguinte comando:
		1.git clone (colar/escrever a chave SSH )
		2.aperte enter
5) Criar uma "branch" para edição do readme.md;
	1.abra o git bash e digite os seguintes comandos:
		1."git checkout -b (nome que voce quiser botar na sua nova branch)"
		2."git push --set-upstream origin (nome da sua branch)"
6) Editar o arquivo readme.md adicionando os passos anteriores;
	1.abrir a pasta clonada no terminal, e abra o arquivo "README"
	2.faça a alteraçao que quiser
	3.salve o arquivo
7) Realizar um pull-request solicitando integração ao projeto principal.
	1.no github, abrir os seus repositorios
	2.va no menu "Branch", escolha a branch que contém seus commits
	3.clique em "Solicitaçao de pull"
	4.use o menu do branch base para selecionar o branch no qual voce quer mesclar as alteraçoes e use o menu para escolher o branch do tópico em que voce fez as alteraçoes
	5.digite um titulo e uma descriçao para a pull request
