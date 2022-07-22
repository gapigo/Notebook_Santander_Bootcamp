## Introdução à programação e pensamento computacional

### 1 Pensamento computacional

#### Apresentação

Outros cursos da professora:

- Criando uma API REST conectada a Amazon RDS com Java
- Criando um microsserviço de upload de imagens com a amazon S3
- Java spring com rabbitMQ

##### Percurso:

Aula 1. Pensamento computacional
Aula 2. Introdução à lógica da programação
Aula 3. Fundamentos de algoritmos
Aula 4. Linguagens de programação
Aula 5. Primeiro contato com a programação

---

Área da computação: infinidade de aplicações e mudanças a todo tempo.

#### Introdução

Objetivo da aula: aprender como pensar computacionalmente
Etapa 1: Introdução ao pensamento computacional
Etapa 2: Habilidades complementares
Etapa 3: Pilares: Decomposição
Etapa 4: Pilares: Padrões → Uma área interessante da parte de pesquisa também
Etapa 5: Pilares: Abstração
Etapa 6: Pilares: Algoritmos
Etapa 7: Estudo de caso conceitual: perdido
Etapa 8: Estudo de caso aplicado: Soma de um intervalo
Etapa 9: Estudo de caso aplicado: Adivinhe um número

##### Overview

Pensamento computacional?

```ad-danger
Processo de pensamento envolvido na expressão de soluções em passos computacionais ou algoritmos que podem ser implementados no computador. (Aho, 2011; Lee, 2016)
```

"Quando a gente escreve a gente tira o que está na memória RAM e passa para o HD"

Pensamento computacional:

- Definição de passos de como chegar em um problema
- Sistemático e eficiente
- Sejam capazes de resolver: humanos e máquinas
- Habilidade generalista: Matemática, leitura, escrita (não é uma disciplina acadêmica)

O pensamento computacional é baseado em 4 pilares:

- **Decomposição.** Exemplo: receita de bolo, busca binária, quebra cabeça.
- **Reconhecimento de padrões.** Identificar padrões ou tendências. Similaridades e diferenças entre os problemas. Exemplos: padrão comportamental (bolsa de valores).
- **Abstração**. Extrapolar o conceito do problema para uma forma generalista.
- **Design de algoritmos**. Automatizar: definir passo a passo a solução do problema. (Mão na massa)
  (Dividir um problema complexo em subproblemas)

##### Overview

Computação:

- Processo contínuo
- Definir uma solução
- Testar a solução
- Aperfeiçoamento da solução encontrada.

![[../Files/Pasted image 20220613184621.png]]

![[../Files/Pasted image 20220613184636.png]]

Outros dois pilares bônus de computação:

- Raciocínio lógico
- Refinamento

![[../Files/Pasted image 20220613184816.png]]

Exemplos de aplicação da computação:

- Química: Aperfeiçoamento de reações químicas pela utilização de algoritmos, através da identificação de químicos
- Engenharia: Simulações de aeronaves executadas via software em detrimento de túnel de vento
- Biologia: Modelagem e mapeamento do genoma humano
- Computação: Simulação de problemas de alta ordem em supercomputadores

(Santos Dummond: Supercomputador dentro do LNCC)

Competências:

- Pensamento sistemático
- Colaboração dentro da equipe
- Criatividade e design
- Facilitador

#### Habilidade complementares

Habilidades complementares:

- Raciocínio Lógico
- Aperfeiçoamento

**Raciocínio lógico** é uma forma de pensamento estruturado, ou raciocínio, que permite encontrar a conclusão ou determinar a resolução de um problema.

O raciocínio lógico é necessário ser treinado, não só passado.

Raciocínio lógico, classificação:

- Indução: a partir de um fenômeno observado você induz que algo acontece. Exemplo: ciências experimentais, empirismo
- Dedução: a partir de leis e teorias você induz explicações para determinados fenômenos. Exemplo: ciências exatas (dedução de problemas matemáticos a partir de outros axiomas ou teoremas)
- Abdução: A partir da conclusão você tira a premissa. Exemplo: A grama está molhada, logo deve ter chovido. Exemplo: processo investigativo: diagnósticos médicos, detetives.

````ad-example
"Caixinhas" de classificação do raciocínio lógico:
```
Inferência:
	Sintética:
		Abdução
		Indução
	Analítica:
		Dedução
```
````

