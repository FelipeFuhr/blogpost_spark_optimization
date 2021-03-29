## A Case Study of Optimization of a Apache Spark Big Data Application

// 1a - parte inicial introduzindo big data
The term “big data” refers to data that is so large,
fast or complex that it’s difficult or impossible to process using traditional methods.
Nowadays, many applications have to be scalable to a very big 

// 1b - parte sobre Spark
Apache Spark is a very popular open-source framework for large scale data processing
(also known as big data).
Its API can be used by Java, Python, or Scala applications.
In this case study, the optimized application was developed in Scala.

// 2 - parte sobre a importancia e possibilidade de otimizacoes:
// eh importante otimizar k : diminuir tempo e custo :
// quanto maior o uso de CPU, o tempo de processamento, e o uso de memoria, maior o custo
// frequentemente o custo de uma execucao de uma aplicacao big data pode
// chegar aos milhares(?) de reais
// Algumas operacoes em big data acabam por prejudicar desproporcionalmente a performance.
// Com algumas mudanças na implementação e arquitetura do sistema,
// podemos minimizar o uso dessas operacoes, e por consequencia otimizar
// a performance do processo.

// 3a - descricao curta da estrutura da nossa aplicacao:
	- um conjunto de processos
	- cada processo carrega dataframes, faz join, filtra, agrupa,
	  e retorna um dataframe com novas colunas, criadas durante o agrupamento
// 3b - paragrafo sobre groupby e join (reshuffle/reparticionamento)
// 3c - falar sobre a otimizaçao do select input columns

// 4 - parte sobre como validamos e analise da melhoria
// * no caso do book X, onde obtivemos a melhor melhoria de performance,
// a media do tempo de execucao baixou em ??.??% após a otimização descrita acima
// * a melhoria de performance menos significativa ocorreu no book Y,
// onde ainda assim conseguimos diminuir o tempo de execucao em ??.??%
// * na media, cada um dos processos otimizados diminuiu o tempo de execucao em ??.??%

// 5 - uma ou duas frases concluindo algo?
