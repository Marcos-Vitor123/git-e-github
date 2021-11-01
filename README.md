 Sistemas de controle de versões 

* Git Bash => Fornece comandos do Linux
$ ```` => Mostra todas as pastas e arquivos
$ git --version => diz a versão do Git
$ git config --local user.name "Seu nome aqui" => Nome do autor que irá fazer as alterações no arquivos
$ git config --local user.email "seu@email.aqui" => Email do autor que irá fazer as alterações no arquivos
$ git init => Transforma a pasta atual em repositório
$ git config --list --local => Confere 
$ git status => Mostra o estado do repositório ou quais arquivos foram alterados
* On branch master => ramo ou branch
$ git add <Nome do arquivo > => Adciona 1 arquivo específico no Git ou inclui arquivos no commits, que passa a monitorar.
$ git add . ou git add -A => Adciona todos os arquivos no Git
$ git commit -m "nome da alteração + detalhes se quiser"(commit) => Salva a alteração recente e indica mudanças como um "check point"
* Changes to committed => mudanças a serem commitadas
$ git rm => remove o arquivo recém adcionado deixando de ser monitorado.
* HEAD => Estado atual do nosso código, onde o Git os colocou.
* Working tree => Local onde os arquivos estão sendo editados.
* index => Local onde o git armazena o que será commitado ou local entre a working tree e o repositório Git em si.
$ git log => Vê o histórico de alterações.
* hash do commit => uma identificação única de cada commit
$ git config --local user.name "nome alterado" => Configuração para cada projeto
$ git config --global => para máquina toda
$ git config user.email => visualisa as configurações de email
$ git config user.name => visualisa as configurações do nome
$ git log --oneline => visualisa as alterações resumida em uma única linha
$ git log -p => visualisa as alterações detalhada, inclusive códigos ou escrita que era antes e mostra como ficou depois
$ git log --pretty="format:%H" => comando que nos traz apenas o hash
$ git log --pretty="format:%h %s" => traz o hash resumido seguido pela mensagem do commit
$ git log --help => exibe página manual de git-log
* .gitignore => Arquivo criado na mesma pasta do projeto, em que ignora os arquivos ou pastas nos commits. Para isso, coloca-se o nome do arquivo ou pasta + uma barra no final dentro do ".gitignore"
$ cd .. => Volta uma pasta acima da pasta do projeto
$ mkdir => Cria uma pasta --> detalhe: coloque o nome da pasta logo após o comando
$ cd + nome da pasta + uma barra no final => Acessa a pasta
$ git init --bare => Após o comando $ git init para transformar esse repositório em servidor onde fica somente as alterações dos arquivos e não uma cópia de cada.
* --bare => parâmetro
$ git remote => lista todos os repositórios remotos
$ git remote add + nome escolhido a esse repositório remoto(ex: local) + o caminho onde ele fica(pasta com os arquivos). Pode ser uma url, um endereço na rede ou uma pasta no computador e etc...
$ git remote -v => Mostra o endereço do local
* (fetch) => Busca
* (puch) => Envia 
* pull => pega(puchar)
$ rm => remove pasta ou diretório(flag -rf --> para remover tudo dentro de uma pasta)
$ rm -rf .git => Excluir repositório do Git
$ ls -lah => Verificar se o repositório está oculto
$ git clone => Trazer pela primeira vez um repositório remoto para a sua máquina. (Clonar) Para isso digite além do comando --> + local do disco ex: /c/ ou /d/ e etc. + o endereço do servidor remoto + 1 espaço + o nome do projeto que tu quiser por. Caso contrário, o nome do projeto ficará com o nome servidor
$ git push + nome do repositório remoto (local) + a branch (master) ex: $ git push local master
$ git remote rename origin local => renomeia repositório remoto local(origin --> nome do repositório local atual)
$ git pull local master => trazer os dados de um repositório remoto para o meu (OBS: local --> outro repositório remoto), (master --> branch)
$ git remote add + nome repositório(origin) + link do repositório(https) criado no GitHub => linka repositório remoto com GitHub
$ git push -u + nome repositório(origin) + master => Sempre que der um push nesse repositório master, ele será adcionado no repositório remoto adcionado(origin)
$ git push + nome repositório(origin) + master => empurra a versão atualizada para o GitHub
$ git push local main => envia as modificações para o servidor
$ git pull local main => baixa as modificações
$ git push origin main => envia as modificações para o repositório no GitHub
$ git branch => ex:(master) ramificações(ramos) --> nos informa a branch em que estamos no momento atual
$ git branch + nome a ser dado para a nova branch => Cria uma nova branch --> ex:(git branch titulo)
$ git checkout + nome que foi dado a nova branch => ex:(git checkout titulo) --> Acessa a nova branch criada
$ git checkout master => volta para a branch master
$ git checkout -b + nome da nova branch => ex:(git checkout -b lista) --> Atalho para criar nova branch e já acessar

IMPORTANTE! Ler esse artigo no final curso. Como forma de revisão.

Documentação degit init instrução de uso do Git no site do GitHub => https://training.github.com/downloads/pt_BR/github-git-cheat-sheet/

Dica! Nunca devo comitar códigos imcompletos ou que não funciona.