# Módulo 1 - Instalação e Primeiros Passos no R


## Introdução

Aprender R é como aprender um novo idioma: no início parece artificial, mas torna-se natural com a prática! Se este é o seu primeiro contato com R, é normal achar estranho. 
Muitos biólogos nunca utilizaram uma linguagem de programação. Abrir o R ou o RStudio pela primeira vez e ver uma tela em branco com um cursor esperando comandos às vezes pode ser um pouco assustador.

O objetivo deste módulo é apresentar o ambiente do R, instalar corretamente os programas necessários e executar seus primeiros comandos!


## O que é R?

R é uma linguagem de programação e ambiente computacional voltado para análise estatística, manipulação de dados, visualização gráfica e modelagem. Na Biologia, R é amplamente utilizado em Ecologia, Evolução, Genética, Sistemática, Conservação, Bioestatística, dentre outras áreas.

É possível usar o R sozinho, mas, como estamos começando, vamos usar o RStudio! Ele oferece uma interface muito mais amigável e intuitiva. 


## O que é RStudio?

RStudio é uma interface gráfica para facilitar o uso do R.

Além de organizar tudo em uma única tela, ele integra ferramentas e pacotes que facilitam a visualização de gráficos, a organização de arquivos e o gerenciamento do console, tornando o aprendizado bem mais leve e produtivo.

Fazendo uma analogia, é como se o R fosse um idioma (como Português ou Inglês), e o RStudio fosse o editor de texto (como o Microsoft Word ou o bloco de notas)!


## Instalação

### Instalar o R

Acesse: https://cran.r-project.org/

Escolha seu sistema operacional e siga a instalação padrão.

### Instalar o RStudio

Acesse: https://posit.co/download/rstudio-desktop/

Baixe a versão gratuita Desktop.

Abra os dois programas. Como vamos utilizar apenas o RStudio, não precisamos manter o R aberto. Entretanto, relembre que o RStudio não funciona sem o R, então não desinstale-o!
Você deverá encontrar estas interfaces:


<img width="1918" height="1013" alt="image" src="https://github.com/user-attachments/assets/eb66c730-4f05-4c94-9500-127a5051b4f2" />
<img width="1918" height="1013" alt="image" src="https://github.com/user-attachments/assets/36510210-4670-42aa-a4f5-11d903ecf3a5" />

```diff
+ Se alguma das áreas não estiver sendo visualizada no RStudio, siga: View (canto superior esquerdo) → Panes → Show All Panes.
```


## Interface do RStudio

Em geral, o RStudio é dividido em quatro áreas principais. Verifique-as no seu programa conforme elas são mencionadas aqui.

No canto superior esquerdo fica o editor de <b>scripts</b>. Esse espaço pode ser entendido como o local em que você escreve seu trabalho de forma organizada. Em vez de digitar comandos soltos e esquecê-los depois, você registra tudo em um arquivo que pode ser salvo, revisado e reutilizado futuramente. Para estudantes e pesquisadores, essa é a maneira mais recomendada de trabalhar, pois permite repetir análises e manter um histórico claro do que foi feito.

No canto inferior esquerdo normalmente está o <b>console</b>. O console é a área em que o R executa comandos diretamente. Sempre que você envia uma linha de código, é ali que o resultado aparece. Pode-se pensar no console como uma conversa imediata com o programa: você faz uma solicitação e o R responde. Esse espaço é muito útil para testes rápidos, cálculos simples ou verificações momentâneas. Ainda assim, conforme o uso avança, o ideal é que os comandos principais sejam escritos no script e apenas executados pelo console.

No canto superior direito costuma aparecer o painel chamado <b>Environment</b>. Ele mostra os objetos criados durante a sessão. Objetos são elementos armazenados pelo R, como números, vetores, tabelas ou resultados de análises. Sempre que você cria algo e dá um nome a esse conteúdo, ele pode aparecer nesse painel. Isso ajuda a visualizar o que já está disponível no ambiente de trabalho e evita que você se perca entre diferentes variáveis.

Na parte inferior direita há um conjunto de abas bastante úteis. Entre elas, a aba <b>Files</b> permite navegar pelas pastas do computador e localizar arquivos do projeto. A aba <b>Plots</b> exibe gráficos produzidos durante a sessão. A aba <b>Packages</b> mostra extensões instaladas no R, conhecidas como pacotes, que ampliam as funções disponíveis no programa. Já a aba <b>Help</b> oferece documentação e explicações sobre funções específicas, sendo uma ferramenta valiosa para consulta constante.

A interface do RStudio foi pensada para reunir em um só lugar tudo o que normalmente seria necessário durante uma análise. Você escreve no script, executa no console, acompanha os objetos no Environment, observa gráficos no painel lateral e consulta ajuda quando necessário. Esse fluxo torna o trabalho mais eficiente e organizado!