**Aperfeiçoamento**: A partir de uma solução determinar pontos de melhora e refinamento.
Sinônimos: Melhoramento, aprimoramento, ato de aperfeiçoar, refinamento

Aperfeiçoamento:

1. Encontrar solução eficiente
2. Otimizar processos
3. Simplificar linhas de códigos
4. Funções bem definidas

````ad-note
```ad-quote
1 e 2: Melhor uso de recursos
```
```ad-quote
3 e 4: Melhorar códigos e algoritmos
```
````

#### Pilares: Decomposição

````ad-danger
If you can't solve a problem, then there is an easier problem that you can solve: find it

```bash
- George Polya - professor e matemático
```

````

Primeiro passo da resolução de problemas dentro do conceito de pensamento computacional é: "Dado um problema complexo, devemos quebrá-lo em problemas menores. Portanto, problemas mais fáceis e gerenciáveis".

##### Estratégia

###### Análise

Processo de quebrar e determinar partes menores e gerenciáveis:

- Estudar, explorar
- realizar exame detalhado
- Decompor em elementos constituintes

###### Síntese

Combinar os elementos recompondo o problema original. (As peças precisam fazer sentido para se encaixarem)

- Processo de reconstrução
- Fundir os elementos de maneira coerente
- Conside tem reunir elementos distintos em um único elemento

---

Ordem de execução de tarefas menores:

- Sequência: dependência entre tarefas executadas. Ex: fila
- Paralelismo: Tarefas podem ser executadas concomitantemente. (+ eficiência - tempo)

Dentro da decomposição nós temos as variáveis, problemas pequenos e a segmentação.

- Não basta aplicar, precisa-se treinar-se
- Desenvolver a decomposição "by yourself"
- **Maneiras distintas de decompor o mesmo problema**

##### Como decompor?

1. Identificar ou coletar dados
2. Agregar os dados
3. Funcionalidade

##### Exemplos

Ex do cotidiano: cozinhar

- Identificar os ingredientes
- Determinas as etapas (sequencial ou paralelo)
- Executar cada etapa
- Agregar os ingredientes para finalizar (recompor com coerência)
  Ex do cotidiano: funcionamento de uma bike
- Identificar os componentes
- Papel de cada componente
- Indeterdependência das peças

Exemplo: criar um app

- Finalidade
- Interface
- Funcionalidades
- Pré-requisitos

(Definição de componentes e etapas)
Desenvolvimento mais eficiente

Exemplo: artigo

- O que será abordado?
- Estrutura
- Conteúdo de cada tópico
- Textos de conexão
  (Definição de componentes e etapas)
  (Sequencial ou paralelo, em ordem ou não)

Exemplo: movimentos de um avatar
![[../Files/Pasted image 20220613191609.png]]

Importante disso é: otimiza linhas de código, não repete e abstrai melhor o problema

#### Pilares: Padrões

Reconhecimento de padrões:

- Modelo base
- Estrutrura invarianete
- Repetição
  A partir de modelos encontrar um modelo de referência que não muda
  Detecção de similariades e diferenças

Exemplo: fotos de redes sociais

1. Imagens de diferentes tamanhos
2. Compressão padronizada
3. Salvar no banco de dados

Exemplo: compressão de dados
![[../Files/Pasted image 20220613191843.png]]

Exemplo: detecção entre seres vivos. Ou frutas ou doces

Por que determinar padrões?
Generalizar, com objetivo de obter resolução para problemas diferentes

A generalização feita ao encontrar um padrão em um aplicativo é importante pois assim podemos aplicar uma solução para um determinado problema em vários outros problemas similares daquele mesmo padrão.

- Classes
- Categorias: Tipo de mídia, dependem do domínio

COmo que um ser humano faz isso?

1. Grau de similaridade
2. Grupos conhecidos x objeto desconhecido

Como o computador reconhece padrões?

1. Representação de atributos
2. Aprendizado - conceito associado ao objeto
3. Armazenar dados
4. Regras de decisão

Em resumo a detecção de padrões é:

- Extração de características
- Classificação de dados
- Aplicação a diferentes contextos (métodos ou aplicações)

Exemplos de aplicações que utilizam padrões:

