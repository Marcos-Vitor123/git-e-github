 <h1>Sistemas de controle de versões</h1> 

<b>Git Bash</b> Fornece comandos do Linux
<b>On branch master</b> Ramo ou branch
<b>Changes to committed</b> Mudanças a serem commitadas
<b>HEAD</b> Estado atual do nosso código, onde o Git os colocou.
<b>Working tree</b> Local onde os arquivos estão sendo editados.
<b>index</b> Local onde o git armazena o que será commitado ou local entre a working tree e o repositório Git em si.
<b>hash do commit</b> Uma identificação única de cada commit
<b>.gitignore</b> Arquivo criado na mesma pasta do projeto, em que ignora os arquivos ou pastas nos commits. Para isso, coloca-se o nome do arquivo ou pasta + uma barra no final dentro do <b>.gitignore</b>
<b>(fetch)</b> Busca
<b>(puch)<b> Envia 
<b>pull</b> Puchar

`ls` Mostra todas as pastas e arquivos
`git --version` Diz a versão do Git
`git config --local user.name "Seu nome aqui"` Nome do autor que irá fazer as alterações no arquivos
`git config --local user.email "seu@email.aqui"` Email do autor que irá fazer as alterações no arquivos
`git init` Transforma a pasta atual em repositório
`git config --list --local` Confere 
`git status` Mostra o estado do repositório ou quais arquivos foram alterados
`git add + <Nome do arquivo>` Adciona 1 arquivo específico no Git ou inclui arquivos no commits, que passa a monitorar.
`git add .` ou `git add -A` Adciona todos os arquivos no Git
`git commit -m "nome da alteração + detalhes se quiser"`(commit) Salva a alteração recente e indica mudanças como um <b>"check point"</b>
`git rm` Remove o arquivo recém adcionado deixando de ser monitorado.
`git log` Vê o histórico de alterações.
`git config --local user.name "nome alterado"` Configuração para cada projeto
`git config --global` Para máquina toda
`git config user.email` Visualisa as configurações de email
`git config user.name` Visualisa as configurações do nome
`git log --oneline` Visualisa as alterações resumida em uma única linha
`git log -p` Visualisa as alterações detalhada, inclusive códigos ou escrita que era antes e mostra como ficou depois
`git log --pretty="format:%H"` Comando que nos traz apenas o hash
`git log --pretty="format:%h %s"` Traz o hash resumido seguido pela mensagem do commit
`git log --help` Exibe página manual de git-log
`cd ..` Volta uma pasta acima da pasta do projeto
`mkdir + <Nome da pasta>` Cria uma pasta
`cd + <Nome da pasta/>` Acessa a pasta
`git init --bare` Para transformar o repositório em servidor onde fica somente as alterações dos arquivos e não uma cópia de cada. <b>--bare</b> Parâmetro
`git remote` Lista todos os repositórios remotos
`git remote add + <Nome do repositório remoto> + <Caminho da pasta com os arquivos>` (ex: local). Pode ser uma url, um endereço na rede ou uma pasta no computador e etc...
`git remote -v` Mostra o endereço do local
`rm -rf + <nome da pasta>` Remove pasta ou diretório do Git(flag `-rf` para remover tudo dentro de uma pasta)
`rm -rf .git` Excluir repositório do Git
`ls -lah` Verificar se o repositório está oculto
`git clone + <local do disco ex: /c/ ou /d/ e etc.> + <endereço do servidor remoto> + <1 espaço> + <nome do projeto>` Trazer pela primeira vez um repositório remoto para a sua máquina (Clonar).
`git push <nome do repositório remoto(local)> + <a branch (master)>` Ex: `git push local master`
`git remote rename origin local` Renomeia repositório remoto local(<b>origin</b> nome do repositório local atual)
`git pull local master` Trazer os dados de um repositório remoto para o meu (OBS: <b>local</b> outro repositório remoto), (<b>master<b> branch).
`git remote add + <nome repositório(origin)> + <link do repositório(https) criado no GitHub>` Linka repositório remoto com o <b>GitHub</b>
`git push -u + <nome repositório(origin)> + <master>` Sempre que der um <b>push</b> nesse repositório <b>master</b>, ele será adcionado no repositório remoto adcionado(origin).
`git push + <nome repositório(origin)> + <master>` => empurra a versão atualizada para o GitHub
`git push local main` Envia as modificações para o servidor
`git pull local main` Baixa as modificações
`git push origin main` Envia as modificações para o repositório no <b>GitHub<b>
`git branch` Ex:(master) ramificações(ramos). Nos informa a branch em que estamos no momento atual
`git branch + <nome a ser dado para a nova branch>` Cria uma nova branch. Ex: `git branch titulo`
`git checkout + <nome que foi dado a nova branch>`. Ex: `git checkout titulo` Acessa a nova branch criada
`git checkout master` Volta para a branch master
`git checkout -b + <nome da nova branch>`. Ex: `git checkout -b lista` Atalho para criar nova branch e já acessar

<b>IMPORTANTE! Ler esse artigo no final curso. Como forma de revisão.</b>

<a href="https://training.github.com/downloads/pt_BR/github-git-cheat-sheet/"><b>Documentação de Git init</b></a> <b>instrução de uso do Git no site do GitHub</b>

<b>Dica! Nunca devo comitar códigos imcompletos ou que não funciona.</b>