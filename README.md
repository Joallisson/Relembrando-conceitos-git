# Relembrando-conceitos-git 
Relembrando alguns comandos git no terminal

- COMO INICIAR EM UMA PASTA, O VERSIONAMENTO GIT: <br />
    git init 
    
- VER O STATUS DO VERIONAMENTO: <br />
    git status

- COMO ADICIONAR SUA CONTA DO GITHUB NO REPOSITŔIO LOCAL DO GIT: (provavelmente no último passo vai pedir para colocar usuário e senha) <br />
    git config --global user.email "emailexemplo@exemplo.com" <br />
    git config --global user.name "exemplo nome" <br />
    git remote add origin < coloque a url do seu projeto github aqui > <br />

- COMO ADICIONAR TODOS OS ARQUIVOS E PASTAS PARA SEREM VERSIONADOS: (É necessário que o repositório já esteja criado dentro do github) <br />
    git add .

- COMO CONECTAR MEU PROJETO LOCAL AO MEU REPOSITÓRIO JÁ CRIADO NO GITHUB: <br />
    git remote add origin < url do meu repositorio no github > <br />

- COMO BAIXAR UMA BRANCH REMOTO PARA O REPOSITORIO LOCAL: <br />
    git checkout -b <nome-do-seu-branch-local> origin/<nome-do-branch-remoto>

- CRIAR UM COMMIT: <br />
    git add . <br />
    git commit -m "escreva seu commit aqui"
  
- DAR O PRIMEIRO PUSH: <br />
    git push --set-upstream origin main

- DAR UM PUSH: <br />
    git push

- DESFFAZER ULTIMO MERGE: <br />
    git reset --hard HEAD~1

- EXIBIR HISTÓRICO DE COMMITS MAIS DETALHADO: <br />
    git reflog
    
- EXIBIR HISTÓRICO DE COMMITS: <br /> 
    git log
    
- PARA REVERTER O COMMIT ATUAL E VOLTAR PARA OUTRO: (quando executar git reflog a saida dever ser parecida com esse exemplo: < 9e3b52d HEAD@{2}: commit (initial): commit inicial > e o ID desse commit é o  9e3b52d) > <br />
    git reflog <br />
    git reset --hard < ID do commit >
    
- EXIBIR AS BRANCH LOCAIS: <br />
    git branch
    
- EXIBIR TODAS AS BRANCH: <br />
    git branch -a
    
- PARA CRIAR NOVAS BRANCH: <br />
    git branch staging

- PARA MUDAR DE BRANCH: <br />
    git checkout staging
    
- SEMPRE QUE MUDAR DE BRANCH E EU FIZER UM COMMIT E UM PUSH TENHO QUE EXECUTAR: (no código abaixo < staging > é o nome da nova branch) <br />
    git push --set-upstream origin staging

- FAZENDO ATUALIZAÇÃO DOS ARQUIVOS DO GITHUB PARA O REPOSITÓRIO LOCAL GIT: <br />
    git pull
    
- UNIR DUAS BRANCH (FAZER UM MERGE), NO CASO VOU ENTRAR NA BRANCH MASTER E PUXAR AS ATUALIZAÇÕES QUE FORAM FEITAS NA BRANCH STAGING: (antes de fazer o   merge, é necessário fazer o git pull na branch master para ter certeza que é o código mais atualizado) <br />
    git checkout  master <br />
    git merge staging
    
- CRIAR UMA BRANCH E IR DIRETO PRA ELA: (nesse é exemplo estou criando uma branch chamda < sistema-de-login >  entrando nela) <br />
    git checkout -b sistema-de-login
    
- PARA RESTAURAR ARQUIVOS DELETADOS: <br />
    git restore "digite nome do arquivo.extensão do arquivo por exemplo: teste.txt "

- PARA NÃO VERSIONAR ARQUIVOS QUE SENSIVEIS COMO SENHAS: <br />
    touch .gitignore

- RENOMEAR UMA BRANCH LOCAL NO GIT: <br />
    git branch -m < novonome >
    
- RESOLVER PROBLEMA "fatal: refusing to merge unrelated histories": <br />
    git pull origin < nomeDaBranchLocal > --allow-unrelated-histories
    
- ENVIAR NOME NOVO DA BRANCH PRO GITHUB: <br />
    git push origin -u < novonome >

- DESFAZER MERGE: <br />
    git reset --hard HEAD~1

- EXCLUIR UMA BRANCH NO LOCAL <br />
    git branch -d < nomeDoBranchLocal >

- EXCLUIR UMA BRANCH NO REMOTO <br />
    git push origin --delete < nomeDoBranchRemoto >
    
- APAGAR O "REMOTE ORIGIN" DA BRANCH LOCAL
    git remote remove origin