- Classificação de dados
- Reconhecimento de imagem
- Reconhecimento de fala (tradução de línguas)
- Análise de cenas
- Classificação de documentos

Áreas do conhecimento da computação que esses padrões fazem uso:

- Machine Learning
- Redes Neurais
- Inteligência artificial
- Ciência de dados

#### Pilares: Abstração

O que é abstrair? Observar, um ou mais elementos, avaliando características e propriedades em separado
Abstração: processo intelectual de isolamento de um objeto da realidade
Generalizar: Tornar-se geral, mais amplo, extensão

Generalização, na lógica, é a operação intelectual que consiste em reunir uma classe geral, um conjunto de fenômenos similares

Como classificar dados?

- Características
- Pontos essenciais
- Generalizar x detalhar

```ad-warning
As vezes um objeto tem várias características que não são interessantes para aquela análise.

![[../Files/Pasted image 20220613192754.png]]
![[../Files/Pasted image 20220613192801.png]]

```

Abstração é utilizada em diversas áreas do conhecimento. Alguns exemplos de abstração em computação são:

- Algoritmos
  - Merge sort
  - Clustering
  - Busca binária
- Estruturas de dados:
  - árvores
  - lista
  - grafos
- Máquinas de estado finito
- As próprias linguagens de programação

Conceitos baseados em abstrações:

- Comunicação (entre pessoas, síncrona ou assíncrona, entre componentes de hardware)
- Arquiteturas (cliente e servidor, estrutura de camadas (modelo OS), arquitetura P2P (ponto a ponto))

```ad-example
Exemplo de problema
Por onde começar a limpar o terreno?
- Classificar? Não
- Determinar as distâncias? Sim
- Estender para outros cenários
![[../Files/Pasted image 20220613193407.png]]
```

#### Pilares: algoritmos

O computador não opera sozinho, ele precisa de instruções detalhadas que são descritas dentro dos programas.

Os programas são constituidos pelas intruções que possuem o passo a passo para resolver um problema.

Nesse sentido, algoritmos são um processo de resolução de problemas "step by step" utilizando instruções.

- O que precisa ser feito?
- Qual a ordem de execução?
- Entendimento por humano e máquina

Desenvolvimento do programa

- Instruções detalhadas
- Algoritmo
- Programa

O algoritmo é codificado de acordo com a linguagem de programação escolhida.

```ad-note
Em resumo um algoritmo é:
- Sequência de passos com objetivo definido
- Execução de tarefas específicas
- Conjunto de operações que resultam em uma sucessão finita de ações
```

Exemplos de algoritmo: preparar um saduíche, trocar uma lâmpada, trajeto ao trabalho, fazer uma receita de bolo

Como construir um algoritmo?

1. Compreensão do problema
2. Definição de dados de entrada
3. Definir o processamento
4. Definir dados de saída
5. Utilizar um método de construção
6. Teste e diagnóstico
   (Construção e refinamento de algoritmo)

Tipos de construção de algoritmos no-code:

- Narrativa - Utilização de linguagem natural
- Fluxograma - Utilização de símbolos pré-definidos
- Pseudocódigo - Portugol

Exemplo: Multiplicação de dois números
Narrativa:

1. Receber os valores
2. Multiplicar
3. Imprimir resultado

Fluxograma:
![[../Files/Pasted image 20220613194204.png]]

Exemplo: Média dos alunos
Narrativa:

1. Receber os valores
2. Imprimir resultado
3. Conferir regra de aprovação
4. Imprima o resultado
   ![[../Files/Pasted image 20220613194307.png]]

Em resumo: Algoritmo é um passo a passo de definição de tarefas para resolver um problema.

#### Estudo de caso conceitual: perdido

Suponha: pessoa perdida na floresta.
Como resolver o problema utilizando o pensamento computacional de forma a maximizar a sobrevivência da pessoa?

- Identificar mecanismos
- Recursos comuns
- Detalhes mais importantes

- Sobrevivência
  - Água
    - Chuva
    - Nascente
  - Comida
    - Coletar
    - Caçar
      - Fogo
  - Abrigo
    - Localização
      - Mapa
    - Proteção
      - Fogo
      - Lança
    - Quente e seco
      - Fogo

![[../Files/Pasted image 20220614224431.png]]

O mapa pode ser criado por abstração.

O que utilizamos até aqui:

