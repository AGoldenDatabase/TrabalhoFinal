# Modelo de Apresentação da Entrega Prévia

## `data`

[Cartoes Amarelos.xlsx](https://github.com/AGoldenDatabase/TrabalhoFinal/blob/main/previa/data/interim/Cartoes%20amarelos.xlsx)

[Cartoes Vermelhos.xlsx](https://github.com/AGoldenDatabase/TrabalhoFinal/blob/main/previa/data/interim/Cartoes%20vermelhos.xlsx)

[Gols.xlsx](https://github.com/AGoldenDatabase/TrabalhoFinal/blob/main/previa/data/interim/Gols.xlsx)

[Jogadores.xlsx](https://github.com/AGoldenDatabase/TrabalhoFinal/blob/main/previa/data/interim/Jogadores.xlsx)

[Partidas.xlsx](https://github.com/AGoldenDatabase/TrabalhoFinal/blob/main/previa/data/interim/Partidas.xlsx)

[Substituicoes.xlsx](https://github.com/AGoldenDatabase/TrabalhoFinal/blob/main/previa/data/interim/Substituicoes.xlsx)

[Treinadores.xlsx](https://github.com/AGoldenDatabase/TrabalhoFinal/blob/main/previa/data/interim/Treinador.xlsx)

## `notebooks`

[GOLDB](notebooks/GOLDB.ipynb) -> Notebook com a conversão dos arquivos xlsx para o database

## `src`

Atualmente estamos utilizando python para o tratamento e execução do database. Utilizamos o Modulo Sqlite3 para criar o database e exportar o arquivo .db, para utilizar o database, basta instala-lo, ou executa-lo a partir de um notebook online, como por exemplo, o Google Colab.

## `assets`

Qualquer mídia usada no seu projeto: vídeo, imagens, animações, slides etc. Coloque os arquivos aqui (mesmo que você mantenha uma cópia no diretório do código).

# Modelo para Apresentação da Entrega Prévia do Projeto

# Projeto `<Dataset público sobre times e partidas do Campeonato Brasileiro de Futebol>`

# Equipe `<AGoldenDatabase>` - `<GOLDB>`
* `<Alan Freitas Ribeiro>` - `<193400>`
* `<David Afonso Borges dos Santos>` - `<261030>`
* `<Gabriel Dourado Seabra>` - `<216213>`

## Resumo do Projeto
> Ultimamente tem se tornado muito comum a análise de eventos esportivos orientada a dados, especialmente para realizar previsões e apostas de curto e longo prazo sobre os resultados de um campeonato. No entanto, muitos sites de estatística ainda carecem de informações que podem ser relevantes para o entendimento dos resultados do campeonato. Nesse sentido, buscamos compilar e formatar dados diversos sobre os times e partidas no Brasileirão em um banco de dados que permita traçar correlações entre as condições dos times e seus resultados.

> Nossa base de dados, além de guardar informações sobre as partidas (como data, times visitante/madante, vencedor, gols do time visitante, gols do time mandante), também trará informações sobre o valor de mercado e o salário de cada integrante do elenco e sua idade. Espera-se que, com estes dados, possamos ententar quais fatores mais corroboram para os resultados de um time no campeonato. A título de exemplo, espera-se que o valor de mercado de um jogador seja um indicador de força no seu time e que, portanto, times com jogadores mais valiosos exibam maiores chances de vitória.

## Slides da Apresentação
> Coloque aqui o link para o PDF da apresentação prévia

## Modelo Conceitual Preliminar

> Coloque aqui a imagem do modelo conceitual preliminar em ER ou UML, como o exemplo a seguir:
> ![ER Taxi](images/er-taxi.png)

## Modelos Lógicos Preliminares

> Coloque aqui os primeiros modelos lógicos dos bancos de dados relacionados aos modelos conceituais. Para o modelo relacional, sugere-se o formato a seguir. Para outros modelos lógicos o formato é livre, pode ser adotado aqueles apresentados em sala.

> Exemplo de modelo lógico relacional
~~~
PESSOA(_Código_, Nome, Telefone)
ARMÁRIO(_Código_, Tamanho, Ocupante)
  Ocupante chave estrangeira -> PESSOA(Código)
~~~

> Para o modelo de grafos de propriedades, utilize este
> [modelo de base](https://docs.google.com/presentation/d/10RN7bDKUka_Ro2_41WyEE76Wxm4AioiJOrsh6BRY3Kk/edit?usp=sharing) para construir o seu.
> Coloque a imagem do PNG do seu modelo lógico como ilustrado abaixo (a imagem estará na pasta `image`):
>
> ![Modelo Lógico de Grafos](images/modelo-logico-grafos.png)

> Para o modelo de grafos de conhecimento, utilize a abordagem
> (recurso, propriedade, valor) para apresentar seu grafo exemplo.
> Coloque a imagem do PNG do seu modelo lógico como ilustrado abaixo (a imagem estará na pasta `image).
>
> Você pode usar um grafo ilustrando as classes, como este:
> ![Modelo Lógico de Grafos de Conhecimento](images/grafo-conhecimento-classes.png)
>
> Além de outro com exemplo de instâncias, como este:
> ![Modelo Lógico de Grafos](images/grafo-conhecimento-exemplo.png)

> Para modelos hierárquicos (XML e JSON), utilize um formato
> conforme o abaixo:

> ![Modelo Lógico Hierárquico](images/modelo-logico-hierarquico.png)

## Dataset Preliminar a ser Publicado
> Elencar os arquivos/bases preliminares dos datasets serão publicados publicados.

título do arquivo/base | link | breve descrição
----- | ----- | -----
`<título do arquivo/base>` | `<link para arquivo/base>` | `<breve descrição do arquivo/base>`

> Os arquivos finais do dataset publicado devem ser colocados na pasta `data`, em subpasta `processed`. Outros arquivos serão colocados em subpastas conforme seu papel (externo, interim, raw). A diferença entre externo e raw é que o raw é em formato não adaptado para uso. A pasta `raw` é opcional, pois pode ser substituída pelo link para a base original da seção anterior.
> Coloque arquivos que não estejam disponíveis online e sejam acessados pelo notebook. Relacionais (usualmente CSV), XML, JSON e CSV ou triplas para grafos.

## Bases de Dados
> Elencar as bases de dados fonte utilizadas no projeto.

título da base | link | breve descrição
----- | ----- | -----
`<título da base>` | `<link para a página da base>` | `<breve descrição da base>`

## Operações realizadas para a construção do dataset

> Coloque um link para o arquivo do notebook, programas ou workflows que executam as operações de construção do dataset:
* extração de dados de fontes não estruturadas como, por exemplo, páginas Web
* agregação de dados fragmentados obtidos a partir de API
* integração de dados de múltiplas fontes
* tratamento de dados
* transformação de dados para facilitar análise e pesquisa

> Se for notebook, ele estará dentro da pasta `notebook`. Se por alguma razão o código não for executável no Jupyter, coloque na pasta `src`. Se as operações envolverem queries executadas atraves de uma interface de um SGBD não executável no Jupyter, como o Cypher, apresente na forma de markdown.

## Perguntas de Pesquisa/Análise Combinadas e Respectivas Análises

> Liste aqui as perguntas de pesquisa/análise e respectivas análises.
> Nem todas as perguntas precisam de queries que as implementam.
> É possível haver perguntas em que a solução é apenas descrita para
> demonstrar o potencial da base.
>
### Pergunta/Análise 1
> * Pergunta 1
>   
>   * Explicação sucinta da análise que será feita ou conjunto de queries que
>     responde à pergunta.

### Pergunta/Análise 2
> * Pergunta 2
>   
>   * Explicação sucinta da análise que será feita ou conjunto de queries que
>     responde à pergunta.

### Pergunta/Análise 3
> * Pergunta 3
>   
>   * Explicação sucinta da análise que será feita ou conjunto de queries que
>     responde à pergunta.

> Coloque um link para o arquivo do notebook que executa o conjunto de queries. Ele estará dentro da pasta `notebook`. Se por alguma razão o código não for executável no Jupyter, coloque na pasta `src`. Se as queries forem executadas atraves de uma interface de um SGBD não executável no Jupyter, como o Cypher, apresente na forma de markdown.
