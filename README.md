

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

Governança corporativa é o sistema pelo qual as empresas e demais organizações são dirigidas, monitoradas e incentivadas, envolvendo os relacionamentos entre sócios, conselho de administração, diretoria, órgãos de fiscalização e controle e demais partes interessadas, (Instituto Brasileiro de Governança Corporativa –IBGC–, 2020), ainda segundo o IBGC, 2020, as boas práticas de governança corporativa convertem princípios básicos em recomendações objetivas, alinhando interesses com a finalidade de preservar e otimizar o valor econômico de longo prazo da organização, facilitando seu acesso a recursos e contribuindo para a qualidade da gestão da organização, sua longevidade e o bem comum.

Modelo de Governanca IUPAR - Itaú Unibanco Participações, 2020

Segundo IUPAR, 2020m O principal objetivo da estrutura de governança corporativa é criar um conjunto eficiente de mecanismos de incentivo e monitoramento para assegurar que os administradores estejam sempre alinhados aos interesses dos acionistas de forma sustentável e perene. 

Os três pilares principais da estrutura de governança corporativa:

<p align="center">
  <img src="PilaresGovIU.jpg" >
</p>

Organograma da estrutura da administração, estruturado em fórum colegiados, visando uma abordagem diversificada dos assuntos para uma tomada de decisão.

<p align="center">
  <img src="GovIU.png" >
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

<p align="center">
  <img src="IMAGEM-01.jpg" >
  <br />
  Fonte: BAUM, 2020, p.4 - Adaptado
  <br />
</p>

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

Além do conceito supracitado, alguns especialistas defendem que para um
sistema ser considerado um Big Data, ele deve conter 3 características principais, os
3 V’s do Big Data, são eles:

. Volume: Talvez o mais obvio dos 3 V's, fazendo referência ao “big” no
termo Big Data, volume é uma caraterística direta do termo em questão. Como a
quantidade de dados crescendo na velocidade já citada, ter a capacidade de
absorver volumes gigantescos de dados é uma característica imperativa nos
processos de análise de dados atuais e futuros.

. Velocidade: O segundo V faz alusão à velocidade em que os dados são
gerados ou inseridos em uma plataforma de Big Data. Na Figura 5, podemos ver
que, na média, em apenas 60 segundos do ano de 2019, foram enviados 18.100.000
mensagens de texto entre celulares e 4.497.420 de buscas foram realizadas no
Google, tudo isso alimentando em tempo real os sistemas de dados das empresas
que prestam esses serviços.

. Variedade: Por variedade podemos entender os diferentes tipos de dados
processados numa plataforma de Big Data, sejam esses estruturados ou não
estruturados, sendo que o Big Data conseguiu transformar a realidade de um
universo primordialmente de dados estruturados em bacos relacionais. Hoje é
possível cruzar informações de diversas características, como por exemplo o perfil
de uma pessoa solicitando um motorista, dependendo da sua localização dentro de
um centro urbano com uma determinada condição climática.

<p align="center">
  <img src="IMAGEM-02.jpg" width="600">
  <br />
  Fonte: JAMES, 2019
  <br />
</p>

Além dos 3 V’s existem vertentes conceituais que querem transformar em 8
V’s, adicionando muitas outras características, porém os conceitos mais amplamente
aceitos são Veracidade e Valor, criando 5 Vs, sendo assim:

. Veracidade: Levando em conta que nem todo dado é relevante para a
análise em questão a acurácia do dado é importante para o sistema de Big Data como 
um todo para trazer valor à análise, dessa forma, quanto maior a acurácia do
dado, melhor é qualidade de informação final.

. Valor: Se considerarmos que o objetivo do Big Data é entregar informação
que gere conhecimento para o negócio, nada mais significativo do que valor como
requisito a ser incluído na arquitetura.

### Os pilares de uma arquitetura de processamento de dados em larga escala

Independente da arquitetura a ser implementada para Big Data, o ideal é
que os componentes sejam desacoplados entre si, trazendo benefícios como
facilidade de manutenção, melhoria de custos, velocidade para escalar o ambiente e
muitos outros. Sendo assim, é interessante enxergar a arquitetura de dados como
grandes pilares, conforme descrito na Figura a seguir.

<p align="center">
  <img src="IMAGEM-03.jpg" >
  <br />
  Fonte: SNIVELY, 2018, slide 9  
  <br />
</p>

De forma direta, os dados são coletados pela plataforma de diversas
origens, em seguida são armazenados para que sejam acessados quando
necessário. O próximo passo é processar os dados com o objetivo de extrair
informações relavantes e analizar os casos em que essas informações são
aplicáveis. Em seguida essas informações ficam disponíveis para serem acessadas
e interpretadas por áreas de negócio ou analistas que tomam decisões baseadas
nessas informações.

### Arquitetura de Big Data

Para que uma estrutura de Big Dara entregue o valor descrito com as
capacidades citadas, é importante que se tenha uma arquitetura de componentes
que comporte as necessidades descritas anteriormente, sendo assim, a Figura a seguir
descreve uma arquitetura genérica de referência para ser utilizada em ambientes de
Big Data bem como a descrição de cada componente.

<p align="center">
  <img src="IMAGEM-04.jpg" >
  <br />
  Fonte: MICROSOFT, 2019  
  <br />