- Decomposição
- Reconhecimento de padrões
- Abstração

Agora vamos determinar as instruções para a pessoa cozinhar
Preparando a comida:

- Pegar o peixe
- Colocar água na panela
- Fever a água
- Limpar o peixe
- Fazer o cozido
- Assar o filé

![[../Files/Pasted image 20220614224652.png]]

(Há paralelismo entre colocar água na panela e ferver a água)

Esse é o mesmo processo para:

- Encontrar água
- Construir abrigo
- Maximizar chances de resgate

#### Estudo de caso aplicado: soma de um intervalo

Ex: soma numérica entre 1 e 200

Primeira ideia:
Ir apenas somando:
1+2+3+4+5+6+7...

Outra forma mais eficiente de fazer isso:
Coloquemos os números na seguinte ordem:
200 + 1
199 + 2
198 + 3
197 + 4
...

200 + 1 = 201
199 + 2 = 201
198 + 3 = 201
197 + 4 = 201
...
_Padrão encontrado_

Como expressar de forma generalista agora?
Utilizando abstração

O valor vai se repetir quantas vezes?
Já que estamos usando dois números em cada soma, o valor será dividido por 2.
Dessa forma:
$$\frac{200}2 = 100$$$$201\times100 = 20100$$
Como expressar em variáveis agora?

Soma de n° entre x e y
(1 e 200)

```ad-warning
$$y+x = \text{resultado parcial}$$
$$(y-1) + (x+1) = \text{resultado parcial}$$
$$\text{total}\times\text{resultado parcial}=\text{resultado}$$
```

Algoritmo:
Passo 1 - Recebe os valores (x e y)
Passo 2 - Resolva: y/2 = total
Passo 3 - Resolva: x+y = resultado_parcial
Passo 4 - Ache o total: Final = total x resultado_parcial
Passo 5 - Imprima o resultado

#### Estudo de caso aplicado: Adivinhe um número

Ex: adivinhe o número

O problema consiste em determinar o número escolhido por uma dentro de um intervalo.
Perguntas com respostas de sim e não apenas.

Ex:
O número é 1?
O número é 2?
O número é 3?
_Ineficiente_

P: O número é maior que 50?
R: Não
P: O número é menor que 20?
R: Sim.
_Ex: Busca binária_

Algoritmo busca binária:
Passo 1 - Ordenar o vetor
Passo 2 - Módulo de L/2
Passo 3 - Acessar estrutura
Passo 4 - Comparar valores
Passo 5 - Repita até encontrar o número
Passo 6 - Imprima "Busca bem sucedida"

Como aprimorar essa habilidade?
"_Permitindo que seus alunos expliquem suas decisões e seu processo de desenvolvimento" (Brennan & Renesck)_

### 2 Introdução à lógica de programação

#### O que é lógica?

Esta aula foca em apresentar o conceito de lógica aplicada à programação, como um processo de pensamento atrelado ao conceito de algoritmos e resolução de problemas.

Problema:

- Questão
- Numerosas soluções
- Objeto de questão
- Proposta duvidosa

Definição formal de problema: "Problema é uma questão que foge a uma determinada regra, ou melhor é um desvio de percurso, o qual impede de atingir um objetivo com eficiencia e eficácia."

O que é a lógica?
Definição formal de lógica: "Parte da filosofia que trata das formas do pensamento em geral (Dedução, indução, hipótese, inferência etc.) e das operações intelectuais que visam à determinação do que é verdadeiro ou não."

Lógica:

- Forma como desencadeiam acontecimentos
- Organização coesa
- Forma de raciocínio
- Ordenação que segue convenções

Definição mais informal de lógica: "Organização e planejamento das instruções, assertivas em um algoritmo, a fim de viabilizar a implantação de um programa."

Como essa definição se aplica no cotidiano?

1. Tem-se uma sequência de instruções
2. Baseadas em ações
3. Juntam e criam uma ação maior

Seres humanos podem prever comportamentos, computadores não.
_Precisam de instruções detalhadas._

```ad-quote
"Everybody in this country should learn how to program a computer because it teaches you how to think." - Steve Jobs
```

#### Técnica de lógica de programação

Técnicas:

_Exemplo - construção de um prédio_
Ordem de instruções:

