#Passo a passo de como linkar um projeto do DESKTOP com um repositório remoto no Github

Obs: se for Windows tem que baixar o Git Bash https://git-scm.com/downloads


##No Terminal (Git Bash p/ Windows)

- Navegue até a pasta do arquivo usando o comando ``cd``
 - Digite o comando ``git init``
 - Crie um novo repositório na sua conta do GitHub sem o arquivo README.md
 - Copie a URL do seu novo repositório e coloque no final do código abaixo
 ``
 git remote add origin URL
 ``
 - Digite o código acima no terminal (ou Bash)
 
 Agora deve aparecer (master) no final do path no terminal e o arquivo ``package.json`` deve ter sido criado na pasta.
 
 ###O link esta feito
 
 
 -Para adicionar os arquivos da pasta ao GitHub digite: ``git add .``
 (Para Windows deve aparecer a seguinte mensagem: 
 ``warning: LF will be replaced by CRLF in package.json.
The file will have its original line endings in your working directory``)

Agora os arquivos da pasta estão na area de "staging"

- Para "commitar" os arquivos digite: ``git commit -m "msg sobre o commit"``

- Para que os arquivos apareçam na ``branch`` no GitHub faça o push com o nome da branch que você quer (se ela não existir vai ser criada):
``git push origin nome_da_branch``
 
 - Para puxar arquivos do repositório para o computador use o pull:
 ``git pull origin nome_da_branch``
 
 -Extra 
 -
 ``git status`` mostra o status dos arquivos presentes na pasta.
 
 Se ela não estiver linkada com um repositório git aparecerá a seguinte mensagem:
 ``fatal: not a git repository (or any of the parent directories): .git``
