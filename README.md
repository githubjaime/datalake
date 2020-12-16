<p align="center">
  <img src="Data-Lake-1024x541.png" width="800">
</p>

# PROJETO PRÁTICO - DATA LAKE
<sub>Autores: Cristiano Fortunado, Elaine Soares e Jaime Leite</sub>


## Índice

* [Introdução](#introdução)
* [Governança de Dados](https://github.com/elainefabiola/datalake/blob/main/README.md#governan%C3%A7a-de-dados-em-data-lake)
  * [Como promover a Governança em um Data Lake](https://github.com/elainefabiola/datalake/blob/main/README.md#como-promover-a-governan%C3%A7a-em-um-data-lake)
  * [Definição do comitê Gestor](https://github.com/elainefabiola/datalake/blob/main/README.md#defini%C3%A7%C3%A3o-do-comit%C3%AA-gestor)
  * [Política de acesso a dados](https://github.com/elainefabiola/datalake/blob/main/README.md#pol%C3%ADtica-de-acesso-a-dados)
  * [Captação, transformação e expurgo dos dados](https://github.com/elainefabiola/datalake/blob/main/README.md#capta%C3%A7%C3%A3o-transforma%C3%A7%C3%A3o-e-expurgo-dos-dados)
* [LGPD](#)
  * [O que norteia a LGPD](#)
  * [Direito a privacidade na era digital](#)
  * [Comparação entre a GDPR e a LGPD](#)
  * [Data Lake na LGPD](#)
 * [O Datalake](https://github.com/elainefabiola/datalake/blob/main/README.md#-o-data-lake)
   * [Origem do Termo](https://github.com/elainefabiola/datalake/blob/main/README.md#origem-do-termo)
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

Segundo IUPAR, 2020, O principal objetivo da estrutura de governança corporativa é criar um conjunto eficiente de mecanismos de incentivo e monitoramento para assegurar que os administradores estejam sempre alinhados aos interesses dos acionistas de forma sustentável e perene. 

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

**Transparência** – Consiste no desejo de disponibilizar para as partes interessadas as informações que sejam de seu interesse e não apenas aquelas impostas por disposições de leis ou regulamentos. Não deve restringir-se ao desempenho econômico-financeiro, contemplando também os demais fatores (inclusive intangíveis) que norteiam a ação gerencial e que conduzem à preservação e à otimização do valor da organização; 

**Equidade** – Caracteriza-se pelo tratamento justo e isonômico de todos os sócios e demais partes interessadas (stakeholders), levando em consideração seus direitos, deveres, necessidades, interesses e expectativas;

**Prestação de contas (accountability)** – Os agentes de governança devem prestar contas de sua atuação de modo claro, conciso, compreensível e tempestivo, assumindo integralmente as consequências de seus atos e omissões e atuando com diligência e responsabilidade no âmbito dos seus papéis;   

**Responsabilidade corporativa** – Os agentes de governança devem zelar pela viabilidade econômico-financeira das organizações, reduzir as externalidades negativas de seus negócios e suas operações e aumentar as positivas, levando em consideração, no seu modelo de negócios, os diversos capitais (financeiro, manufaturado, intelectual, humano, social, ambiental, reputacional, etc.) no curto, médio e longo prazos.

Fonte: IBGC, 2020.

### Definição do comitê Gestor

**O PMO, Project Management Office, ou em português, Escritório de Gerenciamento de Projetos**

O PMO tem como objetivo desenvolver e fornecer recursos intelectuais, processos e procedimentos para definição do **escopo**, planejamento das atividades, **pessoas**  e **aquisições** necessárias para execução, a qual fornece um estudo prévio de **prazo** e de  entregáveis, critérios de **qualidade** e aceitação, também fornece um **orçamento** prévio para atingimento dos objetivos com **integração** de pessoas, áreas e ferramentas, identificação e monitoramento de **riscos** e a **comunicação** do andamento do programa , performance e resultados medidos por indicadores pré-definidos para as **partes envolvidas** nos diversos fóruns comitês e demais canais.

Ao receber uma demanda do comitê executivo, o responsável pelo PMO, seleciona uma pessoa e o apresenta como Gerente do Programa, esta pessoa tem como responsabilidade, entender a demanda e definir, planejar, executar, monitorar e divulgar os resultados do programa.

Para uma melhor contextualização do nosso artigo, vamos descrever o objetivo do programa como **“adequação a legislação de proteção dos dados, identificar e corrigir possíveis vazamentos de informação ou acesso indevido, com fins alheios aos interesses da empresa, que possam vir a trazer algum prejuízo financeiro via indenizações ou a imagem da empresa”**.

**As áreas de suporte intelectual e operacional, Pessoas, Tecnologia e Jurídico**

Conforme nosso artigo, a área de tecnologia juntamente com a área Jurídica tem papel fundamental no programa, e é a partir das necessidades apresentadas pelo jurídico que os estudos tecnológicos que são realizados, e algumas alternativas são discutidas, sendo necessário estabelecer um grupo multidisciplinar com pessoas capacitadas em suas áreas de conhecimento para administrar os dados da empresa, canais de entrada, transformação e armazenamento, este grupo pode recomendar um estudo de maturidade da empresa em relação aos dados, onde estão e como são protegidos. O grupo pode definir o uso conceitual do DataLake, e neste momento é submetido ao PMO a carta de viabilidade, recursos intelectuais aquisições necessárias, bem como plano de implantação e de investimentos.

**As áreas de monitoramento, Auditoria e Controles Internos**

Como vimos, nossa demanda é para atender a legislação, e como vamos tratar de riscos operacionais e de imagem da organização afim de evitar prejuízos financeiros, as áreas de auditoria e controles internos define como avaliar o programa, e fazem recomendações de políticas e regras de proteção e acesso aos dados, também desenvolvem um checklist de verificação para acompanhamento durante a implantação e após sua operacionalização.
As áreas de negócios, logística e produção

Atualmente temos fonte infinita para captura dos dados, que pode ser por um aplicativo com interação humana, IoT, aprendizado de máquina, sinais e transmissores de qualquer natureza, ás áreas de negócios, mais do que nunca estão entrelaçadas com a ás áreas de logística e produção, pois um pedido de manufatura, não necessariamente passa por uma pessoa, as vendas são realizadas por uma coke ou coffee machine, os pedidos são enviados automaticamente para logística que cuida da distribuição, que pode ser no modelo tradicional, usando carros e equipamentos com operador, ou até nos modelos atuais de drones, carros e equipamentos autônomos, responsáveis pelo abastecimentos dos estoques finais, que a partir de métricas de armazenamento, dispara um pedido de produção aos setores de manufatura, e não se trata apenas de um produto, pode ser um serviço ligado a vida, que faz o diagnóstico conforme parâmetros pré-estabelecidos, e envia para um sistema que a partir de indicadores faz análise e recomendações para evitar enfermidades e a até morte, maquinas ligadas a vida monitoram sinais vitais e a partir da dinâmica do aprendizado de máquina, verifica-se a suplementação vitamínica e/ou proteica necessária.

A origem, os canais de captura e o formato dos dados não tem tanta importância em relação ao armazenamento, pois devemos estar preparados para armazenar todo tipo de dado, mas para implementar uma estratégia de proteção e acesso aos dados, as áreas de negócios devem conhecer profundamente qual o tipo de informação que é importante para alavancar os negócios, bem como o tipo de acesso que cada pessoa ou grupo de pessoas devem ter em seus canais de captura e inserção de dados e manipulação de relatórios. 

Um pedido de venda originado pela área de negócios, em seus infinitos canais, contém informações que devem ser protegidas, como dados pessoais do comprador, documentos, endereço forma de pagamento, e de suas preferências de compra, produtos, preços, quantidade e intervalos de compras, pois ele passa pelo setor produtivo, onde é feito o planejamento de produção com dados do produto e quantidade, e depois enviados ao cliente; ou, um cliente que abre uma conta bancária por um canal digital, informa seus dados pessoais e patrimoniais, necessita transitar informações financeiras de uma organização para outra, e recebe as suas correspondências físicas; ou, no envio de um pedido de vitamina D para uma farmácia, gerado por um equipamento ligado a vida, em comum, todos passam por um setor de 
logística e de distribuição, que pode ter muitas pessoas, através de suas empresas, parcerias e terceirizações e envolvidas com a informação, assim, embora tenhamos um ponto de encontro dos dados, eles estão replicados em outras estruturas de dados nos canais de parceria ou de prestação de serviços, sendo necessário uma política completa para a fragmentação da informação, de modo que cada acesso seja monitorado e controlado, uma definição clara de quem pode ver o que, de forma centralizada na origem da demanda, o demandado deve controlar e proteger a informação nos diversos canais, oferecendo acesso seguro e simplificado nas suas relações empresariais.

**Escritório de Investimentos**

Após viabilidade técnica e identificação das áreas envolvidas e suas responsabilidades, o programa é apresentado no escritório de investimentos pelo patrocinador, gerente do programa e os executivos das áreas envolvidas. O escritório de investimento tem uma cadeira permanente no comitê executivo, tem como responsabilidade estabelecer processos e procedimentos para análise de viabilidade financeira, ferramentas e técnicas para definição e controle de orçamento para liberação de 
recursos financeiros conforme entregas realizadas e o monitoramento do retorno do investimento.

Agora que entendemos o que precisa ser feito, quem faz o que e quando e qual o investimento, é desenvolvida a governança para o Data Lake, um dos itens mais importante, e é o fator de sucesso do programa, que após definida, deve ser submetida para aprovação do comitê executivo, que aprovada com pessoas, fóruns e responsabilidades, inicia o trabalho.

<p align="center">
  <img src="GovDL.png" >
</p>

### Política de acesso a dados

### Captação, transformação e expurgo dos dados

## Lei Geral de Proteção de Dados (LGPD)

O debate em torno da privacidade no Brasil é maantigo do que imaginamos. Em 2010 foi realizada a primeira consulta pública sobre o tema pelo Ministério da Justiça (cerca de 2.500 contribuições) segundo dados do  Núcleo de Informação e Coordenação do Ponto BR (NIC.br). A linha do tempo abaixo mostra os debates e o surgimento da LGPD (NIC.BR,2020):

* 13.5.16: consulta pública do MJ resulta no PL 5.276/16, de autoria do Poder Executivo;
* 17.3.18: caso Cambridge Analytica/Facebook;
* 25.5.18: eficácia plena do GDPR;
* 29.5.18: PL 5.276/2016 e 4.060/12 declarados prejudicados em face de Subemenda Substitutiva de Plenário (PLC 53/2018 – Orlando Silva). Texto aprovado na Câmara;
* 10.7.18: PLC 53/18 aprovado no Senado, nos termos do parecer do CAE, restando prejudicado o PLS 330/13;
* Sanção: 14/8/2018, com veto à criação da Autoridade Nacional de Proteção de Dados (ANPD), sob a alegação de um possível vício de iniciativa (Projeto de lei de iniciativa parlamentar que cria órgão ou entidade da Administração Pública atingiria o desenho de competências legislativas. Haveria, pois, inconstitucionalidade insuperável e insanável, a justificar o veto). Porém, . mais de 40 artigos que se referem diretamente a ANPD não foram vetados, felizmente;
* Publicação no Diário Oficial da União: 15/8/2018 (inicialmente com 18 meses de prazo para sua eficácia plena – vacacio legis);
* MP 869/18: 28/12/2018 (entre outras questões cria a ANPD e acrescenta mais seis meses de vacacio legis);
* Eficácia plena da LGPD: 16.08.20.



<p align="center">
  <img src="lgpd01.jpg">
  <br />
  Fonte: RIELLI, 2020
  <br />
  
</p>

 Lei Geral de Proteção de Dados (LGPD), Lei 13.709/2018, entrou em vigor em 18 de setembro de 2020 a partir da sanção, pelo Presidente Jair Bolsonaro, da Lei nº 14.058/2020 (FEDERAL,200). É um marco legal que regulamenta o uso, a proteção e a transferência de dados pessoais no Brasil. Ela garante maior vigília  sobre as informações pessoais, exigindo consentimento explícito para coleta e uso dos dados e obriga a oferta de opções para o usuário visualizar, corrigir e excluir esses dados.
Conforme escrito no seu art. 1° que dispõ.
**O tratamento de dados pessoais, inclusive nos meios digitais, por pessoa natural ou por pessoa jurídica de direito público ou privado, com o objetivo de proteger os direitos fundamentais de liberdade e d privacidade e o livre desenvolvimento da personalidade da pessoa natural.**
****


Para os fins de aplicação LGPD os dados são definidos como:

*I - dado pessoal:** informação relacionada a pessoa natural identificada ou identificável

      * Identificada e Identificável (cookies, outros identificadores eletrônicos e geoloacionais)

**II - dado pessoal sensível:** dado pessoal sobre origem racial ou étnica, convicção religiosa, opinião política, filiação a sindicato ou a organização de caráter religioso, filosófico ou político, dado referente à saúde ou à vida sexual, dado genético ou biométrico, quando vinculado a uma pessoa natural;

      reas de monitoramento, Auditoria e Controles Internos**

Como vimos, noDLa demanda é para atender a legislação, e como vamos tratar de riscos operacionais e de imagem da organização afim de evitar prejuízos financeiros, as áre*Podem acarretar em práticas discriminatórias
      
      *Saúde, orientação sexual, política, biometria, genéticos
      *Dados de crianças e adolescentes
    

**III - dado anonimizado:** dado relativo a titular que não possa ser identificado, considerando a utilização de meios técnicos razoáveis e disponíveis na ocasião de seu tratamento;


A  LGPD  nos  traz  em  seu  art.  6°  os  princípios  que  devem  ser  seguidos  ao  realizar tratamentos de dados pessoais:

**I - finalidade:** realização do tratamento para propósitos legítimos, específicos, explícitos e informados ao titular, sem possibilidade de tratamento posterior de forma incompatível com essas finalidades;

**II - adequação:** compatibilidade do tratamento com as finalidades informadas ao titular, de acordo com o contexto do tratamento;

**III - necessidade:** limitação do tratamento ao mínimo necessário para a realização de suas finalidades, com abrangência dos dados pertinentes, proporcionais e não excessivos em relação às finalidades do tratamento de dados;

**IV - livre acesso:** garantia, aos titulares, de consulta facilitada e gratuita sobre a forma e a duração do tratamento, bem como sobre a integralidade de seus dados pessoais;

**V - qualidade dos dados:** garantia, aos titulares, de exatidão, clareza, relevância e atualização dos dados, de acordo com a necessidade e para o cumprimento da finalidade de seu tratamento;

**VI - transparência:** garantia, aos titulares, de informações claras, precisas e facilmente acessíveis sobre a realização do tratamento e os respectivos agentes de tratamento, observados os segredos comercial e industrial;

**VII - segurança:** utilização de medidas técnicas e administrativas aptas a proteger os dados pessoais de acessos não autorizados e de situações acidentais ou ilícitas de destruição, perda, alteração, comunicação ou difusão;

**VIII - prevenção:** adoção de medidas para prevenir a ocorrência de danos em virtude do tratamento de dados pessoais;

**IX - não discriminação:** impossibilidade de realização do tratamento para fins discriminatórios ilícitos ou abusivos;

**X - responsabilização e prestação de contas:** demonstração, pelo agente, da adoção de medidas eficazes e capazes de comprovar a observância e o cumprimento das normas de proteção de dados pessoais e, inclusive, da eficácia dessas medidas.


<p align="center">
  <img src="lgpd02.jpg">
  <br />
   Fonte: Adaptado de RIELLI, 2020
  <br />
</p>


Dentro da Lei Geral de Proteção de Dados, temos no Capítulo II - Do tratamento de dados pessoais. Sobre o tratamento de dados pessoais possui as seguintes seções: Dos Requisitos para o Tratamento de Dados Pessoais, Do Tratamento de Dados Pessoais Sensíveis, Do Tratamento de Dados Pessoais de Crianças e de Adolescentes e Do Término do Tratamento de Dados. Por esse motivo teve ser levado em consideração os direitos do titular e os deveres do controlado destes dados. 

O tratamento de dados pessoais, conforme disposição do art. 7º da LGPD, somente poderá ocorrer nos seguintes casos:

**I** - mediante o fornecimento de consentimento pelo titular; 

**II** - para o cumprimento de obrigação legal ou regulatória pelo controlador;

**III** - pela administração pública, para o tratamento e uso compartilhado de dados necessários à execução de políticas públicas previstas em leis e regulamentos ou respaldadas em contratos, convênios ou instrumentos congêneres, observadas as disposições do Capítulo IV desta Lei; 

**IV** - para a realização de estudos por órgão de pesquisa, garantida, sempre que possível, a anonimização dos dados pessoais;

**V** - quando necessário para a execução de contrato ou de procedimentos preliminares relacionados a contrato do qual seja parte o titular, a pedido do titular dos dados; 
**VI** para pleitos em processo judicial, administrativo ou arbitral;

**VII** para a proteção da vida ou da incolumidade física do titular ou de terceiro;

**VIII** para a tutela da saúde, em procedimento realizado por profissionais da área da saúde ou por entidades sanitárias;

**IX** para atender aos interesses legítimos do controlador ou de terceiro, exceto no caso de prevalecerem direitos e liberdades fundamentais do titular que exijam a proteção dos dados pessoais;

**X** para a proteção do crédito, nos termos do Código de Defesa do Consumidor (CDC).

<p align="center">
  <img src="lgpd03.jpg">
</p>

O tratamento de dados pessoais de crianças e de adolescentes, conforme disposição do art. 14º da LGPD, somente poderá ocorrer nos seguintes casos:

**I** - consentimento específico e  dado por pelo menos um dos pais ou pelo responsável legal;

**II** - No tratamento de dados os controladores deverão manter pública a informação sobre os tipos de dados coletados, a forma de sua utilização;

## <a name=“sectionj1”><a/> O Data Lake 
### Origem do Termo

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

**Origem de dados:** (Data Sources) Nada mais é do que a origem dos diversos dados que
comporão a plataforma de Big Data e, levando em conta o conceito de Data Lake, a
origem de dados pode ser virtualmente qualquer dado de qualquer característica
(estruturado ou não). Desde arquivos de logs ou transcrições de um telefonema,
passando por tabelas vindas do ERP ou planilhas alimentadas por prestadores de
serviços.

**Armazenamento de dados:** (Data Storage) É o repositório de todo o Big Data, uma
estrutura de Data Lake com capacidade de armazenar grandes volumes de dados e
escalar conforme o crescimento do ambiente.

**Ingestão de mensagens em tempo real:** (Real-Time Message Ingestion) Esse é um componente que
depende do objetivo da estrutura de Big Data e deve ser usado quando existe a
necessidade de consumir e processar dados em tempo real. De forma genérica, as
mensagens são recebidas pela estrutura e armazenadas temporariamente antes de
serem inseridas no sistema de Big Data. Essa abordagem é útil pois pode funcionar
como um cache de informações, guardando dados, sem correr o risco de prejudicar
a capacidade do Data Lake de receber os dados em tempo real. Arquiteturas que
dependem de sensores de IoT, dados de trânsito e muitos outros fazem uso dessa
abordagem.

**Processamento em lote:** (Batch Processing) Este componente remonta da mesma estratégia
utilizada em ETLs (do inglês Extract, Transform and Load) convencionais, onde
grandes quantidades de dados de demandam muito tempo de processamento. Em
geral, neste passo, utilizam-se abordagens mais inovativas como MapReduce, onde
o objetivo é executar algoritmos que, paralelamente mapeam as entradas dos dados
com o uso de dicionários de palavras e clusterizam esses dados, agregando em
formatos mais simples e compartimentados que são a entrada para componentes
seguintes da arquitetura.

**Processamento de stream (fluxo):** (Stream Processing) Stream é um mecanismo de entrada
pervasivo que aceita qualquer tipo de mensagem que vêm do componente
responsável por executar a ingestão de dados em tempo real, por conta disso, é
necessário fazer uma sanitização básica dos dados recebidos. Independente da
qualidade, neste passo aplicam-se filtros e agregação de dados para que os
mesmos sejam persistidos com mais qualidade no componente seguinte.

**Armazenamento de dados analíticos :** (Analytical Data Store) Uma vez com os dados
processados, é comum que o destino final dos dados processados sejam bancos de
dados, na sua maioria, em modelos não relacionais como bancos NoSQL de
documentos ou relacionais, como Data Warehouse. Isso acontece porque a maioria 
das ferramentas de análise de dados são preparadas para fazer interfaces com
esses bancos de dados.

**Análise e relatórios:** (Analytics and Reporting) Como dito anteriormente, o grande objetivo de
soluções de Big Data é preparar o dado bruto para ser analisado e, para isso, a
solução faz toda a preparação e processamento do dado e o transforma em dado
estruturado num modelo analítico para que então um profissional capacitado possa
extrair informação de qualidade sobre aqueles dados. É comum que os profissionais
de análise façam uso de ferramentas de modelagem e visualização de dados para
que encontrem a melhor informação possível para tomar decisões.

**Orquestração:** (Orchestration) Em geral, soluções de Big Data fazem processamentos
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

NIC.br - Núcleo de Informação e Coordenação do .br. Como era e como fica a Lei Geral de Proteção de Dados 
Disponível em:<https://www.nic.br/noticia/na-midia/como-era-e-como-fica-a-lei-geral-de-protecao-de-dados/>
Acesso em: 16 de Dez. de 2020.

RIELLI, Mariana Marques, 2020. slides. Disponível em:
<https://edisciplinas.usp.br/pluginfile.php/5360635/mod_folder/content/0/Palestra%20Mariana%20Rielli%20sobre%20LGPD%20%28semestre%20passado%29.pdf?forcedownload=1>. Acesso em: 16 de Dez. de 2020.

SNIVELY, B. Big Data Analytics Architectural Patterns and Best Practices.
Slideshare.net, 2018. Disponível em: <
https://pt.slideshare.net/AmazonWebServices/big-data-analytics-architecturalpatterns-
and-best-practices-ant201r1-aws-reinvent-2018>. Acesso em: 20 de Nov. de
2020.

