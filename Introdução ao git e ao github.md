### Introdução ao Git

#### Entendendo o que é Git e sua importância

Imagine que você tenha um artigo, escreva nele e dai você revisa. Ai você tenha um artigo antigo. Imagina que faça isso de novo, agora você tem mais um artigo antigo2. E de novo um rascunho. E depois criar um arquivo final.

![[../Files/Pasted image 20220713125240.png]]

Para resolver esse problema de versionamento, existe o GIT.

Criado por Linus Torvalds.

O Software é feito de forma colaborativa e o Linux é um Kernel para sistema operacional open source feito de forma colaborativa. Dessa forma, eles tiveram que usar o sistema de versionamento de código da época e ele teve um grande descontentamento.

GIT x GITHUB
sistema de versionamento x repositório online
![[../Files/Pasted image 20220713125931.png]]

Vantagens de usar o git e o git hub:

1. Controle de versão
2. Armazenamento em nuvem
3. Trabalho em equipe
4. Melhorar seu código
5. Reconhecimento

### Navegação via command line interface e instalação

#### Comandos básicos para um bom desempenho no terminal

GUI x CLI
GUI → Interface responsiva
CLI → (Command Line Interface) Linha de comando

O git foi concebido para ser usado na CLI.

O que vamos aprender?

- Mudar de pastas
- Listar as pastas
- Criar pastas/arquivos
- Deletar pastas/arquivos

| Windows    | Unix   |
| ---------- | ------ |
| cd         | cd     |
| dir        | ls     |
| mkdir      | mkdir  |
| del/ rmdir | rm -rf |

Windows

```bash
cd /           # Vai para o diretório raiz
dir            # Lista todos os diretórios
cd ..          # Retrocede um nível de navegação
cd (pasta)     # Vai para a pasta
cls            # Clear screen
(tab)          # Auto completar
mkdir (pasta)  # Criar nova pasta
echo (texto)   # Imprime o (texto)
echo hello > hello.txt  # Redireciona o fluxo do echo para um txt
del (pasta)    # Deleta todos os arquivos dentro de uma pasta
rmdir (pasta) /S /Q  # Deleta a pasta com todos arquivos
```

Linux

```bash
cd /           # Vai para o diretório raiz
ls             # Lista todos os diretórios
cd ..          # Retrocede um nível de navegação
cd (pasta)     # Vai para a pasta
clear          # Limpar a tela
(ctrl + l)     # Limpa a tela tb
(tab)          # Auto completar
mkdir (pasta)  # Criar nova pasta
echo (texto)   # Imprime o (texto)
echo hello > hello.txt  # Redireciona o fluxo do echo para um txt
rm -rf (pasta) # Apagar uma pasta com todos arquivos (r → recursive, f → force (não pede permissão para deleção))
```

#### Realizando a instalação do GIT

Instalação do GIT: é só ir no site do git e baixar.
![[../Files/Pasted image 20220713131354.png]]
![[../Files/Pasted image 20220713131408.png]]
![[../Files/Pasted image 20220713131459.png]]

A instalação do git no linux é bem mais simples, sendo um comando dependendo da sua distro.

Conferir se o git foi instalado

```bash
git --version
```

Para mac, isntalar o homebrew e dar o comando

```bash
brew install git
```

### Entendendo como o Git funciona por baixo dos panos

#### Tópicos fundamentais para entender o funcionamento do Git

- SHA1
- Objetos fundamentais
- Sistema distribuído
- Segurança

##### SHA1

A sigla SHA significa Secure Hash Algorithm (Algoritmo de Hash Seguro), é um conjunto de funções hash criptográficas projetadas pela NSA (Agência de Segurança Nacional dos EUA).

A encriptação gera um conjunto de caracteres com um identificador de 40 dígitos.

É uma forma curta de representar um arquivo.
![[../Files/Pasted image 20220713132414.png]]

Passar arquivo para o sha1:

```bash
openss1 sha1 text.txt
```

"Para mesmos conjunto de binários, são gerados os mesmos hashes".

#### Objetos internos do Git

##### Blobs

![[../Files/Pasted image 20220718115828.png]]
Por que isso ocorre sendo que os dois são convertidos para SHA1?

É porque o git guarda esse objeto em um tipo de arquivo chamado blob
![[../Files/Pasted image 20220718115910.png]]

