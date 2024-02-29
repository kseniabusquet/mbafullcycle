- [Módulo 1](#módulo-1)
  - [Software Enterprise](#software-enterprise)
    - [Ecossistema Enterprise](#ecossistema-enterprise)
    - [Principais características de um Sistema Enterprise](#principais-características-de-um-sistema-enterprise)
  - [Solution Architecture](#solution-architecture)
    - [Perfil da pessoa arquiteta de solução](#perfil-da-pessoa-arquiteta-de-solução)
    - [Soft Skills](#soft-skills)
    - [Principios para arquitetar uma solução](#principios-para-arquitetar-uma-solução)
    - [Iniciando com TCO (Total Cost of Ownership)](#iniciando-com-tco-total-cost-of-ownership)
    - [Aprofundando com TCO](#aprofundando-com-tco)
    - [Enterprise Architecture vs Solution Architecture](#enterprise-architecture-vs-solution-architecture)
    - [Três níveis de arquitetura de solução](#três-níveis-de-arquitetura-de-solução)
    - [Domínio, contextos e linguagem](#domínio-contextos-e-linguagem)
    - [Lei de Conway](#lei-de-conway)
    - [View e Viewpoints](#view-e-viewpoints)
    - [4 + 1](#4--1)
    - [Risco vs Documentação](#risco-vs-documentação)

## Módulo 1

### Software Enterprise

- Grande empresa ou uma unidade de negócios de uma grande empresa
- Agência de governo ou uma unidade de uma agência governamental
- Multinacional que engloba diferentes tipos de negócio
- Pequenas e médias empresas que operam de forma global

#### Ecossistema Enterprise

O software faz parte do ecossistema, ele não trabalha sozinho.

![Ecossistema Enterprise](img/ecossistema_enterprise.png)

A tarefa da **governança**: sempre olhar para como é que a tecnologia vai fazer com que os processos funcionem com que as pessoas consigam trabalhar.

As pessoas tem que ter processos claros, esses processos geralmente são mapeadas dentro do software -> **Enterprise Software**

Como arquitetos de solução, somos responsáveis por olhar essa tríade pensando na governança, garantindo: restrições de negócio, restrições de regulamentação, restrições de pessoal e de orçamento.

#### Principais características de um Sistema Enterprise

O arquiteto de solução não está pensando apenas na parte técnica, ele tem que pensar no negócio, ele tem que entender o contexto da empresa, o contexto do mercado. Além disso, ele tem que pensar em que pensar também em como manter essa solução funcionando, operável e garantindo que vai trazer valor para a empresa.

Independente do software, todos os Software Enterprise têm **características em comum**:

- **Escalabilidade**

Um software escálavel é capaz de manter a sua mesma capacidade de operação, independente da quantidade de pessoas e sistemas que vão fazer parte de todo esse Ecossistema Enterprise.

>**Exemplo**: mantendo o tempo de resposta de 100ms.

- **Disponibilidade**

Disponibilidade e conseguir deixar um sistema no ar para todo mundo usar a qualquer momento. Para manter um sistema disponível, a primeira coisa que é preciso entender é o **custo**. Outro ponto é a **estratégia**, porque existem diversas formas de manter um sistema disponível. O objetivo é **manter a eficiência operacional com o menor custo, garantindo que todo mundo possa acessar o sistema**.

Disponibilidade não é apenas um sistema rodando no ar, mas sim, a **funcionalidade que aquele sistema tem, que você consegue utilizar no momento que você quer**. É preciso alinhar os **trade offs**, entender a empresa, entender o que realmente é **prioridade**, o que dá para fazer **em segundo plano** e o que no final do dia, vai estar disponível para utilizar. Portanto, é melhor pensar em disponibilidade não apenas como máquina funcionando, mas sim, **a funcionalidade que você precisa naquele momento**. Em Sistemas Enterprise, isso é algo que não é simples, são decisões **estratégicas** que, inclusive, não somente um arquiteto de solução, um arquiteto de software, etc, vai poder tomar sozinho.

- **Segurança**

Segurança de dados, segurança operacional, segurança em autenticação, autorização de pessoas que vão ter acesso ao sistema, segurança de rede e compartilhamento de informação

**O que você sabe, o que você tem e o que você é?**  O que eu sei? Eu sei uma senha. O que eu tenho? Eu tenho um pendrive e este pendrive garante que eu estou autenticado. E o que eu sou? Eu tenho uma digital ainda para confirmar um terceiro passo de uma transação extremamente complexa.

- **Customização e Modularização**

No Sistema Enterprise, esse sistema vai ter que ser **customizado** para conseguir garantir a eficiência operacional. Mas, ao mesmo tempo, ele normalmente é **modularizado** por departamentos ou por necessidades específicas do negócio.

O mercado hoje em dia consegue fazer com que você consiga adaptar e customizar ao máximo o software das grandes corporações.

- **Integração**

Pequenos softwares geralmente não tem necessidade de integração.

Trabalho de integração é o mais comum no ambiente enterprise.

**3 pontos principais para pensar:**
1. Os sistemas que eu estou desenvolvendo conseguem se falar?
2. Os sistemas que eu estou desenvolvendo conseguem falar com sistemas de terceiros que foram desenvolvidos fora de casa?
3. Os sistemas de terceiros que você vai contratar como parte da solução em si, tem a capacidade de ser integrada de forma eficiente, com **custo baixo** e com os **sistemas atuais** da sua companhia?

- **Observabilidade**

Uma das partes **mais importantes** falando em qualquer Ecossistema Enterprise, porque é preciso garantir que tanto os seus como os sistemas dos terceiros estão funcionando.

 - Acompanhamento de **métricas** no momento que deu problema com ajuda dos **logs**
- Acompanhamento em tempo real da performance do sistema

A performance não é somente ver como o sistema está performando em relação a aguentar throughput e a latência. Mas, ao mesmo tempo, ser capaz de **rastrear o caminho da informação por dentro dos sistemas**. E, baseado nesse caminho, conseguir garantir o comportamento desse dado durante o caminho depois de passar por diversos sistemas.

### Solution Architecture

**A Arquitetura de solução faz parte de um processo de definição de estrutura, componentes, módulos, interfaces de uma solução de software para satisfazer requisitos funcionais e não funcionais, bem como o seu comportamento.**

- O que o sistema exige para o seu funcionamento?
- Como que esse sistema escala?
- Como ele é hospedado?
- Como é feito um deploy?
- Como funciona a parte de persistência?
- Como que esse sistema vai escalar e descalar?

Arquitetura de solução define/sugere as stacks de tecnologia, plataformas, ferramentas e infraestrutura que serão utilizados para implementar a solução.

O arquiteto de solução tem uma visão bem alto nível do que a aplicação vai fazer, como vai fazer e qual é o mapa da solução para os outros stakeholders (desenvolvedores, arquitetos etc.)conseguirem trabalhar.

Normalmente, softwares menores e de utilizações mais simples, raramente precisam de um arquiteto, muitas vezes um dev que tem uma experiência maior no domínio do problema que vai resolver pé suficiente. Agora, para um sistema que tem que ter **performance, escala, segurança, estabilidade, disponibilidade e tudo mais**, tem que ter uma visão mais ***high level***, porque inclusive, esses sistemas se integram com outros. Portanto, eles geram impacto diretamente em toda a organização se você estiver criando um software dessa forma.

#### Perfil da pessoa arquiteta de solução

Normalmente, uma pessoa arquiteta de solução não necessariamente tem que ser uma pessoa somente técnica. O arquiteto de solução, já tem bagagem em diversos tipos de domínio.

O arquiteto de solução tem conhecimento de diversas tecnologias de acordo com experiências anteriores.

A pessoa arquiteta de solução consegue levar em consideração o contexto, as restrições de negócio, aspectos operacionais, custos e toda a parte técnica.

É uma pessoa que **conhece o negócio com essa tecnologia e conhece a empresa**.

Portanto, o arquiteto tem a visão **do todo, ele entende do negócio, da tecnologia e das restrições que o negócio tem**. E o grande ponto aqui é que a pessoa arquiteta de solução tem que estar preparada para entregar soluções complexas para ambientes enterprise. Porque raramente vai ter um arquiteto de solução trabalhando em um sistema extremamente simples. Um ambiente enterprise, é um ambiente extremamente **crítico**, um ambiente que possui **diversos tipos de integração, diversos tipos de tecnologia com diversos tipos de cultura** dentro da mesma organização. Então, o arquiteto de solução tem que estar habituado com esse tipo de coisa.

#### Soft Skills

- Saber se adaptar em diversos tipos de projetos e contextos
- Ter maturidade emocional para conseguir fazer essa mudança
- Comunicação
- Uma pessoa que, indiretamente ou eventualmente diretamente, se torna um líder
- Uma pessoa que as pessoas podem confiar
- Pensamento estratégico ***(como que isso aqui vai durar ao longo do tempo? Quando que isso vai se pagar? Se a gente for para essa linha, o que vai acontecer?)***
- Criatividade
- Inteligência emocional
- Saber trabalhar em equipe
- Temos que saber ouvir

#### Principios para arquitetar uma solução

- Alinhamento com objetivos do negócio e com o usuário final
- Flexibilidade
- Reusabilidade
  > O que já existe? Como que eu aproveito isso?
- Interoperabilidade

  > Como outros sistemas vão se comunicar com esse sistema ou como esse sistema vai conseguir se comunicar com outros sistemas, mesmo que não precise no momento de desenvolvimento
- Mantenabilidade

  > Desde corrigir um simples bug até conseguir fazer um deploy rápido, eficiente, para conseguir resolver o problema no ar. Ou até mesmo, quando o sistema cair do ar, como que eu vou conseguir já ter um plano B para eu conseguir subir isso o mais rápido possível?
- Regras regulatórias
- Portabilidade
    > Muitas vezes um sistema ou uma solução que você vai estar fazendo, vai ser absorvida por outro sistema, ou o sistema que você fez vai absorver esse outro sistema. As informações, elas têm que estar disponíveis facilmente.

#### Iniciando com TCO (Total Cost of Ownership)

>“Uma boa arquitetura de solução abrange os casos de usos de negócio, a solução técnica e os serviços de infraestrutura subjacentes como componentes separados. Ele também pode ser usado para calcular o custo de propriedade TCO (Total Cost of Ownership) do sistema, para que os gestores da empresa possam entender o impacto financeiro da solução.”

*Fernando, Chanaka. Solution Architecture Patterns for Enterprise (p.54)*

**TCO não é somente o custo que vai ter para desenvolver a solução, mas também manter - corrigir, atualizar e criar novos recursos**

#### Aprofundando com TCO

> Uma métrica financeira que representa o custo total de comprar, desenvolver e operar uma solução ao longo do tempo.

Às vezes a solução que você está querendo desenvolver já existe no mercado e ela tem um preço.

O TCO pode estar na parte de desenvolvimento, mas também na compra de soluções prontas. E não somente a compra - a operação do negócio precisa de servidor, pessoas para dar suporte para o usuário final, suporte para o desenvolvedor e é preciso da infraestrutura. O que essa infraestrutura vai precisar? Eu vou precisar ter observabilidade nesse sistema para garantir que está tudo funcionando e eu posso confiar.

**Quando estamos falando em formato de custo, estamos falando do custo de aquisição, implementação, manutenção, operação e inativação.**

>**Operação**: garantir esse negócio funcionando de forma estável


> **Manutenção**: manter a solução no dia a dia

> **Inativação**: export de dados, quebras de contrato, as máquinas, os bancos de dados

#### Enterprise Architecture vs Solution Architecture

> **Enterprise Architecture**: possui uma visão da corporação como um todo. A Enterprise Architecture trabalha na parte do planejamento e implementação da estrutura organizacional da corporação, incluindo pessoas, processos e tecnologia.

> **Solution Architecture**: define a estrutura, características, comportamentos e relações entre um sistema específico.

A Solution Architecture está embaixo de uma Solução Enterprise que vai ser um guarda chuva que vai nortear todas as soluções que vão acontecer durante todo o processo de desenvolvimento.

#### Três níveis de arquitetura de solução

1. Arquitetura focada no negócio **(Nível 0)**

   > Como que eu vou entender o problema que eu vou resolver? O que é possível? O que não é possível? Quais são os módulos que eu vou ter que trabalhar? Quais são as decisões? Quais são requisitos funcionais, não funcionais? Como que aquilo vai funcionar na empresa? Quantas pessoas vão utilizar esse sistema?

    - ##### Nível 0 - Visão

    >A visão deixa claro os objetivos da solução de uma forma mais empírica, lógica e que deixe claro a razão de existir. A visão vai definir os principais objetivos que vão guiar a solução.

    >A visão apresenta uma visão de alto nível do que a solução vai realizar, suas necessidades, bem como todos os envolvidos.

    - ##### Nível 0 - Escopo

    >O escopo vai definir os limites ***(boundaries)*** da solução: os contextos, os limites, é até onde a solução vai, até onde a solução não vai, o que vai ser feito e acima disso, o que a solução não vai entregar.

    >Vai definir exatamente o problema que vai ser resolvido, os requisitos funcionais e não funcionais, e quais são os componentes, sistemas e tecnologias que essa solução vai utilizar. Também vai considerar as restrições e os pressupostos que podem influenciar no design da solução.

    >Assim, quando temos a visão e o escopo do projeto, é a partir daí vamos começar a entender o negócio, entender o motivo que o negócio funciona e quando isso tudo estiver definido, aí sim vamos para o nosso **nível 1 - solução técnica**.

2. Arquitetura focada na área técnica **(Nível 1)**

   > Como que eu consigo trazer aquilo que a gente pensou e que o negócio precisa para um plano de ação técnico? Ou seja, como isso vai ser desenvolvido? Quais as tecnologias que vão trabalhar? Como é que vão funcionar as integrações? Quanto esse negócio vai custar? Quanto desenvolvedores eu vou precisar? Quais soluções que nós vamos ter que desenvolver? O que a gente vai integrar, o que não vamos integrar, etc.
3. Arquitetura focada no Deployment **(Nível 2)**

   >Focada na infraestrutura que você vai utilizar aquela solução técnica que já foi criada. A infraestrutura que esse negócio vai rodar, como ele vai rodar, como é que vai ser as esteiras que nós vamos trabalhar, como que a gente garante a parte de qualidade de testes etc.

#### Domínio, contextos e linguagem

**Domínio** - o problema que você quer resolver

Trabalhando em Sistemas Enterprise, você tem que ter um conhecimento aprofundado do negócio e também tem que conseguir olhar o negócio pelo ponto de vista dos seus participantes, por exemplo: um vendedor, um parceiro de diferentes departamentos etc.

Linguagem é um aspecto muito importante, porque uma organização tem diversas áreas, tem diversos departamentos e tem diversos tipos de pessoas com culturas diferentes em países diferentes, com culturas absurdamente plurais.

**Dica: criar um glossário por area, por tipos de stakeholders**. Vai servir como um dicionário para entender como é que cada pessoa se comunica, inclusive, na hora de fazer integrações de sistemas entre essas áreas.

#### Lei de Conway

> “A lei de Conway é um princípio que afirma que o design de um sistema é influenciado pela estrutura organizacional do grupo que o produz. Isso significa que a estrutura de comunicação de um grupo será refletida na estrutura do sistemas que eles criam. A arquitetura de um sistema reflete os limites sociais do grupo que o criou.”

A estrutura organizacional da empresa vai influenciar diretamente na estrutura de design de um sistema.

![Ley de Conway](img/ley_de_conway.png)

#### View e Viewpoints

**View**:
> “Uma visão é uma representação de um ou mais aspectos estruturais de uma arquitetura que ilustra como a arquitetura aborda uma ou mais questões mantidas por um ou mais de seus stakeholders”

**Viewpoint**:
> “Um ponto de vista é uma coleção de padrões, modelos e convenções para construir um tipo de visão. Ela define as partes interessadas cuja as preocupações são refletidas no ponto de vista e nas diretrizes, princípios e templates para a construção de seu ponto de vista”

####  4 + 1

![4 + 1](img/4+1_view_model.png)

*P. Kruchten Architectural Blueprints - The "4+1" View Model of Software Architecture*

####  Risco vs Documentação

O risco vai ser totalmente proporcional à quantidade de documentações e formalizações que vai ser preciso fazer em determinada solução.

**Refleções importantes:** reflita e utilize muito o bom senso em relação aos pontos de vista que você vai levantar, os riscos que isso tem em relação à organização como um todo. Até que ponto isso vale uma documentação? Até que ponto isso vale uma documentação com detalhes e mais detalhes? Tudo isso depende do risco.