## Criando um script

Crie um script novo seguindo:

<b>File → New File → R Script</b>

A partir daí, você pode escrever comandos linha por linha no painel superior esquerdo.

Atalho:

<b>Ctrl + Shift + N</b>

Os atalhos existem para tornar o trabalho no RStudio mais rápido, fluido e eficiente. Como o uso de R envolve escrever, testar, corrigir e executar comandos constantemente, depender apenas do mouse para cada ação tornaria o processo lento e repetitivo. Em vez de clicar em menus toda vez que quiser rodar uma linha de código, salvar um arquivo ou limpar o console, um simples comando no teclado realiza a mesma tarefa em segundos.

No caso da execução de código, por exemplo, você frequentemente escreve uma linha, testa o resultado, ajusta algo e executa novamente. Se precisasse mover a mão até o mouse e clicar em “Run” centenas de vezes ao longo do estudo ou de uma análise, isso interromperia o ritmo de trabalho. O atalho permite continuar digitando e testando quase sem pausa, mantendo a concentração.


## Primeiro código

Uma das maneiras mais comuns de começar é usando o R como uma calculadora. Quando você digita uma operação matemática básica e executa, o programa interpreta aquela expressão e devolve o resultado imediatamente no console.

```r
2 + 2
```

Execute com Ctrl + Enter ou clique em "Run". Você deverá ver o resultado aparecer no console.


## Operações matemáticas

Esses cálculos iniciais também mostram que o R segue as regras matemáticas tradicionais. Multiplicações e divisões costumam ser resolvidas antes de somas e subtrações, e os parênteses servem para definir prioridades.

```r
2 + 3
5 - 1
4 * 6
10 / 2
2 ^ 3
```

Experimente diferentes operações matemáticas. 

Isso é importante porque, no futuro, você poderá escrever expressões mais complexas para fórmulas estatísticas, transformações de dados ou cálculos biológicos sem precisar fazer tudo manualmente.


## Rodar script

Ao executar diferentes operações matemáticas, você deve ter percebido que Ctrl + Enter ou "Run" executa apenas a linha de código que o cursor está indicando.

Há diferentes atalhos e modos de facilitar a execução do script:

| Função | Atalho | Manual |
| -------- | -------- | -------- |
| Rodar linha atual | Ctrl + Enter | Clique em "Run" |
| Rodar uma seleção | Selecione as linhas desejadas (com o mouse ou shift+setas) e pressione Ctrl + Enter | Selecione as linhas desejadas e clique em "Run" |
| Rodar o script inteiro | Ctrl + Shift + Enter | Clique no botão "Source" na barra de ferramentas (canto superior direito do editor) |
| Rodar tudo do início até a linha atual | Ctrl + Alt + B | Selecione as linhas manualmente |
| Rodar da linha atual até o final | Ctrl + Alt + E | Selecione as linhas manualmente |
| Re-rodar o código anterior | Ctrl + Shift + P | Selecione as linhas manualmente |

Experimente-os utilizando as operações matemáticas já digitadas no script para testar.


## Limpar console

Para limpar o console, utilize <b>Ctrl + L</b> ou clique em "varrer" no canto superior direito do console. 


## Objetos

Depois desse primeiro contato, surge a ideia mais importante da linguagem: armazenar informações em objetos. Em vez de repetir valores toda vez que precisar deles, você pode atribuir um nome a determinado conteúdo. Esse nome passa a representar aquele valor dentro da sessão de trabalho. É como etiquetar uma caixa e guardar algo dentro dela. Sempre que você chamar esse nome novamente, o R recupera o conteúdo armazenado.

Para definir um objeto, usa-se "<-" ordenando objeto seguido de informação. Ao executar uma linha de código contendo o objeto, a resposta será a informação. Execute o código abaixo:

```r
x <- 10
x
```
```diff

+ Erro comum: lembre-se que em Ctrl + Enter o R executa apenas a linha em que está o cursor. Você deve executar a linha que determina o valor do objeto antes de exigir que a resposta seja dada no console!

```
Objetos são importantes porque quase toda análise depende disso. Em vez de lidar com números isolados, você passa a trabalhar com elementos organizados. Pode guardar uma média, um conjunto de medidas morfológicas, uma lista de espécies observadas ou uma tabela inteira de dados experimentais. 

```r
idade <- 21
especie <- "Trigona spinipes"
coletado <- TRUE
```
Tente definir e executar diferentes objetos.

Outro ponto importante nos primeiros comandos é perceber que o R diferencia maiúsculas e minúsculas. Para o programa, palavras visualmente parecidas podem ser completamente diferentes. Isso significa que atenção à escrita faz parte do processo.

Você também deve ter percebido uma movimentação no Environment após rodar a linha do primeiro objeto. Sempre que você cria um objeto, isto é, quando atribui um valor, vetor, tabela ou outro conteúdo a um nome, ele costuma aparecer automaticamente nesse painel.

