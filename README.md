# fundamentosTI23
Para confugurar o git .
$ git config --global user.name "Seu Nome"
$ git config --global user.email voce@exemplo.com
1 - Pra criar uma chave é necessário fazer o comando $ ssh-keygen -t ed25519 -C "seu_email@example.com"
substituindo o e-mail pelo o seu.
Vai criar uma nova chave SSH, usando o seu e-mail como uma etiqueta.
2- Para adicionar um chave no Github precisamos:
Abrir o Github e ir no ícone de perfil - configurações , no canto superior.
Na barra lateral de configurações do usuário, clicar em "Chaves SSH".
Clique em "Nova chave SSH"
Na parte "Título", adicione um rótulo para a nova chave. 
Cole a chave pública que está na área de download no campo "Chave".
Clique em "Adicionar chave SSH".
3-O arquivo confg deve ser criado dentro do disco,C em usuários,em Técnico TI , dentro da pasta .ssh , não pode ser um aquivo dentro de outra pasta sem extensoes,
 criando um documento de texto com o conteúdo: 
Host github.com
User TharsilaMS (aqui com o seu nome de usuário do Github.)
Hostname ssh.github.com
PreferredAuthentications publickey
IdentityFile ~/.ssh/id_ed25519
Port 443
4-Para clonar usamos o comando "git clone mais a chave SSH" do arquivo que queremos clonar.
5- Pra criar uma branch devemos usar o código git checkout -b e o nome da nova branch.

