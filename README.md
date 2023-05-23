1) Como criar chaves SSH e publicar na máquina;1//
criar a chave ssh
criar ou clonar um repositorio
criar uma chave ssh com o comando: ssh-keygen -t ed25519 -C "your_email@example.com"
Para criar uma chave rsa: executar: ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
Copiar chave pública com o comando: cat ~/.ssh/id_ed25519.pub
2) Como adicionar a chave SSH pública no servidor do github;
2//Abra o Github e vá no ícone de perfil > Settings, no canto superior direito.
Na barra lateral de configurações do usuário, clique em "SSH and GPG keys".
Clique no botão //New SSH key//
No campo //Título//, adicione um rótulo descritivo para a nova chave. Por exemplo, se estiver usando seu computador pessoal, você pode chamar essa chave de "Computador pessoal".
Cole a chave pública que está na área de transferência no campo //Chave//.
3) Como e onde criar o arquivo de config conforme demonstrado em aula;3//
criar arquivo chamado config na pasta ssh
configure o git com seus dados:

Host github.com
user //seu id git//
Hoste ssh.github.com
PreferredAutentications publikey
IdentityFile~/.ssh/id_ed25519
Port 443

4) Clonar o projeto exemplo no link https://github.com/lhamello/fundamentosTI23
clonado com sucesso: usse git clone + 0 //linkdo repositorio//
5) Criar uma "branch" para edição do readme.md;
va ate a pasto do repositorio no link git https://github.com/lhamello/fundamentosTI23 crie uma brancha
ou use o codgo checkout -b //nome da branch//
usse o comando git push --set-upstream origin //nome da branch//
6) Editar o arquivo readme.md adicionando os passos anteriores;
edite o arquio do repositorio
de git add e logo depois git commit
7) Realizar um pull-request solicitando integração ao projeto principal.
8) Faça o download do projeto usando as opções do github e anexe seu artefato (projeto aqui).