</p>

. Origem de dados: Nada mais é do que a origem dos diversos dados que
comporão a plataforma de Big Data e, levando em conta o conceito de Data Lake, a
origem de dados pode ser virtualmente qualquer dado de qualquer característica
(estruturado ou não). Desde arquivos de logs ou transcrições de um telefonema,
passando por tabelas vindas do ERP ou planilhas alimentadas por prestadores de
serviços.

. Armazenamento de dados: É o repositório de todo o Big Data, uma
estrutura de Data Lake com capacidade de armazenar grandes volumes de dados e
escalar conforme o crescimento do ambiente.

. Ingestão de mensagens em tempo real: Esse é um componente que
depende do objetivo da estrutura de Big Data e deve ser usado quando existe a
necessidade de consumir e processar dados em tempo real. De forma genérica, as
mensagens são recebidas pela estrutura e armazenadas temporariamente antes de
serem inseridas no sistema de Big Data. Essa abordagem é útil pois pode funcionar
como um cache de informações, guardando dados, sem correr o risco de prejudicar
a capacidade do Data Lake de receber os dados em tempo real. Arquiteturas que
dependem de sensores de IoT, dados de trânsito e muitos outros fazem uso dessa
abordagem.

. Processamento em lote: Este componente remonta da mesma estratégia
utilizada em ETLs (do inglês Extract, Transform and Load) convencionais, onde
grandes quantidades de dados de demandam muito tempo de processamento. Em
geral, neste passo, utilizam-se abordagens mais inovativas como MapReduce, onde
o objetivo é executar algoritmos que, paralelamente mapeam as entradas dos dados
com o uso de dicionários de palavras e clusterizam esses dados, agregando em
formatos mais simples e compartimentados que são a entrada para componentes
seguintes da arquitetura.

. Processamento de stream (fluxo): Stream é um mecanismo de entrada
pervasivo que aceita qualquer tipo de mensagem que vêm do componente
responsável por executar a ingestão de dados em tempo real, por conta disso, é
necessário fazer uma sanitização básica dos dados recebidos. Independente da
qualidade, neste passo aplicam-se filtros e agregação de dados para que os
mesmos sejam persistidos com mais qualidade no componente seguinte.

. Armazenamento de dados analíticos: Uma vez com os dados
processados, é comum que o destino final dos dados processados sejam bancos de
dados, na sua maioria, em modelos não relacionais como bancos NoSQL de
documentos ou relacionais, como Data Warehouse. Isso acontece porque a maioria 
das ferramentas de análise de dados são preparadas para fazer interfaces com
esses bancos de dados.

. Análise e relatórios: Como dito anteriormente, o grande objetivo de
soluções de Big Data é preparar o dado bruto para ser analisado e, para isso, a
solução faz toda a preparação e processamento do dado e o transforma em dado
estruturado num modelo analítico para que então um profissional capacitado possa
extrair informação de qualidade sobre aqueles dados. É comum que os profissionais
de análise façam uso de ferramentas de modelagem e visualização de dados para
que encontrem a melhor informação possível para tomar decisões.

. Orquestração: Em geral, soluções de Big Data fazem processamentos
repetidos, conhecidos como fluxo de trabalho. Como exemplo prático podemos citar
transformação de dados de entrada, carregamento de sistemas, inserção em
sistemas ou tabelas, enfim, processos interdependentes que dependente de um
componente de orquestração para serem executados.

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

IBGC, Instituto Brasileiro de Governança Corporativa, 2020. Disponível em:
https://www.ibgc.org.br/conhecimento/governanca-corporativa
Acesso em 24 de set de 2020

IUPAR, Site de Relações com Investidores, 2020. Disponível em:
https://www.itau.com.br/relacoes-com-investidores/show.aspx?idCanal=vwRz5Vohb4ufKQ5nOZ68dw==&linguagem=pt
Acesso em 24 de set de 2020

JAMES, J. What ‘Data Never Sleeps 7.0’ Says—and Doesn’t Say. Domo.com, 2019.
Disponível em: <https://www.domo.com/blog/what-data-never-sleeps-7-0-says-anddoesnt-
say/>. Acesso em: 25 de Nov. de 2020.

MARR, B. How Much Data Do We Create Every Day? The Mind-Blowing Stats
Everyone Should Read. Forbes.com, 2018. Disponível em:
<https://www.forbes.com/sites/bernardmarr/2018/05/21/how-much-data-do-wecreate-
every-day-the-mind-blowing-stats-everyone-should-read/#23cc78e60ba9>. Acesso em: 18 de Nov. de 2019.

MICROSOFT. Estilo de Arquitetura de Big Data. Microsoft.com, 2019. Disponível em:
<https://docs.microsoft.com/pt-br/azure/architecture/guide/architecture-styles/bigdata>.
Acesso em: 18 de Nov. de 2020.

SNIVELY, B. Big Data Analytics Architectural Patterns and Best Practices.
Slideshare.net, 2018. Disponível em: <
https://pt.slideshare.net/AmazonWebServices/big-data-analytics-architecturalpatterns-
and-best-practices-ant201r1-aws-reinvent-2018>. Acesso em: 20 de Nov. de
2020.