![[../Files/Pasted image 20220718115922.png]]

(O git guarda metadados no objeto blob)

##### Trees

Objetos que armazenam blobs
![[../Files/Pasted image 20220718120018.png]]

A árvore guarda o nome do arquivo, blobs ou outras árvores. (Como se fosse um sistema de diretório).

![[../Files/Pasted image 20220718120151.png]]

##### Commit

![[../Files/Pasted image 20220718120209.png]]

O commit aponta para uma árvore, para um autor, um parente, uma mensagem e um timestamp.

##### Hierarquia dos objetos do git

![[../Files/Pasted image 20220718120401.png]]
Dessa forma o git é um sistema distribuído seguro.

#### Chave SSH e Token

![[../Files/Pasted image 20220718120547.png]]

Quando você vai jogar o código para o github, você vai ter que se autenticar.

##### Chave SSH

Chave pública e chave privada. Ao colocarmos uma chave pública no github, o github já vai entender onde a situação da nossa conexão.

E como fazer isso?
**Passo 1**. Ir em settings
![[../Files/Pasted image 20220718120816.png]]

**Passo 2**. Ir em SSH and GPG keys
![[../Files/Pasted image 20220718120850.png]]

Agora precisamos gerar uma chave SSH no git.

**Passo 3**. Gerar chave SSH no git

```bash
ssh-keygen -t ed25519 -C {email vinculado}
# ssh-keygen -t ed25519 -C otaviocha@gmail.com
# (optional passphrase as password)
cd {directory where key was saved}
ls
# Two files will be showed, one with .pub in the final, that's the public key
```

**Passo 4**. Copiar a chave pública na seção "new SSH Key"
![[../Files/Pasted image 20220718121357.png]]

**Passo 5**. Rodar o processo encarregado pelas chaves.

```bash
eval $(ssh-agent -s)
ssh-add {caminho chave privada}
```

Agora ao copiar um projeto para sua máquina, use o SSH
![[../Files/Pasted image 20220718121708.png]]

![[../Files/Pasted image 20220718121827.png]]

##### Token de acesso pessoal

**Passo 1**. Ir em settings
![[../Files/Pasted image 20220718120816.png]]

**Passo 2**. Ir em developer settings
![[../Files/Pasted image 20220718122350.png]]

**Passo 3**. Criar novo token
![[../Files/Pasted image 20220718122445.png]]

**Passo 4**. Copiar o seu token
![[../Files/Pasted image 20220718122501.png]]

Como clonar agora um repo na máquina?
Pelo token de acesso, usar o HTTPS
![[../Files/Pasted image 20220718122545.png]]

![[../Files/Pasted image 20220718122656.png]]

![[../Files/Pasted image 20220718122712.png]]

### Primeiros comandos com Git

#### Iniciando o Git e criando um commit

- Iniciar o GIT
- Iniciar o versionamento
- Criar um commit

Comandos envolvidos:

```bash
git init
git add
git commit
```

Criando um repositório:
**Passo 1**. Checkar o diretório dentro do git
**Passo 2**. Inicializar o git

```bash
git init
```

Para ver a pasta gerencial $.git$:

```bash
ls -a
```

**Passo 3**. Configurar um autor para os commits

```bash
git config --global user.email "{email}"
git config --global user.name "{nome}"
```

(O parâmetro `--global` é opcional, sendo possível usar apenas uma configuração no repo local).

Linguagem markdown
![[../Files/Pasted image 20220718123355.png]]
O markdown é uma forma humanizada de escrever HTML.

![[../Files/Pasted image 20220718123803.png]]

> Blockquote
> ![[../Files/Pasted image 20220718123803.png]]
> Teste?

**Passo 4**. Criar arquivos
**Passo 5**. Commitar

```bash
git add *
git commit -m "Commit inicial"
```

### Ciclo de vida dos arquivos no Git

#### Passo a passo no ciclo de vida

Quando usamos o `git init` estamos criando um repositório dentro daquela pasta.

Estados dos arquivos do git
![[../Files/Pasted image 20220718124235.png]]

Quando criamos um arquivo novo, ele entra como estado untracked.
O staged é "o palco dos arquivos que irão para o novo commit".

Locais dentro do contexto do git
![[../Files/Pasted image 20220718124556.png]]

