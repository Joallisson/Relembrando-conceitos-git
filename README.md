# Relembrando-conceitos-git
Relembrando alguns comandos git no terminal

- COMO INICIAR EM UMA PASTA, O VERSIONAMENTO GIT:
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

- EXIBIR HISTÓRICO DE COMMITS MAIS DETALHADO:
    git reflog
    
- EXIBIR HISTÓRICO DE COMMITS:
    git log
    
- EXIBIR AS BRANCH LOCAIS:
    git branch
    
- EXIBIR TODAS AS BRANCH:
    git branch -a
    
- PARA REVERTER O COMMIT ATUAL E VOLTAR PARA OUTRO: (quando executar git reflog a saida dever ser parecida com esse exemplo: < 9e3b52d HEAD@{2}: commit (initial): commit inicial > e o ID desse commit é o  9e3b52d)
    git reflog
    git reset --hard <ID do commit>
    
    
    
    
    
    
    
    
    
    
    
    
    
    
