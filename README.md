

<p align="center">
  <img src="Data-Lake-1024x541.png" >
</p>

# PROJETO PRÁTICO - DATA LAKE
<sub>Autores: Cristiano Fortunado, Elaine Soares e Jaime Leite</sub>


## Índice

* [Introdução](#introdução)
* [Governança de Dados](#)
  * [Como promover a Governança em um Data Lake](#)
  * [Definição do comitê Gestor](#)
  * [Política de acesso a dados](#)
  * [Captação, transformação e expurgo dos dados](#)
* [LGPD](#)
  * [O que norteia a LGPD](#)
  * [Direito a privacidade na era digital](#)
  * [Comparação entre a GDPR e a LGPD](#)
  * [Data Lake na LGPD](#)
 * [O Datalake](#)
   * [O sucessor do Data Warehouse](#)
   * [Arquitetura de referência do Data Lake](#)
   * [Arquitetura de processamento de dados em larga escala](#)
   * [Os pilares de uma arquitetura de processamento de dados em larga escala](#)
   * [Arquitetura de Big Data](#)
   * [Cultura Data Driven](#)
* [Conclusão](#)
* [Referências](#)


## Governança de Dados em Data Lake 
### Como promover a Governança em um Data Lake

**Governança Corporativa**

A Governança é um tema da alta administração das empresas maduras, e na maioria das vezes é uma exigência dos acionistas, e a sua implantação tem como objetivo estratégico a obtenção de melhores resultados nos negócios, através da definição, medição e divulgação das de grandes metas da organização. 
Podemos definir governança como um conjunto de processos e procedimentos para atingir os objetivos estratégicos de uma organização, ou também, como uma prática de planejar, controlar, medir e divulgar os resultados da estratégia das empresas.
Deve-se implantar a governança para atingir os objetivos estratégicos de uma organização, para isso é necessário definir e acompanhar a implantação de programas alinhados a estratégia para obtenção de melhores resultados.
Para queGovIU pessoas com a governança, é importante estabelecer os responsáveis para cada atividade, os fóruns para definição, estudo e de tomada de decisão.

Estrutura de Governança Corporativa

<p align="center">
  <img src="PilaresGovIU.jpg" >
</p>

<p align="center">
  <img src="GovIU.png" >
</p>

<p align="center">
  <img src="IUPAR.png" >
</p>


## O Data Lake 
### O sucessor do Data Warehouse

Por conta dessa necessidade, em 2010 James Dixon cunhou o termo Data
Lake (FOOTE, K. 2018), descrevendo uma arquitetura híbrida para armazenamento
massivo de informações em qualquer formato, incluindo dados não estruturados, em
um único local, tornando o Data Lake a peça central de infra-estrutura em uma
arquitetura orientada à dados. Dixon (BAUM, 2020, p.3) defende que "o Data Lake é um grande corpo de
água, no qual a água entra e sai por diversos dutos, e de onde exemplos podem ser
retirados e analisados”

### Arquitetura de Referência

O Data Lake deixa o dado disponível para ser lido, permitindo que qualquer
pessoa com o conhecimento apropriado tenha acesso para explorar e analizar toda
a gama de dados existente no Data Lake afim de obter informação desejada. Para
entender como o Data Lake possibilita isso, a Figura abaixo mostra uma
arquitetura simples dessa tecnologia, exemplificando as grandes fases do processo,
divididos entre captura, armazenamento e entrega dos dados.

### Arquitetura de processamento de dados em larga escala

### Os pilares de uma arquitetura de processamento de dados em larga escala

Independente da arquitetura a ser implementada para Big Data, o ideal é
que os componentes sejam desacoplados entre si, trazendo benefícios como
facilidade de manutenção, melhoria de custos, velocidade para escalar o ambiente e
muitos outros. Sendo assim, é interessante enxergar a arquitetura de dados como
grandes pilares, conforme descrito na Figura a seguir.


Fonte: SNIVELY, 2018, slide 9

De forma direta, os dados são coletados pela plataforma de diversas
origens, em seguida são armazenados para que sejam acessados quando
necessário. O próximo passo é processar os dados com o objetivo de extrair
informações relavantes e analizar os casos em que essas informações são
aplicáveis. Em seguida essas informações ficam disponíveis para serem acessadas
e interpretadas por áreas de negócio ou analistas que tomam decisões baseadas
nessas informações.

### Arquitetura de Big Data




### Cultura Data Driven

Perceba que os modelos de negócios citados acima não existiriam sem a
disciplina de análise de dados pois exigem inúmeros tipos de dados sendo eles
estruturados, não estruturados, dados em tempo real, dados históricos, enfim, uma
quantidade e diversidade gigantesca de dados que precisam ser armazenados,
processados e interpretados para que uma decisão seja tomada, seja esta decisão
feita por um ser humano entendendo e avaliando a predisposição de um paciente
para uma doença, ou um algoritmo, recomendando um filme para você assistir onde
quiser.
Além das empresas que possuem na informação seu principal negócio,
existe um conceito que vem ganhando força dia após dia que é a cultura de gestão
baseada em dados. Este modelo de gestão exclui a subjetividade do processo de
tomada de decisão e traz benefícios como visão clara das métricas da empresa,
aumento da produtividade e consequentemente dos lucros, antecipação de
possíveis falhas e problemas e velocidade na tomada de decisões. Todos esses
benefícios são alcançados com dados coletados ao longo dos processos já
existentes e precisam ser trabalhados para que se extraiam as informações que tem
valor para a empresa. Conceitos como o “DataOps Manifesto” direcionam os
princípios e boas práticas a serem seguidas por todos aqueles que desejam
implementar uma cultura de dados (DATAOPS MANIFESTO, 2019).

Fonte: BAUM, 2020, p.4 - Adaptado

Levando em conta que atualmente são gerados 2.5 quintilhões de bytes de
dados por dia (MARR, B., 2018), que mais de 80% desses dados são de
característica não estruturada e que tecnologias como IoT devem triplicar a
quantidade de informações que geramos por dia, fica claro que a peça central de
uma arquitetura orientada à dados deve ser capaz de suportar uma quantidade
colossal de dados, sendo o Data Lake a melhor opção conhecida para ser o
armazenamento do que conceitualmente denominamos como Big Data (DOMO,
2017), conceito que irermos explorar no próximo capítulo.


### Arquitetura de processamento de dados em larga escala

De acordo com AKHATAR (2018, Cap.1), a definição de Big Data são “dados
massivos em volume, com relação ao sistema de processamento, com uma
variedade de dados estruturados e não estruturados quem contêm diferentes
padrões de dados a serem analisados”.



## Conclusão ##

## Referências ##

AKHATAR, S. Big Data Architect’s Handbook: A guide to biulding proficiency in tools
systems used by leading big data experts. Birminghan: Packt, 2018.

BAUM, D. Cloud Data Lakes for Dummies. Edição Especial. New Jersey: Snowflake.
2020.

DATAOPS MANIFESTO, DataOps Manifesto.org, 2019 Disponível em: <
https://www.dataopsmanifesto.org/>. Acesso em: 25 de Nov. de 2020.

DOMO, Data Never Sleeps 5.0, Domo.com, 2017. Disponível em:
<https://www.domo.com/learn/data-never-sleeps-
5?aid=ogsm072517_1&sf100871281=1>. Acesso em: 25 de Nov. de 2020.

FOOTE, K. A Brief History of Data Lakes. Dataversity.net, 2018. Disponível em: <
https://www.dataversity.net/brief-history-data-lakes/>. Acesso em: 13 de Nov. de
2020

JAMES, J. What ‘Data Never Sleeps 7.0’ Says—and Doesn’t Say. Domo.com, 2019.
Disponível em: <https://www.domo.com/blog/what-data-never-sleeps-7-0-says-anddoesnt-
say/>. Acesso em: 25 de Nov. de 2020.

MARR, B. How Much Data Do We Create Every Day? The Mind-Blowing Stats
Everyone Should Read. Forbes.com, 2018. Disponível em:
<https://www.forbes.com/sites/bernardmarr/2018/05/21/how-much-data-do-wecreate-
every-day-the-mind-blowing-stats-everyone-should-read/#23cc78e60ba9>. Acesso em: 18 de Nov. de 2019.

SNIVELY, B. Big Data Analytics Architectural Patterns and Best Practices.
Slideshare.net, 2018. Disponível em: <
https://pt.slideshare.net/AmazonWebServices/big-data-analytics-architecturalpatterns-
and-best-practices-ant201r1-aws-reinvent-2018>. Acesso em: 20 de Nov. de
2020.

