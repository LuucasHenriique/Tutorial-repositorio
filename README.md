# Sessão 1: O Passo a Passo da Criação e Envio

## Nesta primeira etapa, realizei o processo de criação de um repositório no GitHub, configuração de um projeto local no computador e envio dos arquivos para o repositório remoto.

**O Início — Criação do repositório no GitHub
Primeiramente, acessei o GitHub e selecionei a opção Create new repository para criar um novo repositório.
Defini o nome do repositório como:**

**Tutorial-repositorio**

Como a intenção era começar o projeto do zero e fazer a conexão posteriormente pelo computador, criei o repositório inicialmente vazio, sem adicionar arquivos como README, .gitignore ou licença.**

Após a criação, o GitHub disponibilizou o endereço do repositório remoto:

*https://github.com/LuucasHenriique/Tutorial-repositorio.git*

**A Conexão — Criação da pasta local**
Depois de criar o repositório no GitHub, criei uma pasta no meu computador para armazenar os arquivos do projeto.

*O caminho utilizado:*

*C:\Users\LUCASHENRIQUECOSTA\Documents\projeto-git*

Dentro dessa pasta, criei um arquivo chamado index.html, contendo um código HTML simples para servir como primeiro arquivo do projeto.

Em seguida, abri o Prompt de Comando (CMD) diretamente nessa pasta e verifiquei a situação do projeto utilizando:

**git status**

O Git identificou o arquivo index.html como um arquivo ainda não rastreado.

Para transformar a pasta em um repositório Git local, utilizei:

**git init**

Depois, adicionei os arquivos do projeto ao controle de versão:

**git add .**

Em seguida, criei o primeiro registro das alterações utilizando um commit:

**git commit -m "Primeiro commit"**
**Vinculando o projeto local ao GitHub**

Após criar o repositório Git local, realizei a conexão entre o projeto que estava no computador e o repositório criado no GitHub.

Para isso, utilizei o comando:

git remote add origin *https://github.com/LuucasHenriique/Tutorial-repositorio.git*

**O termo origin representa o endereço do repositório remoto que foi configurado.**

Depois, alterei o nome da branch principal de master para main:

**git branch -M main**

O Primeiro Envio — Enviando os arquivos para o GitHub
Com o projeto local configurado e conectado ao repositório remoto, realizei o primeiro envio dos arquivos utilizando:

**git push -u origin main**

Durante esse processo, foi necessário realizar a autenticação da minha conta do GitHub. Após a autenticação, o Git conseguiu estabelecer a conexão com o repositório remoto.

O comando git push enviou o commit que estava armazenado no computador para o GitHub.

Após finalizar o processo, atualizei a página do repositório no GitHub e pude verificar que o arquivo index.html estava disponível na página do repositório.

**Resumo do processo**
**O processo completo realizado foi:**

Criar repositório vazio no GitHub
Criar pasta do projeto no computador
Criar o arquivo index.html
git init
git add .
git commit -m "Primeiro commit"
git remote add origin [URL do GitHub]
git branch -M main
git push -u origin main
Arquivo disponível no GitHub

## Dessa forma, o projeto saiu de uma pasta local no computador e foi enviado para a nuvem por meio do Git e do GitHub. O processo também estabeleceu a conexão entre o repositório local e o repositório remoto, permitindo que futuras alterações possam ser versionadas e enviadas novamente para o GitHub.



# Sessão 2: A Anatomia do README Perfeito
Propósito

## O README.md serve para explicar o projeto de forma simples e organizada. Ele é importante para quem está desenvolvendo o projeto e também para outras pessoas que quiserem entender, instalar ou utilizar o projeto.

**Dados Fundamentais**

Um README profissional deve ter algumas informações importantes, como:

Título: mostra o nome do projeto.
Descrição: explica de forma rápida qual é o objetivo do projeto.
Tecnologias utilizadas: informa quais linguagens e ferramentas foram usadas.
Como instalar e executar: mostra os passos necessários para rodar o projeto.
Status do projeto: informa se o projeto está em desenvolvimento, concluído ou passando por melhorias.
Licença: informa como o projeto pode ser utilizado ou distribuído.
O Poder do Markdown

**Usamos Markdown porque ele permite organizar o texto de uma maneira simples, usando títulos, listas, negrito, códigos e outros elementos. Isso deixa o README mais organizado e fácil de ler, sem precisar escrever HTML para formatar todo o documento.**


# Sessão 3: O Mapa das Atualizações (Commits e Pushes)

## Existem diferentes formas de atualizar um projeto no GitHub, e cada uma pode ser útil dependendo da situação.

*GitHub Online*

**Pelo próprio navegador do GitHub, é possível abrir um arquivo, clicar no botão de edição e alterar o código diretamente. É uma forma rápida para pequenas alterações, principalmente quando estou longe do meu computador. Porém, não é muito prática para projetos maiores e muitas alterações, pois não tenho a mesma facilidade de trabalhar com vários arquivos e testar o projeto localmente.**

**Git via Linha de Comando (Terminal)**

Pelo terminal, posso atualizar o projeto usando comandos como:

git add .
git commit -m "Descrição da alteração"
git push

Essa é uma das formas mais tradicionais porque permite ter bastante controle sobre as alterações e funciona praticamente em qualquer ambiente que tenha o Git instalado.

**IDEs — VS Code**

No VS Code, posso fazer as alterações no código e utilizar a própria interface gráfica do Git para visualizar os arquivos modificados, fazer o commit e depois o push. Acho essa opção mais prática porque consigo editar o código e controlar o Git no mesmo programa.

**GitHub Desktop**

**O GitHub Desktop é uma ferramenta criada para facilitar o uso do Git através de uma interface gráfica. Ele mostra os arquivos que foram modificados e permite escrever a mensagem do commit, fazer o commit e depois enviar as alterações para o GitHub sem precisar digitar todos os comandos no terminal.**

A Filosofia da Atualização

## É importante atualizar o repositório continuamente e fazer commits em pequenas partes. Assim, cada alteração fica registrada e, se acontecer algum problema, fica mais fácil descobrir o que foi alterado e voltar para uma versão anterior. Deixar tudo para o final pode dificultar bastante a organização e a identificação de erros.