![[../Files/Pasted image 20220718124723.png]]
![[../Files/Pasted image 20220718124732.png]]

Conferir mudanças que estão no staging area:

```bash
git status
```

Quando trocamos um arquivo de lugar, isso acontece:
![[../Files/Pasted image 20220718125028.png]]

Uma maneira elegante de resolver isso no git é fazendo:

```bash
git add {arquivo} {local novo}
```

![[../Files/Pasted image 20220718125226.png]]

![[../Files/Pasted image 20220718125249.png]]

Criando README.md
![[../Files/Pasted image 20220718125337.png]]

Agora para commitar isso:

```bash
git add *
git commit -m "Adiciona index"
```

### Introdução ao GitHub

#### Trabalhando com o GitHub

Ver configurações do git:

```bash
git config --list
```

Para o git hub é ideal que usemos as mesmas configurações do github na nossa máquina.

Desfazer config

```bash
git config --global --unset user.email
git config --global --unset user.name
```

Fazer config

```bash
git config --global user.email {email}
git config --global user.name {name}
```

##### Importar do repo local para o repo remoto github

```bash
git remote add origin https://github.com/user/repo.git
git remote -v
```

Por convenção usamos o nome "origin", mas ele é só um alias para o link do nosso repo

Agora a gente empurra para o github:

```bash
git push origin master
```

```ad-example
git → comando git
push → empurrar
origin → alias
master → branch
```

### Resolvendo conflitos

![[../Files/Pasted image 20220721132753.png]]

Código desse tipo de erro
![[../Files/Pasted image 20220721132910.png]]

Como resolver?

```bash
git pull origin master
```

![[../Files/Pasted image 20220721133109.png]]

Resolvendo o arquivo conflitado manualmente
![[../Files/Pasted image 20220721133151.png]]

Aceitando as novas modificações
![[../Files/Pasted image 20220721133256.png]]

![[../Files/Pasted image 20220721133331.png]]
.
![[../Files/Pasted image 20220721133342.png]]

#### Como os conflitos acontecem no GitHub e como resolvê-los

![[../Files/brave_28aEOQcsv2.png]]

![[../Files/brave_2jnEOzTTFW.png]]

![[../Files/brave_CS8MxBbone.png]]

![[../Files/brave_Eso8KQURYo.png]]

![[../Files/brave_FFceI3qepe.png]]

![[../Files/brave_o67oFrYiw5.png]]

![[../Files/brave_1F9HVLyVDt.png]]

## Criando seu primeiro repositório no github para compartilhar seu progresso

### Introdução e apresentação do projeto

```ad-quote
"Alguém está sentado na sombra hoje porque alguém plantou uma árvore há muito tempo" - Warren Buffet
```

Reforce seu conhecimento em Git com um desafio totalmente prático, onde você executará todos os passos para a criação, atualização e sincronização de um repositório no GitHub.

Com isso, você poderá compartihlar suas anotações e exercícios em seu próprio repositório. Criando assim, o primeiro (de muitos) projetos do seu portfólio.

Requisitos:

- Noções básicas de Git/GitHub
- Git devidamente instalado (usaremos o git bash)
- Engajamento e vontade de aprender

### Git e Github: Relembrando algumas coisinhas

Criando repo pelo github...
Depois clonar no local
Modificar no local
Commitar e dar push no origin

### Desafio de projeto

Agora é a sua hora de brilhar, use todo seu conhecimento em Git e GitHub para criar o seu próprio repositório. Com isso, em breve você terá muitos outros projetos no seu perfil no GitHub.
Desta forma, outros Devs ou empresas poderão acessar seu portfólio de projetos e colaborar/acompanhar sua evolução profissional.

### Entendendo o Desafio

```ad-question
Descrição do Desafio
Reforce seu conhecimento em Git com um desafio de projeto totalmente prático, onde você executará todos os passos para a criação, atualização e sincronização de um repositório no GitHub. Para isso, tenha em mente todas as dicas e direcionamentos apresentados pelo expert nas aulas. Dessa forma, você poderá compartilhar suas anotações e exercícios em seu próprio repositório. Criando assim, o primeiro (de muitos) projetos do seu portfólio ;)

Slides
A apresentação utilizada neste conteúdo está disponível AQUI

Com isso, você terá acesso a todos os slides e links apresentados durante as aulas.

Bons estudos
```
