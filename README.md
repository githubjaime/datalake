<p align="center">
  <img src="Data-Lake-1024x541.png" width="800">
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
 * [O Datalake](https://github.com/elainefabiola/datalake/blob/main/README.md#-o-data-lake)
   * [O sucessor do Data Warehouse](https://github.com/elainefabiola/datalake/blob/main/README.md#o-sucessor-do-data-warehouse)
   * [Arquitetura de referência do Data Lake](https://github.com/elainefabiola/datalake/blob/main/README.md#-arquitetura-de-refer%C3%AAncia)
   * [Arquitetura de processamento de dados em larga escala](https://github.com/elainefabiola/datalake/blob/main/README.md#arquitetura-de-processamento-de-dados-em-larga-escala)
   * [Os pilares de uma arquitetura de processamento de dados em larga escala](https://github.com/elainefabiola/datalake/blob/main/README.md#os-pilares-de-uma-arquitetura-de-processamento-de-dados-em-larga-escala)
   * [Arquitetura de Big Data](https://github.com/elainefabiola/datalake/blob/main/README.md#arquitetura-de-big-data)
   * [Cultura Data Driven](https://github.com/elainefabiola/datalake/blob/main/README.md#cultura-data-driven)
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
  <img src="PilaresGovIU.jpg" width="700">
</p>

Organograma da estrutura da administração, estruturado em fórum colegiados, visando uma abordagem diversificada dos assuntos para uma tomada de decisão.

<p align="center">
  <img src="GovIU.png" >
</p>

**Princípios Básicos da Governança Corporativa**

Os princípios básicos de governança corporativa permeiam, em maior ou menor grau, todas as práticas do Código das Melhores Práticas de Governança Corporativa, e sua adequada adoção resulta em um clima de confiança tanto internamente quanto nas relações com terceiros. São eles:

Transparência – Consiste no desejo de disponibilizar para as partes interessadas as informações que sejam de seu interesse e não apenas aquelas impostas por disposições de leis ou regulamentos. Não deve restringir-se ao desempenho econômico-financeiro, contemplando também os demais fatores (inclusive intangíveis) que norteiam a ação gerencial e que conduzem à preservação e à otimização do valor da organização; 

Equidade – Caracteriza-se pelo tratamento justo e isonômico de todos os sócios e demais partes interessadas (stakeholders), levando em consideração seus direitos, deveres, necessidades, interesses e expectativas;

Prestação de contas (accountability) – Os agentes de governança devem prestar contas de sua atuação de modo claro, conciso, compreensível e tempestivo, assumindo integralmente as consequências de seus atos e omissões e atuando com diligência e responsabilidade no âmbito dos seus papéis;   

Responsabilidade corporativa – Os agentes de governança devem zelar pela viabilidade econômico-financeira das organizações, reduzir as externalidades negativas de seus negócios e suas operações e aumentar as positivas, levando em consideração, no seu modelo de negócios, os diversos capitais (financeiro, manufaturado, intelectual, humano, social, ambiental, reputacional, etc.) no curto, médio e longo prazos.
Fonte: IBGC, 2020


## Lei Geral de Proteção de Dados (LGPD)

O debate em torno da privacidade no Brasil é mais antigo do que imaginamos. Em 2010 foi realizadoa a primeira consulta pública sobre o tema pelo Ministério da Justiça (cerca de 2.500 contribuições) segundo dados do  Núcleo de Informação e Coordenação do Ponto BR (NIC.br) a linha do tempo que mostra os debaates como surgio a LGPD é apresentado abaixo:

* 13.5.16: consulta pública do MJ resulta no PL 5.276/16, de autoria do Poder Executivo;
* 17.3.18: caso Cambridge Analytica/Facebook;
* 25.5.18: eficácia plena do GDPR;
* 29.5.18: PL 5.276/2016 e 4.060/12 declarados prejudicados em face de Subemenda Substitutiva de Plenário (PLC 53/2018 – Orlando Silva). Texto aprovado na Câmara;
* 10.7.18: PLC 53/18 aprovado no Senado, nos termos do parecer do CAE, restando prejudicado o PLS 330/13;
* Sanção: 14/8/2018, com veto à criação da Autoridade Nacional de Proteção de Dados (ANPD), sob a alegação de um possível vício de iniciativa (Projeto de lei de iniciativa parlamentar que cria órgão ou entidade da Administração Pública atingiria o desenho de competências legislativas. Haveria, pois, inconstitucionalidade insuperável e insanável, a justificar o veto). Porém, os mais de 40 artigos que se referem diretamente a ANPD não foram vetados, felizmente;
* Publicação no Diário Oficial da União: 15/8/2018 (inicialmente com 18 meses de prazo para sua eficácia plena – vacacio legis);
* MP 869/18: 28/12/2018 (entre outras questões cria a ANPD e acrescenta mais seis meses de vacacio legis);
* Eficácia plena da LGPD: 16.08.20.


<p align="center">
  <img src="lgpd01.jpg">
</p>


A Lei Geral de Proteção de Dados (LGPD), Lei 13.709/2018, entrou em vigor em 18 de setembro de 2020 a partir da sanção, pelo Presidente Jair Bolsonaro, da Lei nº 14.058/2020. É um marco legal que regulamenta o uso, a proteção e a transferência de dados pessoais no Brasil. Ela garante maior vigília  sobre as informações pessoais, exigindo consentimento explícito para coleta e uso dos dados e obriga a oferta de opções para o usuário visualizar, corrigir e excluir esses dados.
Conforme escrito no   seu  art.  1° que dispões:

**O tratamento de dados pessoais, inclusive nos meios digitais, por pessoa natural ou por pessoa jurídica de direito público ou privado, com o objetivo de proteger os direitos fundamentais de liberdade e de privacidade e o livre desenvolvimento da personalidade da pessoa natural.**


Para os fins da LGPD, considera-se:

**I - dado pessoal:** informação relacionada a pessoa natural identificada ou identificável;

**II - dado pessoal sensível:** dado pessoal sobre origem racial ou étnica, convicção religiosa, opinião política, filiação a sindicato ou a organização de caráter religioso, filosófico ou político, dado referente à saúde ou à vida sexual, dado genético ou biométrico, quando vinculado a uma pessoa natural;

**III - dado anonimizado:** dado relativo a titular que não possa ser identificado, considerando a utilização de meios técnicos razoáveis e disponíveis na ocasião de seu tratamento;

**IV - banco de dados:** conjunto estruturado de dados pessoais, estabelecido em um ou em vários locais, em suporte eletrônico ou físico;

**V - titular:** pessoa natural a quem se referem os dados pessoais que são objeto de tratamento;

**VI - controlador:** pessoa natural ou jurídica, de direito público ou privado, a quem competem as decisões referentes ao tratamento de dados pessoais;

**VII - operador:** pessoa natural ou jurídica, de direito público ou privado, que realiza o tratamento de dados pessoais em nome do controlador; 

**VIII - encarregado:** pessoa indicada pelo controlador e operador para atuar como canal de comunicação entre o controlador, os titulares dos dados e a Autoridade Nacional de Proteção de Dados (ANPD);    (Redação dada pela Lei nº 13.853, de 2019)     Vigência

**IX - agentes de tratamento:** o controlador e o operador;

**X - tratamento:** toda operação realizada com dados pessoais, como as que se referem a coleta, produção, recepção, classificação, utilização, acesso, reprodução, transmissão, distribuição, processamento, arquivamento, armazenamento, eliminação, avaliação ou controle da informação, modificação, comunicação, transferência, difusão ou extração;

**XI - anonimização:** utilização de meios técnicos razoáveis e disponíveis no momento do tratamento, por meio dos quais um dado perde a possibilidade de associação, direta ou indireta, a um indivíduo;

**XII - consentimento:** manifestação livre, informada e inequívoca pela qual o titular concorda com o tratamento de seus dados pessoais para uma finalidade determinada;

**XIII - bloqueio:** suspensão temporária de qualquer operação de tratamento, mediante guarda do dado pessoal ou do banco de dados;

**XIV - eliminação:** exclusão de dado ou de conjunto de dados armazenados em banco de dados, independentemente do procedimento empregado;

**XV - transferência internacional de dados:** transferência de dados pessoais para país estrangeiro ou organismo internacional do qual o país seja membro;

**XVI - uso compartilhado de dados:** comunicação, difusão, transferência internacional, interconexão de dados pessoais ou tratamento compartilhado de bancos de dados pessoais por órgãos e entidades públicos no cumprimento de suas competências legais, ou entre esses e entes privados, reciprocamente, com autorização específica, para uma ou mais modalidades de tratamento permitidas por esses entes públicos, ou entre entes privados;

**XVII - relatório de impacto à proteção de dados pessoais:** documentação do controlador que contém a descrição dos processos de tratamento de dados pessoais que podem gerar riscos às liberdades civis e aos direitos fundamentais, bem como medidas, salvaguardas e mecanismos de mitigação de risco; 

A  LGPD  nos  traz  em  seu  art.  6°  os  princípios  que  devem  ser  seguidos  ao  realizar tratamentos de dados pessoais:


**I - finalidade:** realização do tratamento para propósitos legítimos, específicos, explícitos e informados ao titular, sem possibilidade de tratamento posterior de forma incompatível com essas finalidades;

**II - adequação:** compatibilidade do tratamento com as finalidades informadas ao titular, de acordo com o contexto do tratamento;

**III - necessidade:** limitação do tratamento ao mínimo necessário para a realização de suas finalidades, com abrangência dos dados pertinentes, proporcionais e não excessivos em relação às finalidades do tratamento de dados;

**IV - livre acesso:** garantia, aos titulares, de consulta facilitada e gratuita sobre a forma e a duração do tratamento, bem como sobre a integralidade de seus dados pessoais;

**V - qualidade dos dados:** garantia, aos titulares, de exatidão, clareza, relevância e atualização dos dados, de acordo com a necessidade e para o cumprimento da finalidade de seu tratamento;

**VI - transparência:** garantia, aos titulares, de informações claras, precisas e facilmente acessíveis sobre a realização do tratamento e os respectivos agentes de tratamento, observados os segredos comercial e industrial;

**VII - segurança:** utilização de medidas técnicas e administrativas aptas a proteger os dados pessoais de acessos não autorizados e de situações acidentais ou ilícitas de destruição, perda, alteração, comunicação ou difusão;

**VIII - prevenção:** adoção de medidas para prevenir a ocorrência de danos em virtude do tratamento de dados pessoais;

**IX** - não discriminação: impossibilidade de realização do tratamento para fins discriminatórios ilícitos ou abusivos;

**X** - responsabilização e prestação de contas: demonstração, pelo agente, da adoção de medidas eficazes e capazes de comprovar a observância e o cumprimento das normas de proteção de dados pessoais e, inclusive, da eficácia dessas medidas. 





## <a name=“sectionj1”><a/> O Data Lake 
### O sucessor do Data Warehouse

Por conta dessa necessidade, em 2010 James Dixon cunhou o termo Data
Lake (FOOTE, K. 2018), descrevendo uma arquitetura híbrida para armazenamento
massivo de informações em qualquer formato, incluindo dados não estruturados, em
um único local, tornando o Data Lake a peça central de infra-estrutura em uma
arquitetura orientada à dados. Dixon (BAUM, 2020, p.3) defende que "o Data Lake é um grande corpo de
água, no qual a água entra e sai por diversos dutos, e de onde exemplos podem ser
retirados e analisados”

### <a name=“section”><a/> Arquitetura de Referência

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
2017).

### Arquitetura de processamento de dados em larga escala

De acordo com AKHATAR (2018, Cap.1), a definição de Big Data são “dados
massivos em volume, com relação ao sistema de processamento, com uma
variedade de dados estruturados e não estruturados quem contêm diferentes
padrões de dados a serem analisados”.

Além do conceito supracitado, alguns especialistas defendem que para um
sistema ser considerado um Big Data, ele deve conter 3 características principais, os
3 V’s do Big Data, são eles:

**Volume:** Talvez o mais obvio dos 3 V's, fazendo referência ao “big” no
termo Big Data, volume é uma caraterística direta do termo em questão. Como a
quantidade de dados crescendo na velocidade já citada, ter a capacidade de
absorver volumes gigantescos de dados é uma característica imperativa nos
processos de análise de dados atuais e futuros.

**Velocidade:** O segundo V faz alusão à velocidade em que os dados são
gerados ou inseridos em uma plataforma de Big Data. Na Figura a seguir, podemos ver
que, na média, em apenas 60 segundos do ano de 2019, foram enviados 18.100.000
mensagens de texto entre celulares e 4.497.420 de buscas foram realizadas no
Google, tudo isso alimentando em tempo real os sistemas de dados das empresas
que prestam esses serviços.

**Variedade:** Por variedade podemos entender os diferentes tipos de dados
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

**Veracidade:** Levando em conta que nem todo dado é relevante para a
análise em questão a acurácia do dado é importante para o sistema de Big Data como 
um todo para trazer valor à análise, dessa forma, quanto maior a acurácia do
dado, melhor é qualidade de informação final.

**Valor:** Se considerarmos que o objetivo do Big Data é entregar informação
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

**Origem de dados:** Nada mais é do que a origem dos diversos dados que
comporão a plataforma de Big Data e, levando em conta o conceito de Data Lake, a
origem de dados pode ser virtualmente qualquer dado de qualquer característica
(estruturado ou não). Desde arquivos de logs ou transcrições de um telefonema,
passando por tabelas vindas do ERP ou planilhas alimentadas por prestadores de
serviços.

**Armazenamento de dados:** É o repositório de todo o Big Data, uma
estrutura de Data Lake com capacidade de armazenar grandes volumes de dados e
escalar conforme o crescimento do ambiente.

**Ingestão de mensagens em tempo real:** Esse é um componente que
depende do objetivo da estrutura de Big Data e deve ser usado quando existe a
necessidade de consumir e processar dados em tempo real. De forma genérica, as
mensagens são recebidas pela estrutura e armazenadas temporariamente antes de
serem inseridas no sistema de Big Data. Essa abordagem é útil pois pode funcionar
como um cache de informações, guardando dados, sem correr o risco de prejudicar
a capacidade do Data Lake de receber os dados em tempo real. Arquiteturas que
dependem de sensores de IoT, dados de trânsito e muitos outros fazem uso dessa
abordagem.

**Processamento em lote:** Este componente remonta da mesma estratégia
utilizada em ETLs (do inglês Extract, Transform and Load) convencionais, onde
grandes quantidades de dados de demandam muito tempo de processamento. Em
geral, neste passo, utilizam-se abordagens mais inovativas como MapReduce, onde
o objetivo é executar algoritmos que, paralelamente mapeam as entradas dos dados
com o uso de dicionários de palavras e clusterizam esses dados, agregando em
formatos mais simples e compartimentados que são a entrada para componentes
seguintes da arquitetura.

**Processamento de stream (fluxo):** Stream é um mecanismo de entrada
pervasivo que aceita qualquer tipo de mensagem que vêm do componente
responsável por executar a ingestão de dados em tempo real, por conta disso, é
necessário fazer uma sanitização básica dos dados recebidos. Independente da
qualidade, neste passo aplicam-se filtros e agregação de dados para que os
mesmos sejam persistidos com mais qualidade no componente seguinte.

**Armazenamento de dados analíticos :** Uma vez com os dados
processados, é comum que o destino final dos dados processados sejam bancos de
dados, na sua maioria, em modelos não relacionais como bancos NoSQL de
documentos ou relacionais, como Data Warehouse. Isso acontece porque a maioria 
das ferramentas de análise de dados são preparadas para fazer interfaces com
esses bancos de dados.

**Análise e relatórios:** Como dito anteriormente, o grande objetivo de
soluções de Big Data é preparar o dado bruto para ser analisado e, para isso, a
solução faz toda a preparação e processamento do dado e o transforma em dado
estruturado num modelo analítico para que então um profissional capacitado possa
extrair informação de qualidade sobre aqueles dados. É comum que os profissionais
de análise façam uso de ferramentas de modelagem e visualização de dados para
que encontrem a melhor informação possível para tomar decisões.

**Orquestração:** Em geral, soluções de Big Data fazem processamentos
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
quiser. Além das empresas que possuem na informação seu principal negócio,
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

BRASIL. Lei nº. 13.709, de 14 de agosto de 2018.Dispõe sobre a proteção de dados pessoais e altera a Lei nº 12.965, de 23 de abril de 2014 (Marco Civil da Internet). Disponível em: http://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/Lei/L13709.htm Acesso em: 13 de Nov 2020.

DATAOPS MANIFESTO, DataOps Manifesto.org, 2019 Disponível em: <
https://www.dataopsmanifesto.org/>. Acesso em: 25 de Nov. de 2020.

DOMO, Data Never Sleeps 5.0, Domo.com, 2017. Disponível em:
<https://www.domo.com/learn/data-never-sleeps-
5?aid=ogsm072517_1&sf100871281=1>. Acesso em: 25 de Nov. de 2020.

FEDERAL, Senado. Senado Notícias. Disponível em: https://www12.senado.leg.br/noticias/materias/2020/09/18/lei-geral-de-protecao-de-dados-entra-em-vigor 
Acesso em 13 Nov 2020.

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