1. Planta baixa - Realizado pelo arquiteto
2. Projeto - Realizado pelo engenheiro
3. Planejamento - Financeiro para determinar a viabilidade do projeto

##### Técnica linear

- Modelo tradicional
- Não tem vínculo

  - Estrutura hierárquica
  - Programação de computadores

- Técnica linear: - Execução sequênciada - Recursos limitados - Única dimensão
  _Ordenação de elementos por uma única propriedade_

Exemplo do dia a dia de técnica linear

1. Acordar
2. Descer as escadas
3. Preparar café
4. Ler café
   _Execução sequenciada_

##### Técnica estruturada

Organização, disposição e ordem dos elementos essenciais que compõem um corpo (concreto ou abstrato).
_Modelos de desenvolvimento ou abstração._

- Objetivo:
  - Escrita
    - Programas
  - Entendimento
  - Validação
  - Manutenção
    - Facilitar

Exemplo:
![[../Files/Pasted image 20220614231304.png]]
_Há uma escolha_

##### Técnica modular

Definição de partes independentes que são controladas por um conjunto de regras
_Modelos de desenvolvimento e resolução._

![[../Files/Pasted image 20220614231401.png]]

- Metas
  - Simplificação
  - Decompor o problema
  - Verificação do módulo

Exemplo do dia a dia:
![[../Files/Pasted image 20220614231455.png]]

### 3 Fundamentos de algoritmos

Nesta aula serão apresentados os conceitos básicos para o correto entendimento de algoritmos. Esses conceitos como, variáveis, tipos de dados, instruções, condições, entre outros temas relacionados.

#### Tipologia e variáveis

Qual é a função do computador?
É processar as informações que passamos para ele
TIpos de informação:

- Dados → Tratados e processados
  - Numéricos
    - Inteiros: 0, 1, 50, 600
    - Reais: 5.95, -8.8
  - Caracteres
    - "Programação"
    - "Fonte: (25)99856-5741"
    - "KU\*&NH"
  - Lógicos
    - Verdadeiro: 1
    - Falos: 0
- Instruções
  - Operações que processam dos dados

O que é uma variável? Espaço na memória para guardar um tipo de dado.

- Mutável
- Possui variações
- Incerto
- Inconstante
- Instável

Variável - pode assumir qualquer um dos valores de um determinado conjunto de valores

É como uma caixinha para receber um tipo de dados
![[../Files/Pasted image 20220712124205.png]]

Nome da variável
Regras:

- Atribuição de um ou mais caracteres
- Primeira letra não número
- Sem espaços em branco
- Vedado (Não Utilização de palavras reservadas)
- Caracteres e números

Variável:

- Ação: modificação de dados
- Controle: vigiada, controle

Constante: Variável constante

- Inalterável
- O que não muda
- Invariável

#### Instruções primitivas

Cálculo matemáticos

- Variáveis
- Constantes

Usamos os operadores que podem ser tanto:

- Binários
- Unários

![[../Files/Pasted image 20220712124457.png]]

Exemplo: $Área  = \pi·raio²$

Definição formal de instruções primitivas:
Instruções são linguagem de palavras-chave (vocabulário) de uma determinada linguagem de programação que tem por finalidade comandar um computador que irá tratar os dados

![[../Files/Pasted image 20220712124732.png]]

Exemplo, média escolar:

```Portugol
Início programa:
	Nota1 = 5                        // Variável
	Nota = 8
	Resultado = 0

	Resultado = (Nota1 + Nota2)/2    // Constante
	Escreva resultado
Fim programa
Saída:
	6.5
```

#### Estruturas condicionais e operadores

**Condição:**
Estado de uma pessoa ou coisa
**Condicional:**
Que expressa uma condição ou suposição
Contém ou implica uma suposição ou hipótese

Qual a ideia de uma estrutura condicional?
Caso uma expressão seja satisfeita, fazer um conjunto de instruções.

![[../Files/Pasted image 20220712125040.png]]

Operadores relacionais
![[../Files/Pasted image 20220712125050.png]]

Condicional simples
![[../Files/Pasted image 20220712125132.png]]

Condicional Composta
![[../Files/Pasted image 20220712125305.png]]

Operadores lógicos:
Quando utilizar? Quando precisamos de valores lógicos (verdadeiro ou falso)

- AND
- OR
- NOT

