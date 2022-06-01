# Relembrando-conceitos-git
Relembrando alguns comandos git no terminal

- COMO INICIAR EM UMA PASTA UM VERSIONAMENTO GIT:
    git init 

- COMO ADICIONAR SUA CONTA DO GITHUB NO REPOSITŔIO LOCAL DO GIT: (provavelmente no último passo vai pedir para colocar usuário e senha)
    git config --global user.email "emailexemplo@exemplo.com"
    git config --global user.name "exemplo nome"
    git remote add origin <coloque a url do seu projeto github aqui>

- COMO ADICIONAR TODOS OS ARQUIVOS E PASTAS PARA SEREM VERSIONADOS: (É necessário que o repositório já esteja criado dentro do github)
    git add .

- COMO CONECTAR MEU PROJETO AO MEU REPOSITÓRIO JÁ CRIADO NO GITHUB:
    git remote

- CRIAR UM COMMIT: 
    git add .
    git commit -m "escreva seu commit aqui"
  
- DAR O PRIMEIRO PUSH:
    git push --set-upstream origin master

- DAR UM PUSH:
    git push
