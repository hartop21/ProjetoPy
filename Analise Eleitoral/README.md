# Pesquisas Eleitorais do Brasil

### A pesquisa foi realizada atráves de uma analise de sentimento usando python e a rede social Twitter.

Para ser realizado a extração dos dados do twitter foram utilizados as seguintes api "__python-twitter-vw__" e "__snscrape__" e para realizar a analise de sentimento foi utilizado a api "__textblob__" e para conseguir recolher informaçoes sobre as eleições foi utilizado a api do "basedosdados" que usa informações do poder360.

Para rodar os scripts é necessario ter o python instalado e o power bi para poder ver os graficos.

## Explicação sobre o script feito em python:

1. De inicio no primeiro bloco de comandos está sendo instalado as bibliotecas/api.

2. Já no segundo bloco de comandos está importando os comandos a serem utilizados

3. No terceiro bloco está sendo relacionado á extração de dados do twitter, que funcionam da seguinte forma, é definido a data de inicial e a data final, logo em após o codigo vai entrar em loop, sendo assim definido pelo __for x in range(360):__ naqual 360 representa o número de dias, e o comando __if i>10:__ naqual o 10 representa a quantidade de dados a serem recolhidos em determinado dia, após passar pelo IF o codigo será incrementado uma data tanto inicial quanto final para poder rodar até a quantia de dias informado, por tanto será recolhido 10 twittes por dia durante 360 dias, logo em seguida todo o conteúdo extraido será inserido em um dataframe.

4. No quarto bloco a função de analisar o sentimento de cada frase extraido do twitter.

5. Já no quinto bloco será realizado uma alteração na data. Também será criado um novo dataframe com a junção da data e do sentimento após isso o dataframe será salvo como um arquivo .xlsx podendo ser utilizado no power bi.

6. No sexto bloco até o 14° será realizado o mesmo procedimento para realizar a extração dos dados dos seguintes candidatos: Lula, bolsonaro, Ciro e Simone Tebet.

7. Nesse bloco foi feita a extração dos dados das eleições que foram feitas pelo poder360, onde a parte selecionada para a pesquisar será a do instituto FSB, no código o campo __billing_project_id=""__ mas para isso é necessario o id de um projeto no google cloud para realizar o download.

8. Após isso o bloco filtrará respeito do dataframe criado para coletar as informações especificas e será criado um outro arquivo .xlsx para utilizar no power bi.

9. Em seguida eu entrei no power bi e carreguei as planilhas do excel.

10. Após isso eu fiz o tratamento dos dados na tabela "Pesquisa Completa FSB" nela foi eu Promovi Cabeçalhos, Alterei o Tipo, Removi algumas colunas, Alterei o tipo de algumas colunas e Substitui valores.

11. Na tabela Sentimentos Pos eu Promovi o Cabeçalho, Alterei o tipo de algumas colunas e Substitui alguns valores.

12. Na tabela Sentimentos Neg eu Promovi o Cabeçalho, Alterei o tipo de algumas colunas e Substitui alguns valores.


## Link do Power BI:

<a href="https://app.powerbi.com/view?r=eyJrIjoiZmUzY2VmY2EtMzhlZS00NmRjLWJhNTktY2EyNzI1ZTk4MDEzIiwidCI6IjA0OTM1NTdlLTViYjQtNDVmOS1iNmRkLTdiMjI1OWYzYzMzOCJ9">Click aqui!</a>