#### Estruturas de repetição

- Laços
- Controle de fluxo
- Malhas de repetição
- Repetição
- Loop

Há uma condição de parada

- Número de repetições pré-fixada
- Condição a ser satisfeita

Finalidade

- Redução de linhas
- Compreensão facilitada
- Redução de erro

Estruturas:

- Enquanto ... faça
- Repita ... até
- Para ... de ... até ... faça

##### Exemplos

Teste lógico

- Início
  Numero de repetições
- Indefinidas

![[../Files/Pasted image 20220712130015.png]]

Artigo
![[../Files/Pasted image 20220712130048.png]]

![[../Files/Pasted image 20220712130112.png]]

#### Vetores e matrizes

Vetor: Sequência de dados de um determinado tipo

Um vetor é caracterizado por uma variável dimensionada com um tamanho pré-fixado

- Container
- Matriz unidimensional

Matriz: Matriz é uma tabela organizada em linhas e colunas no formato m x n, onde m representa o número de linhas (horizontal) e n o número de colunas (vertical)

- Coleção de variável
- Contíguas em memória
- Índices
  ![[../Files/Pasted image 20220712130410.png]]

Exemplo de utilização: colocar notas de um aluno dentro de um vetor.
Exemplo de utilização: matrizes com notas dos alunos
![[../Files/Pasted image 20220712130709.png]]

#### O que são funções?

Sinônimos

- Subalgortimo
- Função
- Bloco
- Subprograma
- Método
- Sub-rotina

Definição formal: As funções, ou sub-rotinas são blocos de instruções que realizam tarefas específicas.

Finalidade:

- Modularização do programa
- Código mais claro e conciso
- Reutilização de instruções

São identificados por nomes e parâmetros

- Definição
- Nome
- Invocação
- Variável local: São destruídas ao encerrar a função

Exemplo: Média escolar
![[../Files/Pasted image 20220712131055.png]]

#### Instruções de entrada/saída

![[../Files/Pasted image 20220712131207.png]]

Definição formal de entrada de dados:
Consiste na inserção e recebimento de dados do mundo real por meio de ação de alguma interface, seja teclado, mouse, arquivos, entre outros.
Exemplos de inserção de dados
![[../Files/Pasted image 20220712131256.png]]

Definição formal de saída de dados:
Consiste na impressão dos dados do mundo abstrato, digital por meio de ação de alguma interface

Os formatos podem variar desde simples arquivos binários até complexas querys de banco de dados.

![[../Files/Pasted image 20220712131351.png]]

Tipos de saída

- Saída programada
- Saída por interrupção (saída por periféricos normalmente)

Casos de saída

- Bem sucedida
- Erro de sintaxe ou outro
- Erros de programação
- Problemas com a interface

### 4 Linguagens de programação

O objetivo desta aula é apresentar os paradigmas de programação existentes, incluindo o conceito em si. As linguagens de programação são baseadas em um ou mais paradigmas, sendo o último caso conhecido como linguagem multiparadigma.

#### Introdução à linguagens de programação

Por que falar de história da computação?

- Compreender as dificuldades enfrentadas
- Fundamentos da computação
- O processo de pensamento
  São baseadas em pesquisas anteriores;
  Novos paradigmas.
  Evolui de hardware para software.

Cronologia
![[../Files/Pasted image 20220712131746.png]]

![[../Files/Pasted image 20220712132213.png]]

![[../Files/Pasted image 20220712132229.png]]
![[../Files/Pasted image 20220712132321.png]]
![[../Files/Pasted image 20220712132351.png]]
![[../Files/Pasted image 20220712132428.png]]

![[../Files/Pasted image 20220712132455.png]]
![[../Files/Pasted image 20220712132528.png]]

Problemas computacionais

- Objeto de discussão que possui instruções passo a passo que são mais facilmente resolvíveis em ambiente computacional
  - Problemas de decisão
  - Problemas de busca
  - Problemas de otimização

Exemplo de problema de decisão:
Determinar se um número é primo

Problema de busca:
Ex: clique: Dada uma rede, saber se um ponto está conectado a 3 outros em um grafo.

Problemas de otimização:

- Maximizar uma função
  O que é uma linguagem de programação?
  Método padronizado composto por um conjunto de regras sintáticas e semânticas de implementação de um **código fonte**: Conjunto de palavras com regras