Isso significa que, ao armazenar uma informação, o RStudio registra visualmente que aquele objeto agora está disponível para uso. Em vez de depender apenas da memória para lembrar o que já foi criado, você pode consultar o Environment e ver rapidamente quais nomes existem no momento.

Além do nome do objeto, o Environment frequentemente mostra informações complementares, como o tipo de dado armazenado e, em alguns casos, a quantidade de elementos presentes. Se você criou um vetor com várias observações ou importou uma tabela, o painel pode indicar dimensões e estrutura básica. Isso facilita perceber diferenças entre objetos simples e conjuntos de dados mais complexos.

O Environment também ajuda na identificação de erros. Se você tenta usar um objeto que acredita ter criado, mas ele não aparece no painel, isso pode indicar que o comando não foi executado corretamente ou que houve erro na criação. Da mesma forma, se existem muitos objetos acumulados, o painel mostra que seu ambiente está ficando carregado e talvez precise de mais organização.


## Vetores

Depois de aprender a criar objetos simples, um passo muito importante no R é entender o conceito de vetor. Vetores são importantes porque permite tratar várias observações de uma vez só. Em vez de analisar número por número manualmente, o R entende que existe um grupo de valores relacionado e pode operar sobre ele automaticamente. 

Crie um vetor utilizando o seguinte comando:

```r
abelhas <- c(12, 8, 15, 10, 7)
```

Os vetores geralmente contêm elementos do mesmo tipo. Se você criou o vetor com números, ele será entendido como um vetor numérico. Isso é ideal para contagens, medidas e resultados quantitativos. Também existem vetores de texto ou lógicos, mas no início vamos focar nos numéricos.

Explore e crie outros vetores.


## Funções

Depois que o vetor existe, entram as funções. Funções são ferramentas prontas do R criadas para executar tarefas específicas. Em vez de calcular tudo manualmente, você entrega o vetor para uma função e ela processa os dados para você. Isso torna o trabalho muito mais rápido, seguro e reproduzível.

Por exemplo, se você quiser saber a média dos valores de determinado objeto, não precisa somar tudo e dividir pelo número de observações. Uma função apropriada faz isso automaticamente. Se quiser o total de indivíduos observados, outra função pode somar todos os elementos. Se quiser saber quantas observações existem no vetor, outra função informa a quantidade de valores presentes.

Outra vantagem dos vetores é a facilidade para comparar situações. Por exemplo, se o vetor abelhas contém valores de várias coletas, você pode rapidamente observar se alguns números são maiores que outros, se há grande variação entre amostras ou se a média parece alta ou baixa. Mais adiante, isso evolui para gráficos e análises estatísticas mais robustas.

Dados reais geralmente vêm em conjuntos (várias medidas de asas, várias temperaturas registradas, várias abundâncias de espécies, várias respostas experimentais, etc.) O R foi desenvolvido justamente para lidar com esse tipo de informação de forma eficiente!

Utilizamos o seguinte comando para calcular a média de um determinado vetor:

```r
mean(abelhas)
```

Você também pode calcular a média de forma manual utilizando o seguinte comando:

```r
sum(abelhas) / length(abelhas)
```

Utilizamos o seguinte comando para calcular a mediana:

```r
median(abelhas)
```

A partir disso, calcule a média e a mediana de diferentes vetores que você determinou anteriormente.

Avançando, você verá que muitos objetos mais complexos, como colunas de tabelas e bancos de dados, são construídos a partir dessa mesma lógica de vetores. Por isso, compreender bem esse conceito no início facilita muito tudo o que vem depois.


## Comentários

Depois de aprender os primeiros comandos, é importante entender como registrar explicações dentro do próprio script, com os comentários. Comentários são trechos de texto que o R ignora ao executar o código. Eles servem apenas para leitura humana, funcionando como anotações dentro do arquivo.

Fazemos um comentário marcando um # no início ou no meio da linha:

```r
# isto é um comentário
2 + 2
3 + 5 # outro comentário
```

Isso significa que você pode escrever observações, títulos de seções, lembretes ou explicações sem interferir no funcionamento do programa. Em projetos simples, os comentários ajudam a lembrar o que cada parte faz. Em projetos maiores, tornam o script muito mais compreensível para você no futuro ou para outras pessoas que venham a ler aquele código.

Usar comentários é um hábito valioso desde o início, porque programação não envolve apenas “fazer funcionar”, mas também manter o trabalho organizado e inteligível. Um script sem comentários pode até executar corretamente, mas muitas vezes se torna confuso depois de algum tempo. 

Compare estes dois scripts e perceba como os comentários auxiliam na organização:
```diff
+  Script apenas para fins didáticos, não execute-o!
```

