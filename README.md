
# Resumo Git e GitHub
Repositório desenvolvido para fins educativo, para armazenar resumo sobre Git e GitHub do curso Versionamento de Código com Git e GitHub da DIO.

[DIO - Digital Innovation One](https://www.dio.me/curso-git-github-ci-cd/AFZSJCW04E1V)

[![Link do Curso](https://img.shields.io/badge/▶-000?style=for-the-badge&logo=movie&logoColor=E94D5F)](https://www.dio.me/curso-git-github-ci-cd/AFZSJCW04E1V) 
[![Link do Curso](https://img.shields.io/badge/Acesse%20o%20Curso%20na%20Plataforma-E94D5F?style=for-the-badge)](https://web.dio.me/course/versionamento-de-codigo-com-git-e-github/learning/f3cbaa66-efbd-4c25-842e-2069c188c066)

## 📒 Ferramentas e Documentação
[![Git](https://img.shields.io/badge/Git-000?style=for-the-badge&logo=git&logoColor=E94D5F)](https://git-scm.com/doc) 
[![GitHub](https://img.shields.io/badge/GitHub-000?style=for-the-badge&logo=github&logoColor=30A3DC)](https://docs.github.com/)


## 💻 Resumo das Aulas
| Nº | Titulo do Resumo | Links |
| --- | ----- | ------- |
| 01 | Comandos Básicos DOS Powershell | [![Link](https://img.shields.io/badge/Ver%20Resumo-E94D5F?style=for-the-badge)](#01---comandos-básicos-dos-powershell) |
| 02 | Configuração do Git| [![Link](https://img.shields.io/badge/Ver%20Resumo-30A3DC?style=for-the-badge)](#02---configuração-do-git)|
| 03 | AUTENTICAÇÃO Via Token | [![Link](https://img.shields.io/badge/Ver%20Resumo-E94D5F?style=for-the-badge)](#03---autenticação-via-token-link)|
| 04 | AUTENTICAÇÃO Via SSH | [![Link](https://img.shields.io/badge/Ver%20Resumo-30A3DC?style=for-the-badge)](#04---autenticação-via-ssh---link)|
| 05 | Criando e Clonando Repositórios | [![Link](https://img.shields.io/badge/Ver%20Resumo-E94D5F?style=for-the-badge)](#05---criando-e-clonando-repositórios)|
| 06 | SALVANDO Alterações no Repo Local| [![Link](https://img.shields.io/badge/Ver%20Resumo-30A3DC?style=for-the-badge)](#06---salvando-alterações-no-repositório-local)|
| 07 | DESFAZENDO Alterações no Repo Local | [![Link](https://img.shields.io/badge/Ver%20Resumo-E94D5F?style=for-the-badge)](#07---desfazendo-alterações-no-repositório-local)|
| 08 | ENV. E BAIXANDO Alterações no REPO REMOTO | [![Link](https://img.shields.io/badge/Ver%20Resumo-30A3DC?style=for-the-badge)](#08---enviando-e-baixando-alterações-no-repositório-remoto)|
| 09 | TRABALHANDO COM BRANCHES | [![Link](https://img.shields.io/badge/Ver%20Resumo-E94D5F?style=for-the-badge)](#09---trabalhando-com-branches---criando-mesclando-deletando-e-tratando-conflitos)|
| 10 | TRABALHANDO COM BRANCHES - Dia a Dia| [![Link](https://img.shields.io/badge/Ver%20Resumo-30A3DC?style=for-the-badge)](#10---trabalhando-com-branches---comandos-úteis-no-dia-a-dia)|
| - | ------------------------ | - |

## 🔎 Referências
- [DIO - Digital Innovation One](https://www.dio.me/curso-git-github-ci-cd/AFZSJCW04E1V)
- [Instr. - @elidianaandrade](https://github.com/elidianaandrade)

## 👨‍💻 Autor
Feito com 💙 por [@kleutons](https://github.com/kleutons)
##

<br>
<br>
<br>
<br>
<br>


## 01 - Comandos Básicos DOS Powershell
[ ◀️ Voltar ao Inicio](#-resumo-das-aulas)

- Limpar Tela
```
clear
```
- Sistemas de Pastas e Arquivos
```
#Criar Pasta
mkdir [NOME-DA-PASTA]

#Navegar ao diretório (Pasta específica)
cd [ENDEREÇO-DA-PASTA]

#Listar arquivos de um diretório 
ls

#exibe conteúdo de um arquivo
cat [ENDEREÇO-DO-ARQUIVO]
```
- Criar Arquivos Vazios
```
touch [NOME-DO-ARQUIVO.EXTENSÃO]
```
<br>
<br>

## 02 - Configuração do Git
[ ◀️ Voltar ao Inicio](#-resumo-das-aulas)
- Exibe os comandos git config
```
git config
```

- Exibe todas as config globais
```
git config --global --list
```

- Alterar Nome e Email Global
```
git config --global user.name "[SEU-NOME]"
git config --global user.email [SEU-EMAIL]
```

- Consultar Branch Padrão 
``` 
git config init.defaultBranch
```

- Alterar Branch Padrão 
```
git config --global init.defaultBranch [NOME-NOVA-BRANCH]
```

<br>
<br>

## 03 - AUTENTICAÇÃO Via Token [LINK](https://github.com/settings/apps)
[ ◀️ Voltar ao Inicio](#-resumo-das-aulas)
- Salvar Credencial (após usar esse comando usar git clone e inseri o token)
```
git config credential.helper store
```

- Como Clonar o repositorio e inseri o token
```
git clone [URL]
```
- Armazenamento de credenciais
```
git config --global credential.helper
```

- Exibe local a pasta de armazenamento 
```
git config --global --show-origin credential.helper
```

- Exibe conteúdo da credencial, se você já está na pasta de configurações
```
cat .git.credentials
```

- Exibe conteúdo e um arquivo, nesse caso .gitconfig, tem está dentro da pasta que deseja abri o arquivo.
```
cat .gitconfig
```


<br>
<br>

## 04 - AUTENTICAÇÃO Via SSH - [Link](https://docs.github.com/pt/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
[ ◀️ Voltar ao Inicio](#-resumo-das-aulas)

- Primeiro criar sua chave SSH

- Verificar se já existe uma chave na máquina 
```
ls -a ~/.ssh
```

- Criar uma chave SSH na Máquina, vai pedir para selecionar o local padrão, se não deseja alterar é só digitar Enter, após vai pedir para definir uma senha, que você deve digitar 2x
```
ssh-keygen -t ed25519 -c "[SEU-EMAIL]"
```

[SSH AGENT](https://docs.github.com/pt/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)

- Iniciar o SSH Agent
```
eval "$(ssh-agent -s)"
```

- Adicionar o SSH Agent, vai pedir a Senha da chave SSH
```
ssh-add ~/.ssh/id_ed25519
```

[CRIAR SSH GITHUB](https://github.com/settings/keys)

- Pegar Chave SSH de sua máquina
```
#navegar até a pasta ssh
cd ~/.ssh 
#listar chaves
ls
#exibir chave
cat id_ed25519
```

- Após pegar a chave adicione no seu GitHub no link acima, criar SSH.

- Clonar Repo via SSH, pede a senha da sua chave ssh
```
git clone [URL-SSH] 
```


<br>
<br>

## 05 - Criando e Clonando Repositórios
[ ◀️ Voltar ao Inicio](#-resumo-das-aulas)

- Iniciar Git, criação da pasta /.git
```
git init
```

- Clonar Repositório
```
git clone [URL-GITHUB]

# Se desejar definir o nome para pasta
git clone [URL-GITHUB] [NOME-DA-PASTA]
```
- Clonar Repositório chamando a Branch
```
git clone [URL-GITHUB] --branch [NOME-DA-BRANCH] --single-branch
```


- Exibe Configurações do Repositório dentro da pasta ./git
```
cat config
```

- Exibe Repositório Remoto
```
git remote -v
```

- Conectar ao Repositório Remoto
```
git remote add origin [URL-DO-REPO-GITHUB] **[NOME-DA-PASTA]
```


<br>
<br>

## 06 - SALVANDO Alterações no Repositório Local
[ ◀️ Voltar ao Inicio](#-resumo-das-aulas)

- Adicionar arquivos atualizados, feitos alterações:
```
#adciona todos os arquivos pendentes
git add .

#adcionar arquivo único
git add [NOME-DO-ARQUIVO]
```

- Exibe o Status, estados dos arquivos, se existe arquivos rastreados 
```
git status
```

- Inserir Commit, quando finalizar as alterações no arquivo ou conjunto de arquivos
```
git commit -m “[NOME-DO-COMMIT]”
```

- Mostrar Últimos Commits Realizados, exibe autor com email e data.
```
git log
```

- Salvar diretório Pasta Vazia no git, (Crie a pasta e insira o arquivo dentro da pasta .gitkeep)
```
touch [NOME-DA-PASTA]/.gitkeep
```

- Escrevendo no arquivo gitignore ( O Git-Ignore serve para ignorar arquivos no git)
```
echo [NOME-DO-ARQUIVO-OU-PASTA]  >  .gitignore

## exemplo pasta nome: resumos
echo resumos/  >  .gitignore
```

<br>
<br>

## 07 - DESFAZENDO Alterações no Repositório Local 
[ ◀️ Voltar ao Inicio](#-resumo-das-aulas)

- Para um bom uso desses comandos abaixo sempre use em conjunto o git status para analisar os status do commits 

- Remover a força o diretório .git e todo o seu conteúdo (se usar o git .init na pasta errada por exemplo)
```
rm -rf .git
```

- Restaurar Arquivo para o último Commit anterior, recupera.
*Atenção esse comando apagar qualquer alteração feita recentemente e voltar e restaura o arquivo parar ter o conteúdo anterior, isso pode acarretar perdas de trabalhos.
```
git restore [NOME-DO-ARQUIVO]
```

- Alterar Mensagem Do Último Commit, caso você deseja alterar a mensagem do commit ante de enviar para o repositório remoto.
```
git commit --amend -m“[ESCREVA-NOVA-MENSAGEM]”
```

- Desfazer Commit, caso você não queira resetar o commit para fazer novamente, Hash Do Commit é o identificador do commit, para pegar esse id use o comando {git log}
--  Soft, remove o commit mas mantém todas as mudanças nos arquivos
```
git reset --soft [HASH-DO-COMMIT]
```

- Desfazer Commit 
-- Mixed e remove da adição de arquivos, para que você possa adicionar os arquivos novamente no rastreamento a arvore de trabalho
```
git reset --mixed [HASH-DO-COMMIT]
```

- Desfazer Commit 
-- Hard,  descarta todas as mudanças feitas, Apaga os arquivos (Muito Cuidado)
```
git reset --hard [HASH-DO-COMMIT]
```

<br>
<br>

## 08 - ENVIANDO E BAIXANDO Alterações no REPOSITÓRIO REMOTO
[ ◀️ Voltar ao Inicio](#-resumo-das-aulas)

- Enviando Arquivo para repositório remoto
```
git remote add origin [URL-GITHUB]

#forçar para usar a Branch main, opcional
git branch -M main

#enviar os arquivos para a Branch remota main
git push – origin main
```

- Baixado Arquivos alterados no Repositório Remoto Online
```
git pull
```

<br>
<br>

## 09 - TRABALHANDO COM BRANCHES - Criando, Mesclando, Deletando e Tratando Conflitos
[ ◀️ Voltar ao Inicio](#-resumo-das-aulas)

- Listar todas as Branchs e mostrar a selecionada com asterisco 
```
git branch
```

- Trocando de Branch 
```
git checkout -b [NOME-DA-BRANCH]

#exemplo sair da branch [main] e ir para a branch [teste]
git checkout -b teste
```

- Use o ( $ git log  ) para saber os apontamentos de cada Branch apontando ao commit

- Exibir, listar o ultimo Commit referente a cada Branch correspondida
```
git branch -v
```

- Mesclar duas Branch, para unir 2 branch navegue a branch principal e use o comando abaixo, isso vai mesclar todos os arquivos de cada branch.
```
git merge [NOME-DA-BRANCH-SEGUNDARIA]
```

- Deletar Excluir um Branch 
```
git branch -d [NOME-DA-BRANCH]
```

- Tratando Conflitos:
Caso existe alguma nova alteração Commit feita na branch remota, e você tentar enviar uma outra nova alteração do repositório local vai dar conflito e o Github não vai permitir o envio desse novo commit, o que fazer?

<details>
<summary>1.	Salve suas alterações atuais:</summary>
Antes de qualquer coisa, certifique-se de que suas alterações locais estão salvas em commits separados usando git commit.
</details>

<details>
<summary>2.	Sincronize com a branch remota:</summary>
Execute o comando git pull origin <nome-da-branch> para trazer as alterações remotas para o seu repositório local. Isso fará o download das alterações da branch remota e tentará fazer um merge automático com as suas alterações locais.
</details>

<details>
<summary>3.	Resolva conflitos:</summary>
Se ocorrerem conflitos, o Git informará quais arquivos estão em conflito. Você precisará resolver esses conflitos manualmente editando os arquivos em questão. Dentro dos arquivos, você verá marcações que indicam as diferenças entre as versões. Remova as marcações e ajuste o conteúdo do arquivo conforme necessário para resolver os conflitos.
</details>


<details>
<summary>4.	Commit das alterações de resolução de conflitos:</summary>
Após resolver os conflitos, adicione os arquivos alterados usando git add e, em seguida, faça um novo commit para registrar as alterações de resolução de conflitos.
</details>

<details>
<summary>5.	Envie as alterações resolvidas::</summary>
Agora você pode fazer um git push para enviar suas alterações para a branch remota. Como você resolveu os conflitos, o GitHub permitirá o envio sem problemas.
</details>



<br>
<br>

## 10 - TRABALHANDO COM BRANCHES - Comandos Úteis no Dia a Dia
[ ◀️ Voltar ao Inicio](#-resumo-das-aulas)
- O Comando git pull é uma junção -> git fetch + git merge, que nada mais é do que uma junção das alterações e os novos arquivos a serem baixando para o repositório local

- Caso queira baixar as alterações sem mesclar com os arquivos local, use git fetch
```
git fetch origin [NOME-DA-BRANCH]
```

- Após baixar as alteração, é possível ver as diferença, use o diff. 
```
git diff [NOME-BRANCH] origin/[NOME-BRANCH]
```

- Para trazer as Alterações
```
git merge origin [NOME-DA-BRANCH]
```

- Clonar Repositório, chamando a branch específica
```
git clone [URL] --branch [NOME-DA-BRANCH] --single-branch
```

<br>
<br>

## 👨‍💻 Autor
Feito com 💙 por [@kleutons](https://github.com/kleutons)
##

<br>
<br>