Código fonte:

- Tradução
- Interpretação

#### Como um computador entende o programa?

Pelo código fonte com:

- Tradução (ou)
- Interpretação

Um programa é um amontoado de palavras senão for possível que o computador.

Processo de tradução → Compilador: Executa análise do programa

O programa fonte é traduzido para um programa objeto em linguagem de máquina,

Tradução:

1. Geração do programa objeto
2. Execução do programa objeto

Interpretação:

1. Programa fonte executado diretamente

![[../Files/Pasted image 20220712192823.png]]

![[../Files/Pasted image 20220712192840.png]]

```ad-warning
Python é uma linguagem interpretada
```

Tradução:

- Execução mais rápida
- Programas menores

Interpretação

- Maior flexibilidade

Conceito de transpilação: Jogar o código de uma linguagem de alto nível para uma outra de alto nível. Exemplo: Typescript é transpilado para o Javascript

#### Características de um programa

Existem boas práticas?
SIm

Desenvolvimento de programas, diretrizes:

- Legibilidade
- Redigibilidade
- Confiabilidade
- Custo

Legibilidade:
(Estado que é legível)

- Facilidade de leitura
- Compreensão
- Ortogonalidade
- Definição adequada das estruturas: Coerência nas instruções

Redigibilidade
(Facilidade de escrita de código)

- Pode conflitar com a legibilidade
- Ortogonalidade
- Simplicidade da escrita: Coerência nas instruções
- Suporte à abstração
- Reuso do código
- Expressividade
  - Exemplo:
    - Operador ++
    - Uso do for

Confiabilidade
(Faz o que foi programado para fazer)

- Verificação de tipos
- Trata exceções
- Uso de ponteiros
- Compatibilidade entre compiladores

Custo
(Análise de impacto)

- Treinamento
- Codificação
- Compilação
- Execução
- Infra-estrutrura
  - Exemplo: adaptação para outros computadores
    - Super computador: Santos Dummond

Outras características

- Atualizações
- Uso para IA
- Disponibilidade de ferramentas
- Comunidade ativa
- Adoção pelo mercado

#### Análises de código

Análises:
![[../Files/Pasted image 20220712193644.png]]

##### Análise léxica

Objetivos

- Particionar
  - Identificar os elementos léxicos (denominados tokens) e agrupá-los.
- Classificar
  - Elementos: identificadores, palavras reservadas, números, strings
- Eliminar
  - Elementos: Caracteres de espaços em branco, comentários, ...

##### Análise sintática

Sintaxe é o componente do sistema linguístico que interliga os constituintes da sentença, atribuindo-lhe uma estrutura.
(Corretude do programa).

Padrão - gramática:

- Depende da linguagem utilizada

##### Análise semântica

Semântica é o estudo do significado. Incide sobre a relação entre significantes, como: palavras, frases, sinais e símbolos.
(Lógica do programa)

````ad-example
Erro de semântica:
	- Não faz o que é esperado

# Errado
![[../Files/Pasted image 20220712194146.png]]

# Certo
![[../Files/Pasted image 20220712194225.png]]


```ad-danger
O erro de semântica é bem mais difícil de encontrar que o erro de sintaxe, tendo que debugar linha a linha para ver o que está aconecendo no programa.
```
````

#### Paradigmas de programação

O que é um paradigma?
Forma de resolução de problemas com diretrizes e limitações específicas de cada paradigma utilizando linguagem de programação.

Classificação:

- Orientação a objeto
- Procedural: Chamadas sucessivas e procedimentos separados
- Funcional: Instruções são baseadas em funções
- Estruturado: Estrutura de blocos aninhados
- Computação distribuída: Funções executadas de forma independente
- Lógico
  ![[../Files/Pasted image 20220712194546.png]]

##### Paradigma estruturado

Conceitos:

- Sequência
- Decisão → Relacionado a teste lógico
- Iteração → Relacionado a funções, laços, condições
  (Ênfase em sequência)

Utilização:

- Problemas simples e diretos
- Aprender programação
  POO ainda não é compreendida por muitos

```C
function fatorial(x) {
	if(x > 1){
		return x*fatorial(x-1);
	}
	return 1;
}
```

##### Orientação a Objeto

