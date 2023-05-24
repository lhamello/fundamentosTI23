# fundamentosTI23
1) Como criar chaves SSH e publicar na máquina;
-Precisamos utilizar o Git Bash.
-Depois digitamos o comando "cd~/.ssh/".
- Para criarmos uma chave SSH , precisaremos usar o comando "ssh- keygen" e usar o Enter.
-Após o comando, será perguntado o nome que o usuario gostaria de utilizar para a chave.
-Caso ja possua uma chave, o usuario pode usar o comando "ls" para ver todas as chaves existentes.
- Depois desse processo, se voce quiser, voce poderá escolher uma senha de segurança. Se não quiser, é so utilizar o Enter 2 vezes que a senha não sera criada.
-Com isso a sua chave sera criada.  
-Após a criação da chave, utilize o comando "cat<"nome da chave escolhida">.pub", para gerar o arquivo que irá para o Github.
2) Como adicionar a chave SSH pública no servidor do github;
-Será preciso criar uma conta (ou ja possuir uma) no Github.
-É necessario ir nas configurações e clicar na opção "SSH and GPG keys" e depois selecionar a opção "New SSH key"
-Após isso, volte ao Git Bash, copie a chave gerada, e cole no Github. Também precisará nomear essa nova chave para concluir a criação.
3) Como e onde criar o arquivo de config conforme demonstrado em aula;
- É necessario encontrar a pasta ".ssh" e abrir ela.
-Após abrir, clique no arquivo "config".
-Dentro do arquivo estarão essas informações:
Host github.com
User: "o seu usuario"
Hostname ssh.github.com
PreferredAuthentications publickey
IdentityFile ~/ssh/id_ed25519
Port 443
-Apos isso, voce deve modificar o "IdentityFile" e colocar:
IdentityFile ~/ssh/"nome do usuario no github".
4) Clonar o projeto exemplo no link https://github.com/lhamello/fundamentosTI23
- É necessário entrar no link do Github.
- Após isso voce clicará na opção "code" e copiará o SSH do repositorio.
- Depois de copiar, voce usara o comando "git clone" e sera necessario colar o SSH para começar o processo de cópia.
5) Criar uma "branch" para edição do readme.md;
-No Git Bash, voce tera que utilizar o comando ("git checkout -b" +"nome" que voce precisara digitar) e com isso mudará o seu "main".
6) Editar o arquivo readme.md adicionando os passos anteriores;
-Abrir a pasta clonada pelo terminal e abrir o README.md pelo bloco de notas.
-Após faça as alterações que deseja.
-Salve o arquivo.
7) Realizar um pull-request solicitando integração ao projeto principal.
-Abrir o repositorio no Github.
-Ir na opção pull-request e depois selecionar a opção new pull request.
