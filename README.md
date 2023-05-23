# fundamentosTI23

1) Como criar chaves SSH e publicar na máquina;

Para criar uma chave SSH é necessário seguir uma sequência de comandos utilizando git.

O primeiro passo que deve realizar é acessar a pasta onde se encontram todas as chaves SSH existentes.
para fazer isso precisa abrir o terminal e acessar a pasta através dos comandos:

cd ~/.ssh/
(acessa a pasta das chaves SSH)

ssh-keygen
(inicializa o processo de gerar a chave)
(perguntará qual nome gostaria de usar para identificar a chave)
(perguntará qual senha gostaria de definir, caso não queira senha, prossiga com enter)

digite ls para verificar se a chave foi gerada.

digite cat nomedasuachave.pub
(a chave pública terá a extensão .pub)

2) Como adicionar a chave SSH pública no servidor do github;

Após ter gerado sua chave SSH, acesse o link do github referente as chaves SSH.

https://github.com/settings/keys

vá em (New SSH key) green button.
defina um nome de identificação da chave em (Title).
No campo (Key) você deverá inserir a chave do tipo pública gerada anteriormente.


3) Como e onde criar o arquivo de config conforme demonstrado em aula;

o arquivo config deverá estar dentro da pasta .ssh


4) Clonar o projeto exemplo no link https://github.com/lhamello/fundamentosTI23




5) Criar uma "branch" para edição do readme.md;

6) Editar o arquivo readme.md adicionando os passos anteriores;

7) Realizar um pull-request solicitando integração ao projeto principal.

8) Faça o download do projeto usando as opções do github e anexe seu artefato (projeto aqui).