```r
data(iris) 
head(iris) 
names(iris)
summary(iris)
media_sepala <- mean(iris$Sepal.Length)
print(paste("Media do comprimento da sepala:", round(media_sepala, 2)))
boxplot(Petal.Length ~ Species, 
        data = iris, 
        main = "Comprimento da Petala por Especie",
        xlab = "Especies", 
        ylab = "Comprimento (cm)",
        col = c("skyblue", "lightgreen", "salmon"))
modelo_anova <- aov(Petal.Length ~ Species, data = iris)
summary(modelo_anova)
```
```r
# ==========================================================
# OBJETIVO: Analisar o comprimento de petalas em flores de Iris
# ==========================================================

# 1. CARREGAMENTO DE DADOS
# O conjunto 'iris' contem medidas de 150 flores de 3 especies
data(iris) 

# 2. EXPLORACAO INICIAL
# Exibe as primeiras 6 linhas para entender a estrutura dos dados
head(iris) 

# Ver os nomes das colunas (Variaveis)
names(iris)

# 3. ESTATISTICA DESCRITIVA
# Calcula resumo estatistico (minimo, media, maximo) para todas as colunas
summary(iris)

# Calcular a media especifica do comprimento da sepala
media_sepala <- mean(iris$Sepal.Length)
print(paste("Media do comprimento da sepala:", round(media_sepala, 2)))

# 4. VISUALIZACAO DE DADOS
# Criar um Boxplot para comparar o comprimento da petala entre especies
boxplot(Petal.Length ~ Species, 
        data = iris, 
        main = "Comprimento da Petala por Especie",
        xlab = "Especies", 
        ylab = "Comprimento (cm)",
        col = c("skyblue", "lightgreen", "salmon"))

# 5. TESTE ESTATISTICO SIMPLES (ANOVA)
# Verificando se ha diferenca significativa no comprimento das petalas entre grupos
modelo_anova <- aov(Petal.Length ~ Species, data = iris)
summary(modelo_anova) # Exibe o p-valor
```

No RStudio, também existem atalhos para comentar/descomentar linhas rapidamente. Isso facilita marcar blocos inteiros de texto sem precisar inserir o símbolo manualmente em cada linha:

<b>Ctrl + Shift + C</b>

Que tal refazer o seu script produzido até aqui como se fosse uma folha de estudos organizada? Em vez de apenas listar comandos, você pode separar seções com comentários explicando cada etapa: operações matemáticas, criação de objetos, vetores, funções principais e observações sobre atalhos importantes. Dessa forma, o script deixa de ser apenas teste de comandos e passa a ser um material de consulta pessoal!


## Salvando um script

Depois de escrever comandos e comentários, o próximo passo essencial é salvar o script. O script é um arquivo comum que armazena tudo o que foi digitado no editor: comandos, comentários e organização geral do trabalho.

Salvar é importante porque, sem isso, todo o conteúdo pode ser perdido ao fechar o programa ou desligar o computador. Além disso, manter arquivos salvos permite retomar os trabalhos.

No RStudio, salvar costuma ser simples: pode-se utilizar o menu correspondente ou o atalho Ctrl + S. Ao salvar pela primeira vez, o programa solicitará um nome e local para o arquivo.

Também é uma boa prática criar uma pasta dedicada ao projeto, mantendo scripts organizados em um só lugar.

Conforme o trabalho cresce, salvar com frequência torna-se hábito importante. Muitos usuários fazem isso repetidamente durante o uso para evitar perdas inesperadas.


## Limpar Environment

Durante os testes iniciais, é comum criar vários objetos no Environment: números, vetores, tabelas e resultados temporários. Com o tempo, esse acúmulo pode gerar confusão, especialmente quando você já não lembra quais objetos ainda são relevantes.

Por isso, em alguns momentos faz sentido limpar o Environment. Ao remover objetos antigos, você reinicia a sessão de forma mais organizada e reduz o risco de utilizar acidentalmente algo criado anteriormente.

Essa prática é especialmente útil quando se deseja testar se o script está realmente completo. Se você limpa o Environment e roda o script do início ao fim, verifica se todas as etapas necessárias estão presentes no arquivo.

Para apagar o Environment, clique em "varrer" no meio da janela dele.

É importante distinguir que apagar objetos do Environment remove dados da sessão atual, enquanto apagar texto do script altera o arquivo escrito por você.


## Sair do RStudio

Você pode sair manualmente do RStudio via "X", ou digitar o seguinte comando no console:

```r
q()
```

Depois, confirme com 'y' (sim) para salvar o workspace ou 'n' (não) para descartar.


## Resumo

Neste módulo você aprendeu:
- o que é R e RStudio
- instalação
- comandos básicos
- objetos, vetores e funções simples

Não tente decorar tudo. O objetivo inicial é perder o medo da ferramenta e começar a praticar pequenos comandos!