Paradigma de programação baseado na utilização de objetos e suas interações
Análogo ao mundo real

O que é um objeto?

- Violão
- Robô
- Animal
- Mulher
- Bolo
- Etc

Um objeto é descrito por características específicas, comportamentos e estado.

- O que tenho
- O que sou capaz de fazer
- Como faço

Exemplo: Caneta

- O que tenho
  - Modelo
  - Carga
  - Cor
  - Corpo
  - Tampa
  - Ponta
- O que sou capaz de fazer
  - Escrever
  - Desenhar
  - Rabiscar
  - Pintar
  - Destampar
- Como faço (estados)

  - Tampada
  - Destampada
  - Em uso

- O que eu tenho → Atributos
- Sou capaz de fazer → Métodos
- Como faço → Estados

Ponto de vista da programação, o que é um objeto?

- POO: Classe
  - Alocação em memória
  - Operações associadas
- Estruturada: Variável
  - Alocação em memória
  - Operações associadas

![[../Files/Pasted image 20220712195346.png]]

Pilares de orientação a objeto:

- Herança
- Encapsulamento
- Polimorfismo
- Abstração

##### Herança

Uma classe filha herda atributos de uma classe mãe
![[../Files/Pasted image 20220712195447.png]]

---

O que é interessante da orientação à objeto?

- Reuso de código

O que é interessante da programação estruturada?

- Problemas específicos e diretos

Fica a cargo do programador decidir qual é o paradigma mais adequado para o contexto.

### 5 Primeiro contato com a programação

#### Algoritmos em portugol

```Portugol
programa {
	funcao inicio() {
		inteiro x, y
		escreva ("Digite os números para executar a soma do intervalo: ")
		leia(x)
		leia(y)
		escreva(soma_intervalo(x, y))
	}

	funcao inteiro soma_intervalo(inteiro x, inteiro y) {
		inteiro total, resultado_parcial
		total = y/2
		resultado_parcial = y + x
		inteiro resultado = total * resultado_parcial
		retorne resultado
	}
}
```

```portugol
programa{
	funcao inicio() {
		real a, b, nota_a, nota_b
		escreva("Digite a nota p1 e p2 do aluno A: ")
		leia(a)
		leia(b)
		escreva("Digite a nota p1 e p2 do aluno B: ")
		leia(nota_a)
		leia(nota_b)

		escreva("Média do aluno A: ", media_aluno(a, b))
		escreva("Média do aluno B: ", media_aluno(nota_a, nota_b))
	}

	funcao real media_aluno(real nota_a, real nota_b){
		retorne (nota_a + nota_b) / 2
	}
}
```

#### Considerações finais

Referências

Computional Thinking
https://www.cs.cmu.edu/~CompThink/resources/TheLinkWing.pdf
https://ubiquity.acm.org/article.cfm?id=1922682
https://www.youtube.com/watch?v=YVEUOHw3Qb8
https://simplificandoredes.com/historia-da-computacao/
https://simplificandoredes.com/pensamento-computacional/

Programação e algoritmos
http://www.inf.ufes.br/~tavares/labcomp2000/aulas.htm
https://www.dca.fee.unicamp.br/cursos/EA876/apostila/HTML/
http://www.inf.ufes.br/~tavares/labcomp2000/aula1.html

Algoritmos
Livros: Fundamentos da programação de computadores - Pearson
https://www.youtube.com/watch?v=HtSuA80QTyo
Algoritmos - MIT
José Augusto Manzano, Algoritmos - Lógica para desenvolvimento de programação de computadores, Ed. Érica, 17a ed. (ou mais recente) - livro de referência

Ana Fernandes
Ascencio, Fundamentos da programação de computadores - algoritmo Pascal, C/C e Java, Ed. Pearson, 2a ed.

Andrew S. Tanenbaum, "Livro Organização Estruturada de Computadores", Ed. Pearson, 5a edição -- Capítulo 1

The Formal Semantics of Programming Languages, Glynn Winskel Deitel e Deitel, "C++ How to Program", 5th edition, Editora Prentice Hall, 2005 -- Capítulo 1

Waldermar Celes, Renato Cerqueira e José Lucas Rangel, "Introdução a Estrutura de Dados com Técnica de Programação em C", Editora Campus-Elsevier, 2004 -- Capítulo 1
