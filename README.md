# Curso iniciante em programação da Alura - Git e GitHub 

<img src="Git e GitHub.jpg">

Link do curso: <a href="https://cursos.alura.com.br/course/git-github-controle-de-versao">Curso de Git e Github: Controle e compartilhe seu código</a><br>
# Sistemas de controle de versões  

<strong>Git Bash</strong> Fornece comandos do Linux<br>
<strong>On branch master</strong> Ramo ou branch<br>
<strong>Changes to committed</strong> Mudanças a serem commitadas<br>
<strong>HEAD</strong> Estado atual do nosso código, onde o Git os colocou.<br>
<strong>Working tree</strong> Local onde os arquivos estão sendo editados.<br>
<strong>index</strong> Local onde o git armazena o que será commitado ou local entre a working tree e o repositório Git em si.<br>
<strong>hash do commit</strong> Uma identificação única de cada commit<br>
<strong>.gitignore</strong> Arquivo criado na mesma pasta do projeto, em que ignora os arquivos ou pastas nos commits. Para isso, coloca-se o nome do arquivo ou pasta + uma barra no final dentro do <strong>.gitignore</strong><br>
<strong>(fetch)</strong> Busca<br>
<strong>(puch)</strong> Enviar<br> 
<strong>(pull)</strong> Puchar<br>

`ls` Mostra todas as pastas e arquivos<br>
`git --version` Diz a versão do Git<br>
`git config --local user.name "Seu nome aqui"` Nome do autor que irá fazer as alterações no arquivos nesse projeto<br>
`git config --local user.email "seu@email.aqui"` Email do autor que irá fazer as alterações no arquivos nesse projeto<br>
`git init` Transforma a pasta atual em repositório<br>
OBS: Caso o caminho da sua pasta possua espaços, é preciso colocá-lo entre aspas. Exemplo: `cd 'Documents/Curso Git e GitHub'`<br>
`git config --list --local` Confere<br> 
`git status` Mostra o estado do repositório ou quais arquivos foram alterados<br>
`git add + <Nome do arquivo>` Adciona 1 arquivo específico no Git ou inclui arquivos no commits, que passa a monitorar.<br>
`git add .` ou `git add -A` Adciona todos os arquivos no Git<br>
`git commit -m "nome da alteração + detalhes se quiser"` (commit) Salva a alteração recente e indica mudanças como um <strong>"check point"</strong><br>
`git rm` Remove o arquivo recém adcionado deixando de ser monitorado.<br>
`git log` Vê o histórico de alterações.<br>
`git config --local user.name "nome alterado"` Configuração para cada projeto<br>
`git config --global` Para máquina toda ou para todos os projetos<br>
`git config user.email` Visualisa as configurações de email<br>
`git config user.name` Visualisa as configurações do nome<br>
`git log --oneline` Visualisa as alterações resumida em uma única linha<br>
`git log -p` Visualisa as alterações detalhada, inclusive códigos ou escrita que era antes e mostra como ficou depois<br>
`git log --pretty="format:%H"` Comando que nos traz apenas o hash<br>
`git log --pretty="format:%h %s"` Traz o hash resumido seguido pela mensagem do commit<br>
`git log --help` Exibe página manual de git-log<br>
`cd ..` Volta uma pasta acima da pasta do projeto<br>
`mkdir + <Nome da pasta>` Cria uma pasta<br>
`cd + <Nome da pasta/>` Acessa a pasta<br>
`git init --bare` Para transformar o repositório em servidor onde fica somente as alterações dos arquivos e não uma cópia de cada. `--bare` Parâmetro<br>
`git remote` Lista todos os repositórios remotos<br>
`git remote add + <Nome do repositório remoto> + <Caminho da pasta com os arquivos>` (ex: local). Pode ser uma url, um endereço na rede ou uma pasta no computador e etc...<br>
`git remote -v` Mostra o endereço do local<br>
`rm -rf + <nome da pasta>` Remove pasta ou diretório do Git(flag `-rf` para remover tudo dentro de uma pasta)<br>
`rm -rf .git` Excluir repositório do Git<br>
`ls -lah` Verificar se o repositório está oculto<br>
`git clone + <local do disco ex: /c/ ou /d/ e etc.> + <endereço do servidor remoto> + <1 espaço> + <nome do projeto>` Trazer pela primeira vez um repositório remoto para a sua máquina (Clonar).<br>
`git push <nome do repositório remoto(local)> + <a branch (master)>` Ex: `git push local master`<br>
`git remote rename origin local` Renomeia repositório remoto local (<strong>origin</strong> nome do repositório local atual)<br>
`git pull local master` Trazer os dados de um repositório remoto para o meu (OBS: <strong>local</strong> outro repositório remoto), (<strong>master</strong> branch).<br>
`git remote add + <nome repositório(origin)> + <link do repositório(https) criado no GitHub>` Linka repositório remoto com o <strong>GitHub</strong><br>
`git push -u + <nome repositório(origin)> + <master>` Sempre que der um <strong>push</strong> nesse repositório <strong>master</strong> ele será adcionado no repositório remoto adcionado(origin).<br>
`git push + <nome repositório(origin)> + <master>` Empurra a versão atualizada para o GitHub<br>
`git push local main` Envia as modificações para o servidor<br>
`git pull local main` Baixa as modificações<br>
`git push origin main` Envia as modificações para o repositório no <strong>GitHub<strong><br>
`git branch` Ex:(master) ramificações(ramos). Nos informa a branch em que estamos no momento atual<br>
`git branch + <nome a ser dado para a nova branch>` Cria uma nova branch. Ex: `git branch titulo`<br>
`git checkout + <nome que foi dado a nova branch>` Acessa a nova branch criada. Ex: `git checkout titulo`<br>
`git checkout master` Volta para a branch master<br>
`git checkout -b + <nome da nova branch>` Ex: `git checkout -b lista` Atalho para criar nova branch e já acessar<br>
`git merge + nome da branch a ser unificada` Unifica a (branch) com a que estiver acessada no momento. Ex: `git merge titulo` Unifica com a (master) que está acessada no momento.<br>
`:x` + enter Salva a mensagem atual do merge e faz o merging<br>
`git merge --abort` [Desde git versão 1.7.4] Desfazer o git merge<br>
`git reset --merge` [versões anteriores do git] Desfazer o git merge<br>
`git rebase titulo` Traz commits da branch(titulo) para trás da branch (master) e atualiza as 2 branches. OBS: É preciso estar na branch(master), para executar esses códigos ou na branch em que se deseja colocar os commits para trás dela. <b>Obs:</b> <a href="https://github.com/Marcos-Vitor123/git-e-github/blob/440c93779b43cbf6afe5e7dec4ca01f149d2dcc2/Solu%C3%A7%C3%A3o%20para%20erro%20de%20conflito%20de%20arquivos%20usando%20o%20rebase.md">Solução para erro de conflito de arquivos usando o rebase</a><br>
`git log --graph` Exibe linhas específicas de desenvolvimento<br>


<strong>IMPORTANTE! Ler esse artigo no final curso. Como forma de revisão.</strong> <a href="https://training.github.com/downloads/pt_BR/github-git-cheat-sheet/"><strong>Documentação de Git init</strong></a> <strong>instrução de uso do Git no site do GitHub<strong><br>

<strong>Dica! Nunca devo comitar códigos imcompletos ou que não funciona.</strong><br>
