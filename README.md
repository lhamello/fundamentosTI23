1) Como criar chaves SSH e publicar na máquina;1//
criar a chave ssh
criar ou clonar um repositorio
criar uma chave ssh com o comando: ssh-keygen -t ed25519 -C "your_email@example.com"
Para criar uma chave rsa: executar: ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
Copiar chave pública com o comando: cat ~/.ssh/id_ed25519.pub
2) Como adicionar a chave SSH pública no servidor do github;
2//Abra o Github e vá no ícone de perfil > Settings, no canto superior direito.
Na barra lateral de configurações do usuário, clique em "SSH and GPG keys".
Clique no botão "New SSH key"
No campo "Título", adicione um rótulo descritivo para a nova chave. Por exemplo, se estiver usando seu computador pessoal, você pode chamar essa chave de "Computador pessoal".
Cole a chave pública que está na área de transferência no campo "Chave".
3) Como e onde criar o arquivo de config conforme demonstrado em aula;3//
criar arquivo chamado config na pasta ssh
configure o git com seus dados


