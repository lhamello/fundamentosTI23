# fundamentosTI23
# fundamentosTI23
Passo1

criar uma chave ssh para add no git (para criar a chave ,é so botar "Criar chave ssh" , e depois copiar os codigos)

Passo2

Criar um repositorio no github (Clicar no + , new repositorio, e colocar o nome na pasta)

passo3

Adiconar a chave ssh após de ser criada no git
Vai em settings -- >new ssh key, e adiciona a chave

passo4

Criar uma pasta em seu computador, depois clicar com o botão direito do mouse dentro da pasta,assim abrindo o terminal

Passo5

Colocar os codigos um de cada vez,em sequencia no seu terminal
os seguintes codigos:

echo "#<nome teu usuario da sua conta do git>" >> README.md
git init
git add README.md
git commit menos m "first commit"
git remote add origin git@hub.com:<TEU NOME DE LOGIN >/<Nome do repositorio> . git
git push - u origin main

Passo6

Para criar uma branch,abra a pasta criada,aperte com botão direito,abre o terminal digite o seguinte codigo
git checkout -b <o nome para a sua branch>

Passo7

ainda no terminal, use o codigo:git add <nome da pasta> (Ex,README.md)
isso para sair da branch"main",entrar em sua branch criada.

Passo8
em seguida usar o codigo:git commit - m <"o nome escolhido">
isso para subir o arquivo

Passo9

No terminal use o codigo: git push --set-upstrean origin<nome de sua branch>
isto é feito para enviar o arquivo editado para o github.

Passo10

(Caso feita alguma alteração na sua pasta após feito as etapas anterior,use o codigo git add, em seguida o git commit e depois e depois o git push, para atualizar as alterações feitas)