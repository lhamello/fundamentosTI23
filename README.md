# fundamentosTI23


PRIMEIRO PASSO:
criar uma chave ssh para add no git  (para criar a chave , é só colocar no google "criar chave ssh" , e depois copiar os codigos)


SEGUNDO PASSO:
criar um repositorio no github (clicar no +  , new repositors , e colocar um nome na pasta e criar)

TERCEIRO PASSO:
Adicionar a chave ssh depois de criada no git

vai em settings --> SSH and GPS keys --> new ssh key , e adiciona a chave la

QUARTO PASSO:
Criar uma pasta no seu computador , e em seguida clicar com o botão direito dentro da pasta , assim abrindo o terminal

QUINTO PASSO:
colocar os codigos um de cada vez , em sequencia no seu terminal
os seguintes codigos:

echo "#<NOME DE USUARIO DA SUA CONTA DO GIT>" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin git@github.com:<SEU NOME DE LOGIN>/<NOME DO REPOSITORIO>.git
git push -u origin main

SEXTO PASSO:
para criar uma branch , abrimos nossa pasta criada , apertamos com o botão direito , e abrimos nosso terminal, abrindo o terminal digitamos o seguinte codigo:
git checkout -b <um nome para sua branch>

SETIMO PASSO:
ainda no terminal , usamos o codigo: git add <nome da pasta>(por exemplo, README.md)

isso para sairmos da branch "main" , e entrar na nossa branch criada.

OITAVO PASSO: 
em seguida usamos o codigo: git commit -m <"um nome de sua escolha">

isso para subir o aqruivo.

NONO PASSO:
Ainda no terminal usamos o codigo: git push --set-upstream origin <nome da sua branch>

isso é para enviar o arquivo editado para o github.


DECIMO PASSO E ULTIMO: 

Ccaso feita alterações na sua pasta após feito as etapas a cima , use o codigo git add, em seguida o git commit e depois um git push , para atualizar as alterações feitas.