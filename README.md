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
para criar uma branch , abrimos nossa pasta 
