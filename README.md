# fundamentosTI23

# 1 Como criar chaves SSH e publicar na máquina;

Abra Git Bash.

Cole o texto abaixo, substituindo o endereço de e-mail da sua conta em GitHub.

$ ssh-keygen -t ed25519-sk -C "YOUR_EMAIL"
Observação: se houver uma falha no comando e você receber o erro invalid format ou feature not supported,, você poderá estar usando uma chave de segurança de hardware que não dá suporte ao algoritmo Ed25519. Insira o comando a seguir.

$ ssh-keygen -t ecdsa-sk -C "your_email@example.com"
Quando solicitado, toque no botão da sua chave de segurança de hardware.

Quando for solicitado a "Insira um arquivo para salvar a chave", pressione Enter para aceitar o local padrão do arquivo.

> Enter a file in which to save the key (/c/Users/YOU/.ssh/id_ed25519_sk):[Press enter]
Quando precisar digitar uma frase secreta, pressione ENTER.

> Enter passphrase (empty for no passphrase): [Digite uma senha]
> Enter same passphrase again: [Digite a senha criada, novamente]

Pronto, você definiu uma chave ssh para esse computador, agora é hora de sinalizar no sua página do Github que essa chave existe, no próximo passo.

Esse texto foi uma adaptação a partir dessa fonte:
Fonte: https://docs.github.com/pt/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent


# 2 Como adicionar a chave SSH pública no servidor do github;


Depois de adicionar uma nova chave SSH de autenticação à sua conta em GitHub.com, você poderá reconfigurar qualquer repositório local para usar o SSH.

Copie a chave pública SSH que criou no passo anterior para a sua área de transferência.
(Abra o arquivo .pub copie o conteúdo dentro dele e siga para a próxima etapa).

1. No canto superior direito de qualquer página, clique na foto do seu perfil e em **Configurações**.
Captura de tela do menu da conta do GitHub mostrando as opções para os usuários exibirem e editarem o perfil, o conteúdo e as configurações. Há um item de menu "Configurações" com o contorno em laranja escuro.
Na seção "Acesso" da barra lateral, clique em Chaves SSH e GPG.

Clique em Nova chave SSH ou Adicionar chave SSH.

No campo "Title" (Título), adicione uma etiqueta descritiva para a nova chave. Por exemplo, se estiver usando um laptop pessoal, você poderá chamar essa chave de "Laptop pessoal".

No campo "Chave", cole sua chave pública.

Clique em Adicionar chave SSH.

Se solicitado, confirme acesso à sua conta em GitHub.

Esse texto foi uma adaptação a partir dessa fonte:
Fonte: https://docs.github.com/pt/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account#adding-a-new-ssh-key-to-your-account


# 3 Como e onde criar o arquivo de config conforme demonstrado em aula;


Dentro da sua pasta .ssh, que deve estar dentro de C://USERS/Usuário/.ssh, abra um novo arquivo bloco de notas (txt) e edite-o com as configurações à seguir:

Host github.com
User “SEU-USER”
Hostname ssh.github.com
PreferredAuthentications publickey
IdentityFile ~/.ssh/id_ed25519.pub (APÓS IDENTITYFILE INSERIR O CAMINHO FICOU A CHAVE SSH)
Port 443

No bloco de notas com as suas configs definidas, salve o arquivo e no momento de salvar altere o tipo de arquivo de “Tipo documento de texto (*.txt)” para “Todos os arquivos (*.*)” e altere o nome para “config”.

Pronto, agora você tem um .config definido.

# 4 Clonar o projeto exemplo no link https://github.com/lhamello/fundamentosTI23

Acesse o link do projeto;
Clique no <code> indicado em verde;
Copie o código ssh ou http indicado;
Abra o Bash na sua pasta de projetos;
Digite "git clone LINK COPIADO";
Dê Enter;
Pronto, foi copiado para a sua pasta de projetos;

# 5 Criar uma "branch" para edição do readme.md;

No Bash dentro da pasta do projeto execute o seguinte comando:

git push --set-upstream origin NOME (dê um nome pra essa branch no lugar de NOME)

Pronto, sua branch está criada;

# 6 Editar o arquivo readme.md adicionando os passos anteriores;

No Github vá na página do repositório;
Clique em "branch" e escolha o que está com seus commits;
Acima da lista de arquivos, clique em solicitação de Pull;
Use o menu suspenso do branch base para selecionar o branch que desenha mesclar as alterações e use o menu do branch de comparação para escolher p branch do  tópico no qual fez as alterações;
Digite um título  e uma descrição pro pull request;

# 7 Realizar um pull-request solicitando integração ao projeto principal.

No github, navegue até a página principal do repositório. Abaixo do nome do repositório clique em Actions;
Na barra laterla esquerda clique no fluxo de trabalho que deseja ver;
Na lista de execuções de fluxo de trabalho, clique no nome de execução para ver o resumo da execução do fluxo de trabalho;
na seção "Artefatos" clique no arquivo que deseja baixar;

