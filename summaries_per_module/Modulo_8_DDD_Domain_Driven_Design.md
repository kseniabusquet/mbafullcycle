# Resumos dos vídeos

## modulo_8_11075.mp4

# Notas de Estudo: Design Orientado a Domínio (Domain Driven Design - DDD)

## Introdução
- **Título da palestra:** Design Orientado a Domínio MBA Arquitetura de Ciclo Completo
- **Objetivos da palestra:**
  1. Definir o que é Design Orientado a Domínio (DDD).
  2. Explicar por que usar DDD.
  3. Discutir padrões estratégicos e táticos.
  4. Apresentar padrões de arquitetura de software que suportam e complementam o uso de DDD.

## O que é Design Orientado a Domínio (DDD)?
- **DDD** é uma abordagem para design de modelos de software.
- Envolve uma equipe que trabalha em conjunto com *especialistas técnicos* e *especialistas de domínio* para resolver problemas de negócios complexos.
- O termo *domínio* refere-se a uma *esfera de conhecimento*, não a um controle territorial.

## Importância do DDD
- O DDD é voltado para a modelagem em situações de problemas complexos.
- Não é recomendado para soluções de software simples ou óbvias.
- O foco está em:
  - **Complexidade:** Problemas que requerem uma abordagem mais profunda e colaborativa.
  - **Contextualidade:** O DDD é contextual e se aplica dentro de um *contexto delimitado*.

## Conceitos Chave
- **Contexto Delimitado (Bounded Context):** 
  - Um espaço onde uma linguagem é desenvolvida.
  - A linguagem é restrita ao que é necessário para o modelo de software em questão.
  
- **Linguagem Ubíqua (Ubiquitous Language):**
  - Uma linguagem comum desenvolvida pela equipe para descrever problemas de negócios.
  - A linguagem é *ubíqua* apenas dentro do contexto delimitado da equipe, não em toda a organização.

## Estruturas de Colaboração
- A equipe, composta por especialistas de negócio e técnicos, trabalha em conjunto para:
  - Definir e entender o problema de negócios.
  - Desenvolver um modelo de software que atenda às necessidades identificadas.
  
## Padrões de Modelagem
### Padrões Estratégicos
- Focados em inovação.
- Envolvem decisões sobre como abordar o problema de forma ampla.

### Padrões Táticos
- Concentram-se em decisões de modelagem de software em nível mais detalhado.
- Ajudam a estruturar o desenvolvimento do software de forma eficiente.

## Conclusão
- O Design Orientado a Domínio é uma abordagem poderosa para resolver problemas complexos de negócios através de uma colaboração eficaz entre equipes técnicas e de domínio.
- A utilização de um contexto delimitado e uma linguagem ubíqua garante que todos os envolvidos tenham uma compreensão clara e comum do problema e da solução proposta. 

## Dicas de Estudo
- **Revisar os conceitos de contexto delimitado e linguagem ubíqua.**
- **Praticar a criação de um modelo de software usando DDD em um cenário de negócios fictício.**
- **Investigar casos de sucesso onde o DDD foi aplicado para entender melhor suas vantagens e desafios.**



---

## modulo_8_11076.mp4

# Estudo sobre Domain Driven Design (DDD)

## Introdução ao Domain Driven Design

- **Título da palestra**: Domain Driven Design MBA Full Cycle Architecture
- **Objetivos**:
  1. Definir o que é Domain Driven Design (DDD).
  2. Explicar por que utilizar DDD.
  3. Explorar os padrões estratégicos e táticos.
  4. Discutir a arquitetura de software que suporta o DDD.

## O que é Domain Driven Design?

- **Definição**: DDD é uma abordagem para *modelagem de software* que se concentra na resolução de problemas de negócios complexos.
- **Participantes**: A equipe é composta por:
  - Especialistas em domínio (experts).
  - Profissionais técnicos.
- **Enfoque**: A modelagem é feita através de um processo de "knowledge crunching", onde a equipe absorve o máximo de conhecimento disponível.

### Conceito de "Domínio"

- O termo "domínio" refere-se a uma *esfera de conhecimento* específica.
- É importante entender que DDD é voltado para:
  - Problemas complexos, não para soluções gerais e simples.

## Contextualização na Modelagem

- **Contexto Confinado (Bounded Context)**:
  - Refere-se ao ambiente onde uma linguagem é desenvolvida.
  - Exemplo: a equipe pode utilizar inglês, português brasileiro, ou outra língua, mas a linguagem é adaptada ao que é necessário para o modelo de software.

- **Linguagem Ubíqua**:
  - *Ubíqua* significa que a linguagem é consistente dentro do contexto limitado da equipe de desenvolvimento.
  - A equipe desenvolve essa linguagem ao interagir e descrever o problema de negócios.

### Importância da Linguagem Ubíqua

- A linguagem é:
  - Definida e restrita ao que é relevante para o modelo de software.
  - Utilizada em toda a documentação e arquitetura desenvolvida.
- Não é uma linguagem universal para toda a empresa, mas sim para o contexto específico do projeto.

## Padrões de Modelagem no DDD

- O DDD inclui **ferramentas de modelagem estratégica** e **ferramentas de modelagem tática**:
  - **Modelagem Estratégica**: Foca na inovação e na visão de longo prazo.
  - **Modelagem Tática**: Ajuda na tomada de decisões detalhadas sobre a modelagem de software.

## Conclusão

- O DDD é uma abordagem poderosa para lidar com problemas de negócios complexos por meio de uma modelagem de software colaborativa e contextualizada.
- A ênfase na *linguagem ubíqua* e no *contexto confinado* permite que equipes funcionem de maneira eficaz, garantindo que todos tenham um entendimento comum e restrito ao problema específico que estão resolvendo.

## Estrutura de Estudo

1. **Definições Importantes**:
   - Domain Driven Design (DDD)
   - Domínio
   - Contexto Confinado
   - Linguagem Ubíqua

2. **Objetivos do DDD**:
   - Resolução de problemas complexos.
   - Colaboração entre especialistas e técnicos.

3. **Padrões de Modelagem**:
   - Estratégicos
   - Táticos

4. **Aplicações do DDD**:
   - Como a abordagem pode ser aplicada em diferentes contextos de desenvolvimento de software.

5. **Reflexão**:
   - Como a implementação do DDD pode beneficiar seu projeto ou organização?



---

## modulo_8_11077.mp4

# Mapeamento de Contexto no Design Estratégico

## Introdução
O mapeamento de contexto é uma parte crucial do design estratégico, especialmente ao utilizar o *Domain-Driven Design* (DDD). É importante entender que não existe apenas um contexto delimitado em um único espaço de problema e solução.

### Pontos Principais
- Sempre haverá pelo menos um novo domínio central e um novo contexto delimitado.
- Pode haver contextos limpos adicionais ou sistemas legados.
- É comum ter múltiplos contextos delimitados que interagem entre si.

## Contextos Delimitados
- Exemplos de contextos delimitados incluem:
  - **Underwriting** (Subscrição)
  - **Risk** (Risco)

### Relação entre Contextos Delimitados
- A linha que separa os contextos pode representar:
  - **Relações entre equipes**: Como as equipes que trabalham em diferentes contextos se relacionam.
  - **Estilo de integração**: Como as informações são trocadas entre os contextos.

## Padrões de Mapeamento de Contexto
Os padrões de mapeamento de contexto refletem tanto relações de equipe quanto relações técnicas. Eles podem ser usados em conjunto.

### 1. Parceria
- **Definição**: Relação próxima entre equipes.
- **Características**:
  - Comunicação intensa, planejamento e reuniões frequentes.
  - As equipes apoiam as necessidades umas das outras sem a necessidade de formalidades.
  - Relação cara de manter, podendo ser vantajoso mudar para um tipo diferente de relacionamento ao longo do tempo.

### 2. Núcleo Compartilhado
- **Definição**: Dois contextos delimitados compartilham um modelo comum.
- **Características**:
  - As equipes utilizam o modelo compartilhado como parte de seu próprio modelo.
  - Comunicação e concordância são necessárias para definir o modelo compartilhado.
  - Desafios incluem falta de comunicação e diferentes modelos mentais entre áreas de negócio.

### 3. Cliente e Fornecedor
- **Definição**: Uma equipe atua como fornecedora e a outra como consumidora.
- **Características**:
  - O fornecedor (ex: Risk) está *upstream* (a montante) do consumidor (ex: Rate).
  - O fornecedor não precisa conhecer o consumidor.
  - O consumidor deve aceitar o que o fornecedor disponibiliza, podendo haver espaço para negociação.

### 4. Conformista
- **Definição**: O consumidor adota o modelo do fornecedor sem tradução.
- **Características**:
  - O modelo upstream é consumido como está.
  - Exemplo: Integração com softwares de terceiros, como Google Workspace, onde não se traduz o modelo, mas se conforma a ele.

### 5. Camada de Anti-Corrupção
- **Definição**: O consumidor traduz o modelo do fornecedor para um modelo mais limpo.
- **Características**:
  - Utiliza-se uma camada para evitar a confusão do modelo upstream.
  - Exemplo: Integração com sistemas complexos onde a tradução é necessária para manter a clareza.

### 6. Serviço de Host Aberto
- **Definição**: Um estilo de integração que fornece uma API.
- **Características**:
  - O downstream se registra para eventos que ocorrem no upstream.
  - Eventos fluem para o downstream, permitindo uma comunicação efetiva.

### 7. Linguagem Publicada
- **Definição**: Contextos delimitados publicam uma linguagem de modelagem para troca de informações.
- **Características**:
  - Cada contexto tem sua própria linguagem publicada, facilitando a troca de dados.
  - Exemplos de eventos: *risk assessed*, *rate calculated*, *quote generated*.

## Conclusão
O mapeamento de contexto é uma ferramenta vital no design estratégico, permitindo que as equipes entendam suas interações e como integrar suas soluções de maneira eficaz. Compreender os diferentes padrões de mapeamento de contexto ajuda a facilitar a comunicação e a colaboração entre equipes, promovendo um ambiente de desenvolvimento mais harmonioso.



---

## modulo_8_11078.mp4

# Mapeamento de Contexto no Design Estratégico

O mapeamento de contexto é uma parte fundamental do design estratégico e é crucial quando se utiliza o *Domain-Driven Design (DDD)*.

## Conceitos Principais

- **Contexto Delimitado (Bounded Context)**: Em um espaço de problema e solução, sempre haverá pelo menos um novo núcleo de domínio e um novo contexto delimitado.
- **Domínios e Contextos**: É comum ter contextos delimitados novos, como *underwriting* (subscrição) e *risk* (risco).

### Linhas entre Contextos Delimitados

- As linhas que separam os contextos não necessariamente representam um acoplamento forte entre eles.
- Essas linhas representam:
  - **Relações de Equipe**: Como as equipes interagem entre si.
  - **Estilo de Integração**: Como a informação é trocada entre os contextos.

## Padrões de Mapeamento de Contexto

### 1. Parcerias

- **Definição**: Relação onde duas equipes trabalham de forma muito próxima.
- **Características**:
  - Muitas comunicações e reuniões.
  - As equipes se apoiam mutuamente.
  - É uma relação dispendiosa de manter.

### 2. Núcleo Compartilhado (Shared Kernel)

- **Definição**: Duas equipes compartilham um modelo comum.
- **Desafios**:
  - Necessidade de comunicação eficaz.
  - Concordância sobre o modelo compartilhado.
  - Dificuldades inerentes devido a diferentes visões de modelagem.

### 3. Cliente-Fornecedor (Customer-Supplier)

- **Definição**: Uma equipe funciona como fornecedora e a outra como consumidora.
- **Características**:
  - A equipe fornecedora não conhece os detalhes do consumidor.
  - O consumidor deve aceitar o que é fornecido pela equipe fornecedora.

### 4. Conformidade (Conformist)

- **Definição**: A equipe consumidora aceita o modelo do fornecedor sem tradução.
- **Exemplo**: Uso de software de terceiros sem tentar mudar a interface.

### 5. Camada de Anti-Corrupção (Anti-Corruption Layer)

- **Definição**: A equipe consumidora traduz o modelo confuso do fornecedor para um modelo claro.
- **Importância**: Mantém a integridade do contexto consumidor ao evitar a complexidade do fornecedor.

### 6. Serviço de Anfitrião Aberto (Open Host Service)

- **Definição**: Proporciona uma API para integração entre contextos.
- **Funcionamento**:
  - O downstream registra-se para eventos do upstream.
  - Exemplos de eventos: "rate calculated" (taxa calculada).

### 7. Linguagem Publicada (Published Language)

- **Definição**: Contextos delimitados publicam uma linguagem de modelagem para troca de dados.
- **Exemplos de Eventos**:
  - *risk assessed* (risco avaliado)
  - *quote generated* (citação gerada)
  - *rate calculated* (taxa calculada)

## Conclusão

O mapeamento de contexto é uma ferramenta vital para entender e gerenciar a complexidade nas interações entre diferentes partes de um sistema. Compreender os padrões de relacionamento entre contextos delimitados melhora a colaboração entre equipes e facilita a troca de informações.



---

## modulo_8_11079.mp4

# Mapeamento de Contexto no Design Estratégico

O mapeamento de contexto é uma parte crucial do design estratégico, especialmente ao utilizar o design orientado a domínio (*domain-driven design*). A seguir, estão os principais pontos discutidos sobre o mapeamento de contexto e suas relações.

## Conceito de Contexto Delimitado

- **Contexto Delimitado**: Em um espaço de problema e solução, existem pelo menos um novo domínio central e um novo contexto delimitado.
- Exemplos de contextos delimitados:
  - **Subscrição (Underwriting)**
  - **Risco (Risk)**

## Relações entre Contextos Delimitados

- A linha entre contextos delimitados pode representar:
  - **Relações entre equipes**: Como as equipes que trabalham em contextos diferentes interagem.
  - **Estilo de integração**: Como as informações são trocadas entre os contextos.

## Padrões de Mapeamento de Contexto

### 1. Parceria (Partnership)

- Representação: Linha grossa entre contextos.
- Características:
  - Requer muita comunicação, planejamento e reuniões.
  - As equipes apoiam-se mutuamente em suas necessidades.
  - Relacionamento caro para manter, podendo ser vantajoso mudar para outro tipo de relacionamento ao longo do tempo.

### 2. Núcleo Compartilhado (Shared Kernel)

- Definição: Dois contextos delimitados compartilham um modelo comum.
- Desafios:
  - É preciso que as equipes concordem sobre o modelo a ser compartilhado.
  - Necessidade de comunicação para entender as partes do modelo que cada equipe utiliza.

### 3. Cliente-Fornecedor (Customer-Supplier)

- Definição: Uma equipe atua como fornecedora e a outra como consumidora.
- Características:
  - O fornecedor (Risco) não precisa conhecer o consumidor (Taxa).
  - O impacto flui de *upstream* (fornecedor) para *downstream* (consumidor).
  - O consumidor deve aceitar o que o fornecedor fornece, com pouca possibilidade de negociar mudanças.

### 4. Conformista (Conformist)

- Definição: A equipe consumidora se conforma ao modelo do fornecedor.
- Exemplo: Uso de softwares de terceiros (como Google Workspace) onde não há tradução dos modelos.

### 5. Camada de Anti-Corrupção (Anti-Corruption Layer)

- Definição: A equipe consumidora traduz o modelo do fornecedor para um formato que seja limpo e bem definido.
- Importância: Impede que a confusão do modelo do fornecedor contamine o modelo do consumidor.

### 6. Serviço de Anfitrião Aberto (Open Host Service)

- Definição: Um estilo de integração onde o downstream usa uma API para registrar eventos do upstream.
- Exemplo: O contexto de Taxa fornece uma API para que Subscrição, Análises e Agentes possam receber eventos.

## Linguagem Publicada (Published Language)

- Definição: Cada contexto delimitado publica uma linguagem de modelagem para troca de informações.
- Exemplos:
  - **Risco**: Risco Avaliado (Risk Assessed)
  - **Taxa**: Taxa Calculada (Rate Calculated)
  - **Subscrição**: Cotação Gerada (Quote Generated)

## Conclusão

O mapeamento de contexto é essencial para a comunicação e a interação eficaz entre diferentes equipes e sistemas em um ambiente de design orientado a domínio. A compreensão das relações e padrões de mapeamento ajuda a garantir que as equipes possam operar de forma coesa e eficiente.



---

## modulo_8_11080.mp4

## Mapeamento de Contexto no Design Estratégico

O mapeamento de contexto é uma parte fundamental do design estratégico, especialmente ao utilizar o design orientado a domínio (DDD). É importante entender que em um espaço de problema e solução, nunca existe apenas um *bounded context*.

### Principais Conceitos

- **Bounded Context**: Um limite que define uma área de modelo dentro de um domínio, onde um modelo específico é aplicado.
- **Domínio Central**: Um núcleo de conhecimento e atividade em torno do qual as operações de negócio se concentram.
- **Legado**: Sistemas existentes que podem ter um papel no contexto atual.

### Relação entre Bounded Contexts

- **Múltiplos Bounded Contexts**: É comum ter pelo menos um novo domínio central e um ou mais bounded contexts.
- **Linhas de Conexão**: As linhas que separam os bounded contexts não representam necessariamente um acoplamento forte, mas sim:
  - Relacionamentos entre equipes.
  - Estilos de integração usados para troca de informações.

## Padrões de Mapeamento de Contexto

### 1. Parcerias

- **Definição**: Relação intensa entre duas equipes que trabalham em contexts diferentes.
- **Características**:
  - Comunicação frequente e planejamento conjunto.
  - Suporte mútuo nas necessidades.
  - Relação dispendiosa que pode exigir uma transição para outro tipo de relacionamento ao longo do tempo.

### 2. Núcleo Compartilhado (Shared Kernel)

- **Definição**: Quando dois bounded contexts compartilham um modelo comum.
- **Desafios**:
  - Necessidade de comunicação clara entre as equipes.
  - Acordo sobre a definição de modelos compartilhados.
  - Dificuldades em compreender as partes do modelo que cada equipe utiliza.

### 3. Fornecedor e Consumidor (Customer Supplier)

- **Definição**: Uma equipe atua como fornecedora (upstream) e a outra como consumidora (downstream).
- **Características**:
  - O fornecedor não precisa conhecer o consumidor.
  - O consumidor deve aceitar a interface que o fornecedor oferece, muitas vezes sem garantias de mudanças.

### 4. Conformista

- **Definição**: O downstream adota o modelo do upstream sem tradução.
- **Exemplo**: Uso de software de terceiros que não requer adaptações ao modelo upstream.

### 5. Camada Anti-Corrupção (Anti-Corruption Layer - ACL)

- **Definição**: Tradução de um modelo complexo (upstream) para um modelo mais limpo (downstream).
- **Características**:
  - Evita que a complexidade do modelo upstream afete o downstream.
  - Necessária em situações onde a conformidade não é viável devido à complexidade do modelo.

### 6. Serviço de Host Aberto (Open Host Service)

- **Definição**: Oferece uma API para que downstream registre eventos que ocorrem upstream.
- **Características**:
  - A integração é realizada através de eventos.
  - Permite que os downstream se mantenham atualizados sobre mudanças no modelo upstream.

### 7. Linguagem Publicada (Published Language)

- **Definição**: Cada bounded context publica uma linguagem de modelagem para troca de dados.
- **Exemplo**: Eventos como "risco avaliado" e "taxa calculada" são parte da linguagem publicada.

## Considerações Finais

O mapeamento de contexto é uma prática essencial para entender as interações entre diferentes áreas de um sistema, permitindo uma melhor colaboração entre equipes e uma integração mais eficiente entre bounded contexts. É fundamental ter clareza sobre as relações e dependências para evitar mal-entendidos e facilitar a comunicação.



---

## modulo_8_11081.mp4

## Estudo sobre Event Sourcing em Contextos Limitados

### Introdução ao Contexto Limitado
- Um *contexto limitado* é uma área específica onde um determinado modelo de domínio é aplicado.
- Dentro desse contexto, pode-se utilizar a técnica de *event sourcing*.

### O que é Event Sourcing?
- O *event sourcing* é uma técnica utilizada para persistir o estado de um *agregado*.
- Um exemplo de agregado mencionado é o de uma *citação de apólice*.

### Funcionamento do Event Sourcing
1. **Emissão de Eventos de Domínio**
   - O *event sourcing* emite eventos de domínio sequencialmente.
   - Cada evento reflete uma parte específica do estado da citação de apólice.
   
2. **Histórico de Eventos**
   - Os eventos são registrados em uma sequência:
     - **Evento 1**: Citação inicializada.
     - **Evento 2**: Linha da citação registrada.
     - **Evento 3**: (e assim por diante até o n-ésimo evento).
     - **Evento n+1**: Linha da citação registrada novamente.
     - **Evento n+2**: Citação gerada.

3. **Persistência e Reconstituição do Estado**
   - Os eventos são armazenados em um mecanismo de armazenamento.
   - Para reconstituir a citação de apólice, os eventos são reproduzidos na ordem em que ocorreram.
   - Cada evento é interpretado pelo modelo da citação de apólice.

### Vantagens do Uso de Event Sourcing
- **Coleta de Fatos Discretos**:
  - Permite coletar informações sobre tudo o que aconteceu dentro de um modelo de domínio.
  
- **Auditoria e Conformidade**:
  - É útil para manter um *audit trail* (registro de auditoria) e garantir conformidade com regras governamentais ou da indústria (ex: saúde, finanças).
  
- **Representação do Estado Completo**:
  - A sequência total de eventos representa o estado completo do agregado.

### Conclusão
- O uso do *event sourcing* é fundamental quando se necessita de um histórico detalhado e auditável das operações realizadas em um modelo de domínio.
- Essa técnica não só facilita a reconstituição do estado anterior, mas também assegura que todas as ações possam ser verificadas e auditadas, promovendo conformidade e transparência.



---

## modulo_8_11082.mp4

# Notas de Estudo sobre Event Sourcing

## Introdução ao Contexto Delimitado
- O **contexto delimitado** é uma área de aplicação específica dentro de um modelo de domínio.
- Dentro desse contexto, técnicas e padrões como o **event sourcing** podem ser utilizados.

## O que é Event Sourcing?
- **Event sourcing** é uma técnica utilizada para persistir o estado de um agregado.
- Um exemplo prático é um agregado de **cotações de seguros**.

## Funcionamento do Event Sourcing
1. **Emissão de Eventos de Domínio**
   - Os eventos de domínio são emitidos um a um.
   - Cada evento reflete uma parte específica do estado da cotação de seguro.
   
2. **Exemplo de Eventos em uma Cotação**
   - **Evento 1:** Cotação inicializada.
   - **Evento 2:** Linha da cotação registrada.
   - **Evento 3:** Repetição da linha da cotação registrada.
   - **Evento 4:** Cotação gerada.

3. **Persistência de Eventos**
   - Todos esses eventos são armazenados em um mecanismo de armazenamento.
   - Eles podem ser recuperados posteriormente para reconstituir o estado anterior da cotação.

## Reconstituição do Estado
- Para recriar a política que existia anteriormente:
  - Os eventos armazenados são reproduzidos um a um, na mesma ordem em que ocorreram.
  - A cotação de seguro é ajustada com base no que cada evento significa para ela.

### Processo de Reconstituição
- Após reproduzir toda a sequência de eventos:
  - O estado da cotação de seguro é completamente reconstituído.

## Por que usar Event Sourcing?
- **Principais Motivos:**
  - Necessidade de coletar **fatos discretos** sobre tudo que aconteceu dentro de um modelo de domínio.
  - Garantir conformidade com regras governamentais ou da indústria (ex: regras médicas, financeiras).
  - Criar um **rastro de auditoria** e uma história persistida de tudo que aconteceu.

### Benefícios do Event Sourcing
- Representa o estado completo do agregado.
- Fornece uma visão detalhada do histórico e dos eventos que influenciaram o estado atual.

## Conclusão
- O event sourcing é uma técnica poderosa para a gestão de estados e eventos em modelos de domínio, permitindo a auditoria e a reconstituição precisa do histórico de uma entidade.



---

## modulo_8_11083.mp4

# Resumo sobre Event Sourcing

## Contexto Limitado

- Um *contexto limitado* pode utilizar uma técnica chamada **event sourcing**.
- O **event sourcing** é usado para persistir o estado de um *aggregate* (agregado), como um *policy quote aggregate* (agregado de cotação de política).

## Funcionamento do Event Sourcing

- O **event sourcing** emite **eventos de domínio**. Cada evento de domínio reflete uma parte específica do estado da cotação da política.
  
### Exemplo de Eventos

1. **Cotação Inicializada**: Primeiro evento.
2. **Registro de Linha da Cotação**: Segundo evento.
3. **Registro de Linha da Cotação (Novamente)**: A partir do terceiro até o n-ésimo evento.
4. **Cotação Gerada**: Último evento (n+2).

- Esses eventos são persistidos em um mecanismo de armazenamento para serem recuperados posteriormente.

## Reconstituição do Estado

- O objetivo de recuperar os eventos é reconstituir a política que existia anteriormente.
- Isso é feito através da reprodução dos eventos armazenados:
  - Os eventos são reproduzidos **um a um**, na ordem em que ocorreram.
  - Cada evento é interpretado pelo *policy quote* para determinar o que significa para ele.

### Processo de Reconstituição

1. Reproduzir o primeiro evento.
2. Atualizar o estado da cotação com base nesse evento.
3. Repetir para todos os eventos na sequência.

- Após a reprodução de todos os eventos, o estado da cotação da política é completamente reconstituído.

## Razões para Usar Event Sourcing

1. **Coleta de Fatos Discretos**: Útil quando é necessário ter uma *ficha* de tudo que aconteceu dentro de um modelo de domínio.
2. **Conformidade**: Permite garantir a conformidade com regras governamentais ou setoriais (ex.: regras médicas, transações financeiras).
3. **Rastro de Auditoria**: Proporciona um histórico persistido de tudo que ocorreu.
4. **Representação do Estado Completo**: A corrente total de eventos representa o estado completo do agregado.

## Conclusão

O **event sourcing** é uma técnica poderosa para garantir a integridade e a rastreabilidade do estado dos agregados em um modelo de domínio, permitindo reconstituição e conformidade com regras externas.



---

## modulo_8_11084.mp4

# Resumo sobre Event Sourcing em Contextos Delimitados

## Introdução ao Contexto Delimitado
- Um **contexto delimitado** é uma parte de um sistema onde um modelo de domínio é definido e aplicado.
- Dentro desse contexto, técnicas e padrões específicos podem ser utilizados para gerenciar estados.

## O que é Event Sourcing?
- **Event Sourcing** é uma técnica utilizada para persistir o estado de um *aggregate* (agregado).
- Exemplo: Um *aggregate* referente a uma cotação de seguro (policy quote).

### Funcionamento do Event Sourcing
1. **Emissão de eventos de domínio**:
   - O *aggregate* emite eventos de domínio, cada um representando uma parte específica do estado da cotação.
2. **Histórico de Eventos**:
   - Eventos são registrados em uma sequência cronológica. Exemplos de eventos:
     - **Quote Initialized** (Cotação Inicializada)
     - **Quote Line Recorded** (Linha da Cotação Registrada)
     - **Quote Generated** (Cotação Gerada)
3. **Persistência**:
   - Os eventos são armazenados em um mecanismo de armazenamento para serem recuperados posteriormente.

## Reconstituição do Estado
- Para recriar o estado anterior da cotação:
  - Os eventos são reproduzidos em ordem, um de cada vez.
  - O sistema interpreta o que cada evento significa para o estado da cotação.
- **Resultado**: Após reproduzir todos os eventos, o estado da cotação é totalmente reconstituído.

## Motivos para Utilizar Event Sourcing
1. **Coleta de Fatos Discretos**:
   - Útil para registrar tudo o que ocorreu em um modelo de domínio.
   - Exemplos de áreas de aplicação:
     - Conformidade com regras governamentais.
     - Normas da indústria (ex.: setor médico ou financeiro).
2. **Auditoria e Rastreabilidade**:
   - Permite a criação de um histórico auditável de todas as ações que ocorreram.
3. **Representação Completa do Estado**:
   - Todo o fluxo de eventos representa o estado completo do agregado.

## Conclusão
- O Event Sourcing é uma técnica poderosa para garantir a integridade e a rastreabilidade dos dados dentro de um contexto delimitado, permitindo uma visão clara do histórico de ações e do estado atual dos *aggregates*.



---

## modulo_8_11085.mp4

# Resumo da Discussão sobre Processos de Orquestração de Aplicações

## Introdução
Nesta seção, discutimos o uso de um processo de aplicação premium, um gerenciador de processos ou *saga*, que é utilizado para gerar etapas e processar comandos com base nessas etapas.

## Conceitos Principais

### Gerenciador de Processos
- O gerenciador de processos é conhecido como um *orquestrador*.
- Este sistema realiza a *orquestração de processos*.

### Importância do Message Bus
- O *message bus* continua presente na arquitetura.
- A diferença é que não é necessário que cada contexto de domínio (como risco e subscrição) traduza o evento recebido.

## Funcionamento do Processo
1. **Recepção de Eventos:**
   - O evento "aplicação submetida" é recebido no *message bus*.
   
2. **Tradução de Comandos:**
   - O processo de aplicação premium traduz o evento "aplicação submetida" para o comando "avaliar risco".
   - O contexto de risco, portanto, não precisa fazer essa tradução por conta própria.

3. **Processamento de Comandos:**
   - O contexto de risco recebe o comando "avaliar risco".
   - O contexto processa esse comando e emite um evento "risco avaliado".

## Benefícios da Orquestração
- A orquestração permite que o gerenciador de processos cuide de parte do trabalho pesado:
  - **Roteamento:** Gerencia como os eventos e comandos são direcionados entre os diferentes contextos.
  - **Eficiência:** Reduz a complexidade e o acoplamento entre os diferentes componentes do sistema.

## Comparação com Coreografia
- Embora o processo discutido seja similar à *coreografia*, a orquestração oferece vantagens em termos de gerenciamento e simplificação dos processos.

## Conclusão
- A utilização de um gerenciador de processos proporciona uma maneira mais eficiente de lidar com eventos e comandos em um sistema distribuído, permitindo que os diferentes contextos de domínio se concentrem em suas responsabilidades específicas sem a necessidade de gerenciar traduções de eventos.



---

## modulo_8_11086.mp4

# Resumo da Palestra sobre Processos de Orquestração de Aplicações

## Introdução
Nesta palestra, discutimos a utilização de *processos de aplicação premium* ou *gerenciadores de processos* (sagas) para gerar etapas e comandos. Esses comandos, uma vez processados, emitem eventos que são consumidos pelo processo de aplicação premium.

## Conceitos-chave

### Gerenciador de Processos
- Também conhecido como *orquestrador*.
- Realiza a *orquestração de processos*.

### Barramento de Mensagens
- O barramento de mensagens permanece presente no sistema.
- A diferença é que o processo de aplicação premium faz a tradução dos eventos em comandos.

### Exemplos de Tradução de Comandos
- Evento na mensagem: **application submitted** (aplicação submetida).
- Tradução pelo processo de aplicação: **assess risk** (avaliar risco).
- O contexto de risco não precisa traduzir o evento, apenas recebe o comando **assess risk**, processa e emite o evento **risk assessed** (risco avaliado).

## Benefícios da Orquestração
- A orquestração permite que um gerenciador de processos cuide do trabalho pesado e do roteamento.
- Facilita a comunicação entre diferentes contextos, evitando a necessidade de adaptações complexas.

## Comparação com Coreografia
- O processo descrito é semelhante ao que foi apresentado anteriormente através do conceito de *coreografia*.
- A principal diferença é a presença de um orquestrador que simplifica a comunicação e o fluxo de informações.

## Conclusão
- O uso de um gerenciador de processos em um sistema baseado em eventos pode aumentar a eficiência e reduzir a complexidade.
- A orquestração melhora a forma como os eventos são processados e traduzidos, permitindo um fluxo mais claro e eficiente de informações.

## Pontos para Estudo
- Compreender a diferença entre *orquestração* e *coreografia*.
- Estudar como eventos são traduzidos e processados dentro de um sistema de gerenciamento de processos.
- Analisar os benefícios da orquestração em sistemas complexos.

### Dicas de Estudo
- Revisar conceitos de barramento de mensagens.
- Praticar a identificação de contextos e eventos em sistemas de software.
- Discutir em grupo exemplos práticos de orquestração e coreografia em projetos reais.



---

## modulo_8_11087.mp4

# Resumo da Aula sobre Processos de Orquestração

## Introdução à Orquestração de Processos
- A orquestração de processos é um conceito essencial em sistemas de software complexos.
- Utiliza-se um **gerenciador de processos** ou **saga** para coordenar as etapas de um processo.

## Funcionamento do Gerenciador de Processos
- O gerenciador de processos age como um **orquestrador**.
- Ele gera *passos* com base nas ações tomadas e nos comandos processados.
- Os eventos são emitidos e consumidos pelo processo de aplicação premium.

### Mensagem Bus
- O **message bus** permanece presente na arquitetura.
- Em vez de cada componente, como o *risco* e o *subscrição*, traduzir eventos individualmente:
  - O processo de aplicação premium realiza a tradução.

## Exemplo de Tradução de Eventos
1. Evento recebido: **Application Submitted** (Aplicação Submetida).
2. O processo de aplicação premium traduz esse evento para **Assess Risk** (Avaliar Risco).
3. O contexto de risco recebe o comando **Assess Risk** e processa, emitindo o evento **Risk Assessed** (Risco Avaliado).

### Vantagens da Orquestração
- A orquestração ajuda a centralizar o processo de tradução e roteamento:
  - Reduz a complexidade para os contextos de risco e subscrição.
  - Permite que os componentes se concentrem em suas funções principais.

## Comparação com Coreografia
- O método de orquestração é semelhante ao processo de *coreografia*:
  - A diferença é que a orquestração utiliza um gerenciador para realizar o trabalho pesado.
  - Isso melhora a eficiência e clareza na comunicação entre componentes.

## Conclusão
- A orquestração de processos é uma abordagem eficaz para gerenciar sistemas complexos.
- O uso de um gerenciador de processos simplifica a interação entre diferentes componentes, promovendo uma comunicação mais clara e eficiente. 

### Palavras-chave
- **Gerenciador de processos**
- **Saga**
- **Orquestrador**
- **Message bus**
- **Tradução de eventos**
- **Coreografia** 

Estes pontos fornecem uma visão clara do funcionamento e das vantagens do uso de um gerenciador de processos em sistemas de software.



---

## modulo_8_11088.mp4

# Resumo da Discussão sobre Gerenciamento de Processos e Orquestração

## Introdução
Nesta seção, abordamos o uso de um *processo premium de aplicação* ou *gerenciador de processos* (saga) para gerar etapas e processar comandos, emitindo eventos que são consumidos pelo processo premium da aplicação.

## Gerenciamento de Processos

- **Definição de Gerenciador de Processos**: 
  - Um gerenciador de processos é conhecido como um *orquestrador*.
  - Ele facilita a *orquestração de processos* dentro do sistema.

## Funcionamento do Sistema

- **Mensagem Bus**:
  - O *message bus* continua presente no sistema.
  - Em vez de cada contexto (como risco e subscrição) traduzir eventos recebidos em comandos, o processo premium da aplicação realiza essa tradução.

- **Exemplo de Tradução de Eventos**:
  - Evento recebido: "application submitted" (aplicação submetida).
  - Tradução no processo premium: "assess risk" (avaliar risco) para o contexto de risco.
  - O contexto de risco recebe o comando "assess risk", processa e emite o evento "risk assessed" (risco avaliado).

## Benefícios da Orquestração

- **Eficiência**:
  - O uso de um orquestrador reduz a carga sobre os contextos individuais, permitindo que eles se concentrem em suas funções específicas.
  
- **Continuidade da Tradução de Eventos**:
  - A tradução de eventos continua ocorrendo de maneira organizada, garantindo que cada parte do sistema receba as informações necessárias de forma eficiente.

## Comparação com Coreografia

- A orquestração é uma alternativa à *coreografia*, onde eventos e comandos são geridos de maneira descentralizada.
- Com a orquestração, o gerenciador de processos cuida de parte do trabalho pesado e do roteamento, facilitando a comunicação entre os diferentes contextos do sistema.

## Conclusão
A utilização de um gerenciador de processos para orquestrar a comunicação entre os diferentes contextos de um sistema não apenas simplifica o fluxo de informações, mas também melhora a eficiência do processamento e a gestão de eventos. Essa abordagem permite que cada parte do sistema opere de forma mais focada e organizada.



---

## modulo_8_11089.mp4

# Resumo da Aula: Espaço do Problema vs. Espaço da Solução no Domínio do Rio & Design

## Introdução
- O tema da aula é a abordagem do **Domínio do Rio & Design**, focando em duas perspectivas importantes: **espaço do problema** e **espaço da solução**.
- Não é necessário seguir estritamente essas visões, mas elas fornecem uma estrutura interessante para entender o desenvolvimento de software.

## Espaço do Problema
- **Definição**: O espaço do problema refere-se à identificação e compreensão dos problemas que precisam ser resolvidos.
- **Estabelecimento do Domínio do Software**: O foco aqui é identificar o domínio principal, como, por exemplo, a área de vendas e compra de ingressos.

### Subdomínios
- **Identificação de Subdomínios**: É crucial encontrar novos subdomínios ou reaproveitar subdomínios existentes.
- **Contexto e Linguagem Ubíqua**: Mesmo que subdomínios tenham o mesmo nome em diferentes softwares, eles podem ser distintos devido ao contexto em que estão inseridos.

#### Exemplo de Subdomínio: Vendas de Ingressos
- **Subdomínio de Eventos**:
  - Envolve parceiros, clientes, eventos, assentos e ingressos.
  - Necessidade de autenticação para identificar usuários e suas permissões.
  - Gestão de e-mails para comunicação.

## Espaço da Solução
- **Definição**: O espaço da solução trata de como os subdomínios identificados no espaço do problema serão resolvidos.
- **Core Domains**: Identificação dos domínios mais importantes (Cores) para o software, como eventos e ingressos.

### Relações entre Subdomínios
- **Upstream e Downstream**: 
  - O subdomínio de eventos é um consumidor do subdomínio de ingressos.
  - O ingresso atua como fornecedor, enquanto eventos é o cliente.
  
#### Exemplos de Domínios Genéricos
- **Autenticação**: É mais viável utilizar soluções prontas (frameworks ou softwares de terceiros) ao invés de desenvolver do zero.
- **E-mails**: Também pode ser tratado como um domínio genérico, utilizando soluções de envio de e-mails já existentes.

## Importância da Visão da Solução
- A visão da solução é fundamental para entender como os subdomínios se relacionam e como as mudanças em um podem impactar o outro.
- A estabilidade dos domínios centrais (Core Domains) é essencial para a redução de custos de manutenção e melhoria da qualidade do software.

### Riscos e Proteções
- A relação downstream pode levar a riscos, onde mudanças nos upstreams impactam os downstreams.
- É necessário pensar em mecanismos para proteger os domínios centrais de instabilidades.

## Conclusão
- A aula destaca a importância de mapear contextos e a relação entre subdomínios.
- A discussão sobre táticas será abordada em aulas futuras, mas o foco atual é entender as perspectivas do problema e da solução.

## Próximos Passos
- Continuar a exploração do tema em futuras aulas, aprofundando-se nas táticas de implementação.

---

**Lembre-se**: A compreensão clara desses conceitos é fundamental para o desenvolvimento de software eficaz e bem estruturado, especialmente em domínios complexos como vendas de ingressos.



---

## modulo_8_11091.mp4

# Estudo sobre Espaço do Problema e Espaço da Solução no Domínio do Rio & Design

## Introdução
- O contexto da palestra aborda a modelagem de software por meio de duas perspectivas principais: **espaço do problema** e **espaço da solução**.
- O foco está no entendimento desses espaços para melhor desenvolver aplicações no domínio específico de vendas de ingressos.

## Espaço do Problema
- **Definição**: O espaço do problema refere-se à identificação e compreensão do problema que o software precisa resolver.
- **Importância**: Estabelecer o domínio do software é essencial, pois é neste espaço que se define qual é o problema principal a ser abordado.
- **Subdomínios**: 
  - Identificação de subdomínios é crucial, uma vez que cada subdomínio pode representar um aspecto específico do problema.
  - Exemplo de subdomínios no contexto de venda de ingressos:
    - **Eventos**: gerenciamento de parceiros, clientes e detalhes do evento.
    - **Ingressos**: geração de QR Codes e validação.
    - **Autenticação**: controle de identidade dos usuários.
    - **E-mails**: comunicação com os clientes.

### Perspectiva de Modelagem
- O espaço do problema é mais bem descrito no livro **Redbook** de Vernon do que no livro de Evans.
- A modelagem deve considerar o contexto e a *linguagem ubíqua* de cada subdomínio.

## Espaço da Solução
- **Definição**: O espaço da solução envolve a maneira como os subdomínios identificados no espaço do problema serão resolvidos.
- **Core Domains**: Identificação dos subdomínios mais importantes, que são críticos para o funcionamento do software.
  - Exemplo: As partes de **Eventos** e **Ingressos** são considerados os *Core Domains*.

### Relações Entre Subdomínios
- **Upstream e Downstream**:
  - **Eventos** atua como um consumidor de **Ingressos**.
  - **Ingressos** é o fornecedor de dados para **Eventos**.
- **Autenticação** e **E-mails**:
  - São considerados *domínios genéricos*, onde soluções prontas podem ser utilizadas em vez de desenvolver algo do zero.

## Considerações Finais
- A análise do espaço da solução é fundamental para garantir que o sistema seja eficiente e que as relações entre os subdomínios sejam bem definidas.
- A estabilidade dos *Core Domains* é crucial para reduzir custos de manutenção e evitar bugs.
- A modelagem deve ser feita de forma a proteger os domínios principais de alterações frequentes que possam surgir de outros subdomínios.

## Conclusão
- A compreensão clara do espaço do problema e do espaço da solução é essencial para o sucesso do desenvolvimento de software no domínio do Rio & Design.
- A palestra enfatiza a importância de mapear contextos e relações entre subdomínios para um design eficaz e funcional. 

### Próximos Passos
- Continuar explorando a relação entre espaços e subdomínios na prática.
- Abordar questões táticas em futuras discussões. 

**Resumo**: A palestra fornece uma base sólida para a compreensão do espaço do problema versus o espaço da solução, destacando a importância de identificar e mapear subdomínios dentro de um software de vendas de ingressos.



---

## modulo_8_11092.mp4

# Estudo sobre Domínio do Rio & Design

## Introdução
- O foco da discussão é a diferença entre o *espaço do problema* e o *espaço da solução* no contexto do desenvolvimento de software.
- A importância de entender o *domínio do software* como sendo essencialmente o problema a ser resolvido.

## Espaço do Problema
- **Definição**: O espaço do problema refere-se à identificação e compreensão dos desafios que o software deve resolver.
- **Identificação do Domínio Principal**:
  - Exemplo: Vendas e compra de ingressos.
  - Necessidade de identificar subdomínios ou problemas menores que precisam ser resolvidos.
  
### Subdomínios
- Mesmo que dois subdomínios tenham o mesmo nome, eles podem ser diferentes devido ao seu contexto.
- Exemplo de subdomínios para o domínio de venda de ingressos:
  - **Eventos**: Inclui parceiros, clientes, detalhes do evento (data, hora, assentos).
  - **Ingressos**: QR Codes, validação de ingressos, autenticação de usuários.
  - **Autenticação**: Estabelecimento da identidade do usuário.
  - **E-mails**: Comunicação com usuários.

## Espaço da Solução
- **Definição**: O espaço da solução envolve a maneira como os subdomínios identificados serão resolvidos.
- **Core Domains**:
  - Identificação do que é mais importante para o software.
  - Exemplo: Eventos e Ingressos como Core Domains.

### Relacionamentos entre Subdomínios
- **Upstream e Downstream**:
  - Eventos dependem de Ingressos (Eventos como consumidor, Ingressos como fornecedor).
  - Necessidade de uma relação clara entre as equipes envolvidas no desenvolvimento.

### Decisões de Desenvolvimento
- Autenticação pode ser feita usando soluções prontas em vez de desenvolver do zero.
- Consideração de software de prateleira para subdomínios genéricos.
- A relação de conformidade é importante quando se utiliza soluções de terceiros.

## Riscos e Estabilidade
- A relação downstream implica riscos, pois mudanças em upstream podem impactar os downstream.
- A estabilidade dos Core Domains é crucial para reduzir custos de manutenção e bugs.

## Conclusão
- A solução envolve estabelecer relações entre os subdomínios e a compreensão de como eles interagem.
- A discussão sobre a parte tática será abordada em momentos posteriores.
- Importância de manter a visão clara sobre os problemas e soluções para o desenvolvimento eficaz de software.

## Observações Finais
- Continuar a exploração dos domínios e suas interações é fundamental.
- A prática de refletir sobre a modelagem do software pode levar a melhores soluções e maior eficiência no desenvolvimento.



---

## modulo_8_11093.mp4

# Resumo da Aula sobre Domínio do Rio & Design

## Introdução
- A discussão se concentra em duas perspectivas: **espaço do problema** e **espaço da solução**.
- *Domínio do software* é estabelecido no espaço do problema.

## Espaço do Problema
- Identifica o *domínio principal* e os *subdomínios* que precisam ser resolvidos.
- **Exemplo:** Domínio de venda de ingressos.
  - **Subdomínios identificados:**
    - Eventos
    - Autenticação
    - E-mails
    - Validação de ingressos (QR Codes)

### Características do Espaço do Problema
- É importante **identificar novos subdomínios** ou reaproveitar subdomínios existentes.
- Um *subdomínio* pode ter contextos diferentes, mesmo que o nome seja o mesmo.
- Cada subdomínio possui sua própria *linguagem ubíqua*.

## Espaço da Solução
- Neste espaço, os subdomínios do problema são analisados para determinar *como resolvê-los*.
- **Core Domains**: Identificação dos subdomínios mais importantes para o software.
  - Exemplo: Eventos e ingressos são considerados Core Domains.

### Relações entre Subdomínios
- Relações de **upstream** e **downstream** entre subdomínios:
  - **Upstream**: Fornecedor (ex: ingressos).
  - **Downstream**: Cliente (ex: eventos).
- Importância de entender essas relações para **estabilidade** e **manutenção** do sistema.
  
### Considerações sobre Autenticação e E-mails
- Autenticação pode ser uma solução genérica, onde é preferível utilizar softwares prontos.
- E-mails também podem ser tratados como soluções externas, com o sistema se adaptando a essas ferramentas.

## Riscos e Estabilidade
- As relações downstream podem causar instabilidade em *Core Domains*.
- É crucial proteger o domínio central para evitar impactos negativos de mudanças nos upstreams.

## Conclusão
- A análise do espaço do problema e do espaço da solução é essencial para entender as relações entre subdomínios e suas implementações.
- A próxima etapa envolverá uma abordagem mais tática no design do sistema.

## Reflexões Finais
- A compreensão das dinâmicas entre problemas e soluções ajuda a evitar subestimações na modelagem do software.
- A discussão é uma introdução ao mapeamento de contextos e suas relações, preparando o terreno para o design tático que será abordado em futuras aulas. 

---

### Observações Importantes
- A aula enfatizou que a visão do problema e da solução não se limita a técnicas de programação, mas aborda as relações de negócio e como o software deve ser modelado em função disso.
- A importância de ter uma comunicação clara entre equipes e subdomínios para garantir o sucesso do projeto.



---

## modulo_8_11094.mp4

# Notas de Estudo: Domain Driven Design (DDD)

## Introdução
- A palestra aborda a importância do *Domain Driven Design (DDD)*, focando em sua visão estratégica.
- O *core domain* é identificado como o "ouro" do software, onde devemos concentrar nossos esforços.

## Refinamento do Domínio
- O processo de design estratégico é flexível e pode ser modificado conforme a equipe adquire mais conhecimento sobre o problema.
- O *refinamento do domínio* é um processo esperado e necessário.

### Pontos Chave sobre Refinamento
- Mudanças no design estratégico são aceitáveis e podem trazer benefícios.
- O *livro do Evans* discute a *destilação de domínio*, que ajuda a identificar o core domain e sua visão.

## Visão do Domínio
- A visão do domínio deve se concentrar na essência do negócio, não em tecnologias específicas como aplicações web ou mensageria.
  
### Exemplo de Visão do Domínio: Venda de Ingressos
- O modelo deve permitir:
  - Compras de ingressos apenas com cartão de crédito.
  - Validação rápida dos ingressos.
  - Parcerias para criação e gestão de eventos.
  - Repartição de pagamentos entre parceiros e a organização.
  - Variação nas visões entre usuários, administradores e parceiros.

## Diagrama de Classes
- Um diagrama simplificado é usado para modelar o core domain, incluindo elementos como:
  - Eventos
  - Pagamentos
  - Ordens de compra
- A ordem de compra é central e conecta diferentes entidades.

## Camadas de Responsabilidade
- Baseado no conceito de *responsabilidades*, o livro do Evans e outros textos abordam as camadas que compõem o sistema.

### Estrutura das Camadas
1. **Potencial**: Estado atual dos recursos (clientes, assentos, eventos).
2. **Operações**: Geração e validação de ingressos.
3. **Política**: Estratégias para melhorar o negócio (descontos, gerenciamento de conflitos de compra).
4. **Decisão**: Apoio à tomada de decisões baseado em vendas.

### Dependências entre Camadas
- As dependências fluem de cima para baixo:
  - Camadas superiores podem depender de camadas inferiores.
  - Mudanças em camadas superiores impactam as inferiores, mas não o contrário.

## Importância do Core Domain
- O *core domain* é o foco para alocação de recursos e talentos.
- A compreensão das camadas e de suas responsabilidades ajuda a refinar o conhecimento sobre o problema.
  
## Conclusão
- O design do sistema deve se basear nas informações obtidas durante o processo de modelagem.
- A abordagem DDD permite um entendimento mais profundo do problema, auxiliando na criação de um design de sistema mais robusto.

### Próximos Passos
- Continuar explorando os conceitos de DDD na prática e como aplicá-los no design de sistemas.



---

## modulo_8_11095.mp4

# Notas de Estudo sobre Domain Driven Design (DDD)

## Introdução
- O DDD é uma abordagem estratégica para o design de software.
- Foco na identificação e modelagem de subdomínios e do *core domain*.

## Refinamento do Domínio
- O processo de design estratégico é flexível e pode ser modificado.
- Mudanças são esperadas e aceitas, visando o aprimoramento do modelo.
- O refinamento do domínio envolve:
  - Aprendizado contínuo sobre o problema.
  - Reorganização de subdomínios e relações.

## Destilação de Domínio
- Conceito abordado no livro de Evans, o Bluebook.
- A visão do domínio deve capturar a essência do negócio, sem se perder em detalhes técnicos.
- Exemplo de visão do domínio para venda de ingressos:
  - Permitir compras com cartão de crédito.
  - Garantir validação rápida dos ingressos.
  - Permitir que parceiros criem eventos e gerenciem lugares.

## Modelagem do Core Domain
- A modelagem deve focar no problema, não na aplicação técnica imediata.
- Um diagrama simples pode ser utilizado para representar o core domain.
- Importância de visualizar a relação entre eventos e pagamentos:
  - O pagamento é parte essencial da compra.
  
## Núcleo Segregado
- Identificação do *nucleo segregado* dentro do core domain.
- Investimento em refinamento onde os erros devem ser minimizados.
- Importância de ter os melhores desenvolvedores trabalhando no core domain.

## Camadas de Responsabilidade
- Introduzido no livro de Bushman.
- Definição de responsabilidades dentro do software:
  - **Potencial**: Recursos e capacidades atuais do negócio.
  - **Operações**: Processos essenciais, como geração e validação de ingressos.
  - **Política**: Estratégias para melhoria do negócio, como cupons de desconto.

### Dependências entre Camadas
- As camadas devem seguir uma relação de dependência de cima para baixo:
  - Camadas superiores podem depender das inferiores, mas não o contrário.
- Exemplo:
  - **Decisão**: Baseada em vendas e influenciada pelas operações e potencial.

## Considerações Finais
- Mudanças na tomada de decisão impactam diretamente o desempenho financeiro do sistema.
- A compreensão das camadas críticas ajuda a otimizar o design do sistema.
- O design do sistema deve ser uma evolução a partir da análise do domínio e suas nuances.

## Conclusão
- O DDD é uma jornada contínua de aprendizagem e adaptação.
- As práticas discutidas são fundamentais para criar sistemas que atendam efetivamente às necessidades do negócio.
- Preparação para avançar para o *system design* com uma base sólida de entendimento do problema.

## Próximos Passos
- Continuar a explorar o DDD e suas aplicações práticas.
- Aplicar os conceitos aprendidos em projetos reais para fortalecer a compreensão.



---

## modulo_8_11096.mp4

## Resumo da Aula sobre Domain Driven Design (DDD)

### Introdução
- O foco da aula é a **visão estratégica** no Domain Driven Design (DDD).
- Discussão sobre a importância de **subdomínios** e como eles se relacionam com o **core domain**.

### Refinamento do Domínio
- O processo de design estratégico não é definitivo; mudanças são esperadas.
- O conceito de **refinamento do domínio** implica em:
  - Aprender e se adaptar ao problema.
  - Rearranjar elementos e criar novos subdomínios conforme necessário.

### Destilação de Domínio
- Referência ao livro de Eric Evans (Bluebook) sobre a **destilação de domínio**.
- Importância de declarar a visão do domínio:
  - Foca na essência do problema, não em soluções tecnológicas específicas.
  - A visão deve ser uma representação clara do que se deseja alcançar.

#### Exemplos de Visão do Domínio
- Para o problema de venda de ingressos, a visão do domínio deve:
  - Permitir compras de ingressos com cartão de crédito.
  - Garantir validação rápida do ingresso.
  - Permitir que parceiros criem eventos e gerenciem lugares.
  - Representar diferentes visões dos usuários (clientes, administradores, parceiros).

### Diagrama de Classes
- Apresentação de um **diagrama de classes simplificado** para ilustrar o core domain:
  - Importância de entender a relação entre eventos e pagamentos.
  - A **ordem de compra** é central para a modelagem.

### Núcleo Segregado
- Dentro do core domain, é importante identificar o **núcleo segregado**:
  - O **núcleo** é onde devemos aplicar mais atenção e recursos.
  - A equipe deve focar em evitar erros e fazer correções rapidamente.

### Camadas de Responsabilidade
- Conceito de **camadas de responsabilidade** baseado no livro de Bushman:
  - As camadas ajudam a separar as responsabilidades dentro do software.
  - Dependências entre camadas fluem de cima para baixo:
    - **Potencial**: Estado atual dos recursos (clientes, assentos, eventos).
    - **Operações**: Processos de vendas e validação de ingressos.
    - **Política**: Estratégias de negócios, como cupons de desconto.
    - **Decisão**: Suporte à tomada de decisões, crucial para as vendas.

### Conclusão
- A compreensão dessas camadas e da visão do domínio ajuda no refinamento do conhecimento sobre o problema.
- Essa abordagem prepara o terreno para um design de sistema mais eficaz.
- A aula enfatiza a importância de aprender continuamente e adaptar-se durante o desenvolvimento.

### Próximos Passos
- Continuar a exploração do DDD em aulas futuras.
- Aprofundar o conhecimento nas estratégias de modelagem e design de sistemas. 

### Observações Finais
- A prática de DDD é um processo iterativo que envolve a colaboração contínua da equipe.
- A visão do domínio deve ser constantemente revisitada e ajustada conforme o projeto avança.



---

## modulo_8_11097.mp4

# Resumo da Aula sobre Domain Driven Design (DDD)

## Introdução ao Domain Driven Design

- O foco da aula é na **visão estratégica** dentro do DDD.
- A importância de estabelecer **subdomínios** e entender o **core domain** do software.

## Refinamento do Domínio

- O processo de design estratégico não é definitivo.
- É normal que alterações sejam necessárias ao avançar para o design tático e a implementação:
  - **Refinamento do domínio**: Aprender e se adaptar ao longo do processo.
  - Mudanças podem trazer benefícios para a modelagem.

## Destilação de Domínio

- Conceito abordado no livro de Eric Evans, conhecido como **Bluebook**.
- A visão do domínio deve focar na essência do negócio, não em tecnologias específicas:
  - Exemplo de visão: "Desenvolver uma aplicação que permita a compra de ingressos sem conflitos de lugares".

## Visão do Domínio

- A visão do domínio deve:
  - Permitir compras apenas com cartão de crédito.
  - Garantir validação rápida dos ingressos.
  - Possibilitar que parceiros criem e gerenciem eventos.
  - Representar diferentes visões de usuários (clientes, administradores, parceiros).
  - Facilitar a pesquisa de eventos e compras.

## Diagrama de Classes

- Apresentação de um diagrama simplificado que modela o **core domain**:
  - Inclui subdomínios e a relação entre eles.
  - A **ordem de compra** é central e conecta as informações.

## Camadas de Responsabilidade

- O conceito de **camadas de responsabilidade** é crucial:
  - **Potencial**: Estado atual dos recursos disponíveis.
  - **Operações**: Processos necessários para gerar e validar ingressos.
  - **Política**: Estratégias de negócios para melhorar a operação (ex.: cupons de desconto).
  
### Estrutura das Camadas

1. **Camada de Potencial**
   - Recursos como clientes e eventos.
2. **Camada de Operações**
   - Envolve a geração e validação de ingressos.
3. **Camada de Política**
   - Estratégias que guiam o negócio.
4. **Camada de Decisão**
   - Apoio à tomada de decisões, centralizada nas vendas.

## Dependências entre Camadas

- A relação entre as camadas:
  - Camadas superiores podem depender das inferiores, mas não o contrário.
  - Mudanças nas decisões afetarão diretamente a camada de vendas.

## Conclusão

- A importância de entender as **camadas** e a **declaração da visão do domínio** para refinar o conhecimento sobre o problema.
- O entendimento aprofundado das camadas críticas prepara o terreno para um **system design** mais eficaz.

## Próximos Passos

- Continuar a exploração do DDD e aplicar os aprendizados na modelagem de sistemas.
- Preparar-se para discussões futuras sobre **system design** com base nas fundações estabelecidas.

---

## Dicas de Estudo

- **Revisar os conceitos de DDD** e suas aplicações práticas.
- **Praticar a modelagem de domínios** utilizando diagramas e casos de uso.
- **Discutir em grupo** os desafios do refinamento de domínios e as camadas de responsabilidade.
- **Ler o Bluebook de Eric Evans** para aprofundar o conhecimento em DDD.



---

## modulo_8_11098.mp4

# Resumo da Aula sobre Domain Driven Design

## Introdução
- O tema da aula é *Domain Driven Design* (DDD).
- Revisão da aula anterior: diferença entre *modelo rico* e *modelo anêmico*.
- Importância do modelo rico no DDD.

## O Modelo Rico
### Identificação de Entidades
- **Pergunta-chave**: Como identificar uma entidade no DDD?
  - A entidade deve ser diferenciável de outras entidades.
  - A diferenciação é feita por meio de uma *identidade*.

### Conceito de Identidade
- Uma entidade é um objeto que possui uma identidade única.
- Essa identidade pode ser representada de várias maneiras, como:
  - Um código sequencial (ex: evento 001).
  - Um hash.
  - Data do evento (ex: 1º de janeiro de 2023).
  
### Comparação de Entidades
- Para determinar se duas entidades são iguais, é suficiente comparar suas identidades.
- Exemplo:
  - Assim como as chaves primárias em um banco de dados, a identidade da entidade é crucial para a manipulação e recuperação de dados.

## Exemplo Prático: Identidade de uma Pessoa
### Identificação de uma Pessoa
- O que torna uma pessoa única em um sistema?
  - **Nome**: Não é único, pois pode haver pessoas com nomes iguais.
  - **RG**: Também não é confiável, pois pode haver múltiplos RGs.
  - **CPF**: É a melhor escolha, pois é único e imutável para cada pessoa.

### Importância do CPF
- O CPF deve ser utilizado para identificar uma pessoa no sistema.
  - Exemplo legal: Em processos jurídicos, a identificação correta é crucial para evitar erros.

### Mitos sobre DDD e Banco de Dados
- Mito: "Banco de dados é um detalhe no DDD."
  - Realidade: O banco de dados impacta como se trabalha com entidades.
- A identidade (ex: CPF) pode não ser a mesma que a chave primária no banco de dados.
  - Pode-se usar um *ID substituto* para performance (ex: um inteiro) enquanto mantém o CPF como a identidade.

## Linguagem Ubíqua
- Ao discutir com especialistas de domínio, deve-se usar a linguagem que todos entendem.
  - Referir-se ao CPF e não ao ID.
- A comunicação clara evita ruídos e mal-entendidos.

## Resumo Final
- A identidade é um aspecto crucial das entidades em DDD.
- A próxima aula abordará como tornar o modelo rico mais expressivo com as regras de negócio.

## Conclusão
- A aula enfatizou a importância da identidade nas entidades e como isso se relaciona com o banco de dados e a comunicação no desenvolvimento de software.
- Aguarde a próxima aula para mais insights sobre DDD!



---

## modulo_8_11099.mp4

# Estudo sobre Domain Driven Design

## Introdução
- Continuação da saga sobre *Domain Driven Design* (DDD).
- Na aula anterior, foi discutida a diferença entre *modelo rico* e *modelo anêmico*.

## Modelo Rico
- O foco do modelo rico está nas *entidades*.
- As entidades são objetos que contêm informações e têm uma *identidade* única.

### Identificação de Entidades no DDD
- Para identificar uma entidade, pergunte:
  - **Eu devo diferenciar esse evento de outros?**
  - Se a resposta for sim, estamos lidando com uma entidade.
- A identidade é o que diferencia uma entidade de outra.

#### Exemplos de Identidade
- Um evento pode ter um identificador como:
  - Código próprio (ex: evento 001)
  - Hash
  - Data do evento (ex: 1º de janeiro de 2023)
- Ao comparar entidades, a identidade é o único elemento necessário.

## Chave Primária e Identidade
- A chave primária no banco de dados é similar à identidade da entidade.
- Exemplo: 
  - Para uma *pessoa*, o CPF é uma boa identidade porque é único.
  - Nome e RG não garantem a unicidade.

### Importância da Identidade
- A identidade deve ser imutável e única.
- No contexto de um sistema jurídico, identificar uma pessoa pelo CPF é essencial para evitar confusões.

## Banco de Dados e DDD
- O banco de dados é um detalhe importante na implementação do DDD.
- Pergunta comum: *O CPF pode ser uma chave primária?*
  - Sim, mas pode haver razões de performance para usar um *ID substituto*.
- O ID pode ser usado para consultas, mas a comunicação sobre identidade deve ser feita usando termos do domínio (ex: CPF).

### Comunicação no Domínio
- Ao interagir com especialistas do domínio, sempre use a identidade real (ex: CPF) em vez do ID.
- Isso evita ruídos e mal-entendidos.

## Conclusão
- A identidade é um conceito crucial nas entidades do DDD.
- Na próxima aula, será abordado como tornar o modelo rico mais expressivo com regras de negócio.

## Próximos Passos
- Estudar mais sobre como implementar regras de negócio em um modelo rico.
- Preparar-se para discutir a expressividade do modelo na próxima aula.



---

## modulo_8_11100.mp4

# Notas de Estudo: Domain Driven Design - Modelo Rico e Identidade de Entidades

## Introdução ao Modelo Rico
- O modelo rico é uma abordagem que se concentra nas entidades dentro do Domain Driven Design (DDD).
- Diferencia-se do modelo anêmico, que se preocupa mais com a persistência de dados do que com as regras de negócio.

## Identificando uma Entidade no DDD
- **Pergunta Principal**: Como identificar uma entidade em DDD?
  - Uma entidade é um objeto que precisamos manipular e que possui uma *identidade* única.
  - A identidade é o que diferencia uma entidade de outra.

### Características da Identidade
- A identidade pode ser representada de várias maneiras:
  - **Código próprio**: Exemplo: Evento 001.
  - **Hash**: Para garantir a unicidade.
  - **Data**: Importante para identificar eventos em um contexto temporal.

### Comparação de Entidades
- Para determinar se duas entidades são iguais, comparamos suas identidades, não suas propriedades.
- A identidade funciona de forma similar à *chave primária* em bancos de dados.

## Exemplos de Identidade
### Exemplo: Identidade de uma Pessoa
- **Identificadores Comuns**:
  - Nome: Não é único (ex.: várias pessoas podem ter o mesmo nome).
  - RG: Também não é confiável, pois pode haver duplicação em diferentes estados.
  - **CPF**: É o identificador ideal no Brasil, pois é único e inalterável.

### Importância do CPF
- O CPF garante que a identificação de uma pessoa seja precisa em sistemas, como em processos jurídicos.
- Utilizar o CPF evita confusões que podem surgir ao usar nomes comuns.

## Chave Primária e DDD
- O CPF pode ser considerado uma *chave primária*, mas é importante entender que:
  - A decisão sobre a chave primária pode ser influenciada por questões de *performance* no banco de dados.
  - Um **ID substituto** (geralmente um inteiro) pode ser usado para eficiência, enquanto o CPF permanece como a identidade da entidade.

### Comunicação com Especialistas do Domínio
- Ao se comunicar com especialistas do domínio, utilize a identidade da entidade (ex.: CPF) e evite termos técnicos como ID.
- O uso de uma *linguagem ubíqua* é essencial para evitar confusões e garantir que todos compreendam o mesmo conceito.

## Resumo das Características das Entidades
- **Identidade**: Algo que não muda ao longo do tempo (ex.: CPF).
- **Atributos Mutáveis**: Informações que podem mudar, como nome e peso.
- **Continuidade da Identidade**: Embora os atributos possam mudar, a identidade permanece a mesma.

## Próximos Passos
- Na próxima aula, será abordado como tornar o modelo rico mais expressivo através das regras de negócio.

---

Essas notas oferecem uma visão clara sobre o modelo rico e a identificação de entidades dentro do Domain Driven Design, preparando o estudante para compreender a importância da identidade em sistemas complexos.



---

## modulo_8_11101.mp4

# Estudo sobre Repositórios no Domain Driven Design (DDD)

## Introdução
- O conceito de repositórios dentro do DDD é diferente do que muitos estão acostumados a ver em ORMs.
- É importante entender a diferença para manter a riqueza da modelagem.

## O Papel dos Repositórios
- Os repositórios são responsáveis por:
  - Armazenar dados.
  - Realizar operações de leitura e escrita.
- **Principais conceitos**:
  - O repositório deve manter uma relação de **um para um** com o agregado.
  - O agregado não deve conhecer os detalhes de armazenamento.

## Diferenças entre Repositórios DDD e ORMs
- **ORMs (Object-Relational Mappers)**:
  - Criam repositórios que podem misturar responsabilidades com entidades.
  - Exemplo: Em um ORM, pode-se criar repositórios para diferentes entidades, como `evento` e `event.spot`.
  
- **Repositórios no DDD**:
  - O repositório lida apenas com o agregado como um todo.
  - Não deve existir um repositório para `event.spot`, pois isso dilui a responsabilidade do agregado.

## Operações em Repositórios
- As operações em um repositório incluem:
  - **Criar**: Pode ser implementado como `inserir`.
  - **Atualizar**: Normalmente não retorna nada (void).
  - **Excluir**: Também não retorna nada, mas pode lançar um erro se falhar.
  - **Consultar**: Pode retornar um ou vários eventos.
  
- **Observações Importantes**:
  - Evitar devolver entidades filhas ou objetos de valor diretamente do repositório.
  - O foco deve ser sempre o agregado.

## Variações nos Repositórios
- Dependendo da situação, o repositório pode ter métodos que não retornem apenas o agregado.
- É possível retornar objetos de valor que contêm o evento e outras informações.

## Introdução ao Data Access Object (DAO)
- O **DAO** é uma alternativa ao repositório que lida com preocupações mais específicas:
  - Permite consultas complexas e específicas, sem a necessidade de estar atrelado ao DDD.
  - Deve ser utilizado com cautela para operações de escrita.

## Comparação entre Repositórios e DAOs
- **Repositórios**:
  - Focam na consistência do agregado.
  - Devem manipular o estado completo do agregado.

- **DAOs**:
  - Podem ser usados para consultas específicas e descomplicadas.
  - Não têm a mesma preocupação com consistência que os repositórios.

## Conclusão
- É crucial entender a distinção entre os repositórios de DDD e aqueles gerados por ORMs.
- O foco deve ser sempre no agregado e na manutenção da integridade da modelagem.
- Evitar práticas erradas, como manipular entidades filhas diretamente.

## Próximos Passos
- Continuar a explorar conceitos de DDD e suas aplicações práticas.
- Estudar mais sobre a implementação de repositórios e DAOs em projetos reais.



---

## modulo_8_11102.mp4

# Estudo sobre Repositórios no Domain Driven Design (DDD)

## Introdução
No contexto do Domain Driven Design (DDD), o conceito de repositório é fundamental, mas difere do que muitos desenvolvedores conhecem através de ORMs (Object Relational Mappers). Este resumo aborda as nuances dessa diferença e como os repositórios devem ser utilizados no DDD.

## Conceito de Repositórios
- **Repositórios** são responsáveis pelo armazenamento e recuperação de agregados.
- Não devem ser confundidos com as implementações de repositórios em ORMs, que têm uma abordagem diferente.

## Funções dos Repositórios
- **Armazenamento de Dados**: O repositório é o responsável por persistir os dados dos agregados.
- **Operações**:
  - **Criação**: Inserir um novo agregado.
  - **Atualização**: Modificar um agregado existente.
  - **Exclusão**: Remover um agregado.
  - **Leitura**: Consultar agregados, podendo retornar um ou vários.

## Diferenças em Relação aos ORMs
- **Relação de um para um**: Cada agregado deve ter um repositório correspondente.
- Não deve haver repositórios separados para partes do agregado (ex.: event.spot) — o repositório deve lidar com o agregado como um todo.
- Repositórios no DDD devem focar na integridade do agregado, evitando diluir as regras de negócio em entidades filhas.

## Operações em Repositórios
- **Retornos**:
  - Operações como criar, atualizar e excluir podem retornar `void` ou lançar erros em caso de falhas.
  - Consultas podem retornar objetos de valor ou coleções.
- **Consultas Específicas**: Se necessário, pode-se criar um método para consultas mais específicas, mas sempre em relação ao agregado.

## Objetos de Valor
- Repositórios podem retornar *objetos de valor* para encapsular informações adicionais de forma imutável e livre de efeitos colaterais.
- **Exemplo**: Retornar um objeto de valor que contém informações sobre o evento e outras características, como datas.

## Data Access Object (DAO)
- **DAO** é uma alternativa aos repositórios que pode ser utilizada para consultas mais específicas.
- **Diferenças em relação ao repositório**:
  - O DAO não precisa manter a relação de intimidade com o agregado.
  - É mais flexível para consultas complexas e operações específicas, mas deve ser usado com cautela para operações de escrita.

## Considerações Finais
- **Importância do Agregado**: O foco deve sempre ser o agregado e suas regras de negócio.
- **Cuidado com ORMs**: É crucial entender que os repositórios implementados em ORMs não devem ser utilizados como os repositórios do DDD.
- O repositório deve garantir que toda a complexidade do agregado seja persistida corretamente no banco de dados.

## Resumo
- O conceito de repositório no DDD é crucial para manter a integridade e a riqueza da modelagem de domínio.
- Repositórios são responsáveis pela persistência de agregados e não devem ser confundidos com as implementações de ORMs.
- A utilização de DAOs deve ser cuidadosa e restrita a casos específicos, evitando misturar operações de escrita com regras de negócio dos agregados.

---

**Próximos Passos**: Continuar a explorar outros conceitos dentro do Domain Driven Design e como eles interagem com os repositórios e agregados.



---

## modulo_8_11103.mp4

## Notas de Estudo sobre Repositórios em Domain Driven Design (DDD)

### Introdução
- O conceito de *repositórios* em DDD é diferente do que geralmente se entende em *Object-Relational Mapping (ORM)*.
- A função dos repositórios é fundamental para a organização e a integridade dos dados dentro de um sistema que utiliza DDD.

### Repositórios e Agregados
- O repositório é responsável por armazenar e recuperar *agregados* e não deve lidar diretamente com a persistência de entidades individuais.
- **Relação de um para um**:
  - Cada agregado deve ter seu próprio repositório.
  - Exemplo: O repositório de um evento deve lidar apenas com o evento como um todo, e não com partes específicas, como *event.spot*.

### Operações do Repositório
- As operações do repositório incluem:
  - **Criar** (ou *inserir*)
  - **Atualizar**
  - **Excluir**
  - **Consultar** (pode incluir filtros, mas sempre respeitando a integridade do agregado)

#### Detalhes das Operações
- Não deve haver operações de manipulação direta de entidades filhas dentro do repositório.
- Exemplo: Evitar métodos como "reservar evento" ou "cancelar evento"; essas operações pertencem às entidades.
- A ideia é manter a *responsabilidade* e *controle* dentro do agregado.

### Consulta de Dados
- É aceitável que o repositório retorne objetos de valor em consultas, mas deve-se evitar retornar entidades filhas.
- Sempre que possível, as operações de escrita devem manipular apenas o agregado inteiro.

### DAO (Data Access Object)
- O *DAO* é uma alternativa ao repositório, focando em:
  - Consultas específicas e complexas.
  - Não possui as mesmas preocupações com agregados que o repositório.
  
#### Diferenças entre Repositório e DAO
- **Repositório**:
  - Lida com a consistência e integridade do agregado.
  - Ideal para operações de escrita.
- **DAO**:
  - Focado em consultas e desempenho.
  - Pode ser utilizado para operações específicas que não requerem a mesma estrutura do agregado.

### Considerações Finais
- A utilização de ORMs deve ser feita com cautela:
  - Os repositórios em DDD não devem ser confundidos com os repositórios gerados por ORMs, que estão mais voltados para a persistência direta.
  - O repositório DDD deve garantir que toda a complexidade do agregado seja mantida e persistida corretamente.

### Avisos Importantes
- **Atenção**: Não faça operações que interfiram diretamente nas entidades filhas fora do agregado. Isso pode levar à diluição das regras de negócio e ao controle inadequado.

### Conclusão
- A compreensão correta do papel dos repositórios e DAOs em DDD é crucial para a modelagem eficaz e a manutenção da integridade do sistema.
- O próximo passo é continuar a explorar os conceitos de DDD e suas aplicações práticas.

### Próximos Passos
- Continue estudando os conceitos de DDD e como aplicá-los em projetos reais.
- Explore a relação entre entidades, valores e agregados mais a fundo para uma melhor compreensão do modelo.



---

## modulo_8_11104.mp4

# Estudo sobre Repositórios no Domain Driven Design (DDD)

## Introdução
- O tema da aula é o conceito de **repositórios** dentro do **Domain Driven Design (DDD)**.
- É importante destacar que a abordagem de repositórios no DDD difere do que é comum em **ORMs** (Object-Relational Mappers).

## O Papel dos Repositórios
- Os repositórios são responsáveis por armazenar e recuperar agregados.
- **Agregados** e **entidades** não devem ter conhecimento sobre questões de armazenamento, mantendo a riqueza da modelagem.

### Funções dos Repositórios
- Os repositórios realizam operações de:
  - **Criação** (inserir)
  - **Leitura** (consultar)
  - **Atualização**
  - **Exclusão**
  
- Não devem ter operações específicas relacionadas a entidades filhas, como "reservar evento" ou "cancelar evento".

## Relação Um para Um
- Cada agregado deve ter um repositório correspondente.
- O repositório lida apenas com o **agregado** como um todo, não com suas partes.

### Consultas Específicas
- Consultas específicas (ex: eventos com spots não reservados) devem ser feitas através de métodos que não diluam a responsabilidade do agregado.
- O repositório deve manter o controle sobre o agregado.

## Retorno de Dados
- Operações como inserir, atualizar e excluir podem retornar tipos diferentes:
  - **Inserir** e **Atualizar**: podem retornar `void`.
  - **Consultar**: deve retornar uma coleção ou um único evento.

### Uso de Objetos de Valor
- Em algumas situações, pode ser útil retornar um **objeto de valor** que encapsule informações adicionais.
- Objetos de valor são **imutáveis** e se **autovalidam**.

## DAO (Data Access Object)
- O **DAO** é um conceito que pode ser utilizado para consultas mais específicas, sem se preocupar com a estrutura do agregado.
- O DAO pode ser usado para:
  - Consultas complexas para relatórios.
  - Operações de escrita em casos de conveniência, mas deve ser feito com cautela.

## Diferenças entre Repositórios e ORMs
- Repositórios no DDD focam na persistência do agregado completo, enquanto ORMs tendem a tratar entidades de forma anêmica.
- A intimidade do repositório deve ser com o agregado, e não com a tabela do banco de dados diretamente.

## Conclusão
- Compreender a diferença entre repositórios em DDD e ORMs é essencial para garantir a consistência e a riqueza das regras de negócio dentro de uma aplicação.
- Sempre mantenha as operações de escrita e leitura focadas no agregado, evitando operações diretas nas partes de um agregado.

## Atenções Finais
- Evite fazer operações que não estejam relacionadas diretamente ao agregado dentro do repositório.
- Reforce a ideia de que a responsabilidade de manipulação dos dados deve ser sempre do agregado para manter a integridade da modelagem.



---

## modulo_8_11105.mp4

# Resumo da Aula sobre Padrões de Arquitetura e Design Patterns no DDD

## Introdução
- A aula aborda **padrões de arquitetura** e **design patterns** utilizados no **Domain-Driven Design (DDD)**.
- O foco inicial será nos **design patterns** antes de discutir os padrões de arquitetura.

## Design Patterns
### Definição
- Não existem design patterns específicos para DDD.
- Qualquer padrão pode ser aplicado desde que se compreenda o problema que ele resolve.

### Cuidados
- Evitar a *síndrome da paternite* (uso excessivo de padrões sem necessidade), que pode complicar o design.

### Padrões de Design Comuns
1. **Factory**
   - Utilizado para criar **agregados**.
   - Permite diferentes formas de instanciar um objeto através de métodos de fábrica (factory methods).
   - Pode ser aplicado em:
     - **Agregados**
     - **Repositórios**
     - **Objetos de valor**
     - **Serviços de domínio**
   
2. **Specification**
   - Muito utilizado para validação de dados.
   - Permite combinar regras de validação (ex: verificar se um campo não é vazio, não é nulo e é um número).
   - Implementação de regras de negócio fora do agregado, tornando o sistema mais modular.

3. **Mediator**
   - Usado para tratamento de eventos.
   - Detalhes sobre sua aplicação serão abordados na parte prática.

## Padrões de Arquitetura
### Importância da Arquitetura em Camadas
- Separação clara entre:
  - **Apresentação do usuário**
  - **Regras de negócio**
  - **Banco de dados**
  
### Arquitetura Hexagonal
- Mantém o *domínio isolado* de tecnologias externas como frameworks e bibliotecas.
- *Ports and Adapters*: conceito que permite que a aplicação não dependa de outras tecnologias, mas sim o contrário.

### Benefícios
- Protege as regras de negócio.
- Facilita a implementação de DDD ao manter as responsabilidades bem definidas.
- Previne dependências fortes com ORMs e frameworks, permitindo uma modelagem rica do domínio.

## Conclusão
- Resumo dos principais padrões discutidos:
  - **Factory**
  - **Specification**
  - **Mediator**
- Importância de implementar uma **arquitetura em camadas** e **arquitetura hexagonal** para uma modelagem eficaz do domínio.

## Próximos Passos
- Revisar os design patterns mencionados.
- Preparar-se para a implementação da arquitetura em camadas na próxima aula. 

**Até a próxima!**



---

## modulo_8_11106.mp4

# Resumo da Aula sobre Padrões de Arquitetura e Design Patterns no DDD

## Introdução
- A aula aborda questões sobre **padrões de arquitetura** e **design patterns** no contexto do **Domain-Driven Design (DDD)**.
- O instrutor menciona que não há necessidade de discutir cada padrão separadamente, mas sim oferecer uma visão geral.

## Padrões de Design
### Definição
- **Design patterns** são soluções reutilizáveis para problemas comuns em design de software.
- Não existem **design patterns** específicos para DDD; pode-se usar padrões existentes, como os do **Gang of Four** ou os mencionados por **Martin Fowler**.

### Ponto Importante
- Evitar a *síndrome da paternite*: usar padrões apenas por usá-los, o que pode complicar o design.

### Exemplos de Design Patterns Comuns
1. **Factory**
   - Utilizado para criar agregados.
   - Permite diferentes formas de instanciar um agregado com base em parâmetros.
   - Pode ser implementado como um **factory method**.
   - Também pode ser usado para gerar repositórios e objetos de valor.

2. **Specification**
   - Muito citado no livro de **Eric Evans**.
   - Usado para validação de dados e regras de negócio.
   - Permite combinar regras de validação (ex: verificar se um campo é vazio, nulo ou um número).
   - Útil para criar regras de negócio sem poluir o agregado principal.

3. **Mediator**
   - Utilizado para o tratamento de eventos.
   - Será abordado na parte prática da aula.

## Padrões de Arquitetura
### Importância
- **Arquitetura em Camadas** é essencial para isolar o domínio do software e evitar a *invasão do domínio* por tecnologias externas.
- É fundamental separar a lógica de apresentação, regras de negócio e acesso a dados.

### Arquitetura Hexagonal
- Proposta para manter o núcleo do negócio protegido.
- Define a interação através de **ports and adapters**.
- Permite que a aplicação central não dependa de frameworks ou bibliotecas, mas que estes dependam da aplicação.

### Estrutura Recomendada
- A aplicação deve incluir:
  - **Entidades**
  - **Agregados**
  - **Repositórios**
  - **Serviços de Domínio**
- Essa estrutura protege as regras de negócio e facilita a manutenção e evolução do software.

## Resumo Final
- **Design Patterns** importantes a serem revisados:
  - **Factories**
  - **Specification**
  - **Mediator**
- A implementação de **arquitetura em camadas** e **arquitetura hexagonal** é crucial para um bom design em DDD.
- A separação de responsabilidades é fundamental para uma modelagem rica e eficaz do domínio.

## Conclusão
- O instrutor incentiva a continuidade do aprendizado e prática dos conceitos abordados.
- A próxima aula terá uma abordagem mais prática sobre os temas discutidos.



---

## modulo_8_11107.mp4

# Resumo da Aula sobre Padrões de Arquitetura e Design Patterns no DDD

## Introdução
- O foco da aula é discutir **padrões de arquitetura** e **design patterns** utilizados no **Domain Driven Design (DDD)**.
- O palestrante optou por discutir design patterns primeiro, antes de abordar padrões de arquitetura.

## Design Patterns

### Definição e Importância
- Não existem design patterns específicos obrigatórios para DDD; qualquer padrão pode ser aplicado, desde que se compreenda seu propósito.
- **Cuidado com a síndrome da "paternite"**: usar padrões de forma inadequada pode complicar o projeto.

### Padrões de Design Usados com Frequência

1. **Factories**
   - Usadas para a criação de **agregados**.
   - Permitem criar instâncias de forma flexível, utilizando métodos como **factory method**.
   - Exemplos de uso:
     - Criação de objetos de valor.
     - Geração de repositórios.
     - Instanciação de serviços de domínio.

2. **Specification**
   - Utilizado para a **validação de dados**.
   - Permite combinar regras de validação (AND/OR).
   - Exemplo prático:
     - Regras de aposentadoria: criação de diferentes specifications que verificam se um funcionário pode se aposentar com base em várias regras.

3. **Mediator**
   - Usado para o tratamento de eventos.
   - Detalhes práticos a serem discutidos em aulas futuras.

## Padrões de Arquitetura

### Arquitetura Hexagonal
- Fundamental para evitar a **invasão do domínio**, onde o domínio se torna dependente de tecnologias externas.
- Necessidade de separar:
  - **Camada de apresentação** (UI)
  - **Regras de negócio** (domínio)
  - **Acesso a dados** (banco de dados)

### Importância da Arquitetura em Camadas
- Protege as regras de negócio, garantindo que a aplicação seja independente de frameworks ou bibliotecas externas.
- O conceito de **ports and adapters** é fundamental:
  - Um lado dirige (interações externas) e o outro é dirigido (lógica de negócios).
  
### Considerações Finais
- A implementação de DDD requer uma boa separação de responsabilidades e uma arquitetura clara.
- Os principais pontos a serem lembrados:
  - Utilização de **factories** e **specifications**.
  - Importância da **arquitetura em camadas** e da **arquitetura hexagonal**.

## Dever de Casa
- Pesquisar mais sobre os padrões de design mencionados:
  - **Factories**
  - **Specifications**
  - **Mediator**
- Preparar-se para a implementação prática de arquitetura em camadas. 

## Conclusão
- A aula enfatizou a importância de entender e aplicar corretamente padrões de design e arquitetura para a modelagem eficaz do domínio em DDD.
- O palestrante encerra com um convite para continuar a jornada de aprendizado.



---

## modulo_8_11108.mp4

# Resumo da Aula sobre Padrões de Arquitetura e Design Patterns no DDD

## Introdução
- Aula sobre *padrões de arquitetura* e *design patterns* no contexto do Domain-Driven Design (DDD).
- Diferenciação entre padrões de arquitetura e design patterns.

## Padrões de Design (Design Patterns)

### Importância dos Design Patterns
- Não existem *design patterns* específicos para DDD; diversos padrões podem ser aplicados.
- Exemplos de fontes de padrões: *Gang of Four* e livros de Martin Fowler.
- Importância de entender o problema que o padrão resolve.

### Design Patterns Comuns em DDD

1. **Factory**
   - Utilizado para a criação de *agregados*.
   - Permite múltiplas formas de instanciar um objeto, evitando complexidade.
   - Exemplo: Factory Method, onde pode haver métodos com o mesmo nome, mas com diferentes parâmetros.
   - Aplicações:
     - Criar objetos de valor.
     - Gerar repositórios e serviços de domínio.

2. **Specification**
   - Usado para validação de dados.
   - Permite combinar regras de validação de forma flexível.
   - Exemplo: Regras para verificar se um campo é vazio, nulo ou se é um número.
   - Pode ser usado para encapsular regras de negócio, como a validação de aposentadoria.

3. **Mediator**
   - Usado para tratamento de eventos.
   - Será abordado na parte prática da aula.

## Padrões de Arquitetura

### Arquitetura Hexagonal
- Importância de isolar o domínio da aplicação de tecnologias específicas (ex.: frameworks).
- Conceito de *invasão do domínio*: quando o domínio depende de tecnologias externas.
  
### Estrutura da Arquitetura
- A arquitetura deve ser em camadas para separar:
  - Apresentação do usuário
  - Regras de negócio
  - Acesso a dados
  
### Ports and Adapters
- A arquitetura hexagonal é também conhecida como *ports and adapters*.
- A ideia é que a aplicação não dependa de frameworks ou tecnologias externas.
- Protege as regras de negócio essenciais e permite que a aplicação seja utilizada por diferentes clientes ou serviços (banco de dados, e-mail, mensageria).

## Conclusão
- Resumo dos padrões discutidos:
  - **Factories**: criação de objetos.
  - **Specification**: validação de dados e regras de negócio.
  - **Mediator**: tratamento de eventos.
  - **Arquitetura em camadas e hexagonal**: fundamental para DDD.
  
- A importância de entender e aplicar esses padrões corretamente para evitar a complexidade desnecessária no sistema.

## Ações Finais
- Recomenda-se pesquisar mais sobre os padrões discutidos.
- Preparação para a parte prática da aula.

---

### Observações
- Estar atento à implementação de DDD com uma modelagem rica do domínio.
- Evitar a dependência excessiva de ORMs e frameworks.

--- 

*Pronto para continuar a jornada no DDD! Até a próxima.*



---

## modulo_8_11109.mp4

# Resumo da Aula sobre DDD e Microserviços

## Introdução
Na aula de hoje, discutimos a importância do *Domain-Driven Design* (DDD) na construção de micro-serviços. Vamos explorar como o DDD ajuda a identificar e organizar as aplicações dentro de um sistema.

## DDD e Micro-serviços
- O DDD é uma abordagem que facilita a identificação de micro-serviços necessários para resolver um problema de negócio.
- Ele promove uma visão mais clara sobre a divisão entre as aplicações, permitindo um maior desacoplamento.

### Vantagens do DDD
- **Desacoplamento**: Permite que partes do sistema, como a geração de ingressos e eventos, operem de forma independente.
- **Escalabilidade**: Micro-serviços podem ser escalados de maneira independente, evitando gastos desnecessários.

### Contextos e Agrupamentos
- A ideia central é criar *contextos* coesos, que agrupam problemas que precisam ser resolvidos juntos.
- A separação clara entre esses contextos pode resultar na criação de múltiplos micro-serviços.

## Refinamento do Modelo
1. **Análise de Regras de Negócio**: O modelo deve ser refinado conforme se obtém mais entendimento das regras de negócio.
2. **Interação com Domain Experts**: As decisões sobre a estrutura dos serviços devem ser baseadas em informações coletadas de especialistas no domínio.
3. **Flexibilidade**: É possível ajustar a estrutura ao longo do tempo, como juntar ingressos com eventos ou criar novos subdomínios.

## Comunicação entre Aplicações
- A relação entre os contextos pode determinar o tipo de comunicação entre as aplicações:
  - **Assíncrona**: Quando a comunicação não precisa ser imediata.
  - **Síncrona**: Quando a comunicação requer uma resposta imediata.

## Conclusão
- O DDD é uma metodologia essencial para modelar soluções e identificar micro-serviços.
- Através da modelagem estratégica, conseguimos compreender melhor os contextos e as implicações de nossas decisões de design.

### Próximos Passos
- Continuar explorando o DDD e suas aplicações práticas no desenvolvimento de micro-serviços.

**Maravilha, pessoal! Vamos evoluindo aqui na nossa saga. Até a próxima!**



---

## modulo_8_11110.mp4

# Resumo da Aula sobre Domain-Driven Design (DDD) e Microserviços

## Introdução
- O tema principal da aula é a relação entre *Domain-Driven Design (DDD)* e *microserviços*.
- O DDD é abordado como uma metodologia que ajuda a identificar e construir microserviços.

## Importância do DDD na Identificação de Microserviços
- **Identificação de micro-serviços**: O DDD auxilia na visualização das necessidades para a construção de microserviços dentro de um domínio.
- **Divisão de aplicações**: É sugerido que uma visão mais assertiva sobre a divisão de aplicações pode ser obtida a partir da análise dos subdomínios.

## Agrupamento e Desacoplamento
- O agrupamento de funcionalidades permite um *maior desacoplamento* entre diferentes partes da aplicação.
- Exemplo prático:
  - **Geração de ingressos**: Pode ser desacoplada dos eventos, permitindo que a geração de QR Codes ocorra independentemente.

## Escalabilidade
- Cada aplicação pode ser escalada de forma independente, evitando gastos desnecessários.
- Se as funcionalidades estivessem dentro do mesmo domínio, escalá-las juntas poderia levar a *ineficiências*.

## Coesão e Acoplamento
- É importante ter *coesão* dentro dos contextos:
  - Agrupamento de problemas que precisam ser resolvidos juntos.
- O acoplamento entre os contextos não deve ser zero, mas deve ser bem definido para que a separação de problemas seja clara.

## Refinamento do Modelo
- O modelo pode ser refinado com base nas regras de negócio e na interação com *domain experts*.
- As decisões sobre microserviços podem mudar conforme o entendimento do problema evolui.

## Comunicação entre Microserviços
- A comunicação entre microserviços pode ser:
  - **Assíncrona**: Quando não é necessário aguardar a resposta imediata.
  - **Síncrona**: Quando a resposta imediata é necessária.
- A escolha entre esses tipos de comunicação depende do contexto e da relação entre as aplicações.

## Conclusão
- O DDD é uma metodologia essencial para a modelagem de microserviços.
- A modelagem estratégica é suficiente para entender os contextos e as implicações de se tornar um microserviço.
- A aula conclui com a ideia de que a compreensão dos subdomínios e suas interações é crucial para a arquitetura de sistemas baseada em microserviços.

## Próximos Passos
- Continuar explorando os conceitos de DDD e microserviços nas futuras aulas.

---

### Dicas de Estudo
- **Revisar os conceitos de DDD**: Entender os princípios fundamentais e como aplicá-los na prática.
- **Estudar exemplos práticos**: Analisar casos de uso reais onde DDD foi utilizado para implementar microserviços.
- **Discutir em grupos**: Trocar ideias com colegas sobre a aplicação do DDD em diferentes cenários de negócios.



---

## modulo_8_11120.mp4

## Resumo da Aula sobre Mapeamento em Entidade Relacional

### Introdução
- A aula se concentra no **mapeamento em entidade relacional** utilizando o microRM.
- O uso de **decorators** é mencionado como prática comum em frameworks como **Hibernate** e **Doctrine**.

### Mapeamento de Entidades
- O mapeamento pode ser feito diretamente nas entidades, mas isso pode poluir o domínio.
- A proposta é utilizar uma abordagem separada para lidar com o mapeamento.
  
### Estrutura do Entity Schema
- Criação de um **Entity Schema** para definir os campos da entidade.
- Exemplo prático com a entidade **partner**.
- Campos a serem definidos:
  - `name` (do tipo `varchar`)
  - `id` (chave primária, pode ser do tipo `uuid` ou `varchar`)

### Configuração do MicroRM
- Início da instância do MicroRM com o driver MySQL.
- Importação de entidades e schemas.
- Importância de usar **async** para operações que retornam promessas.

### Criação e Persistência de Dados
- Uso do **Entity Manager** para persistir entidades.
  - O método `persist` apenas gerencia a entidade, não a salva no banco.
  - O conceito de **Unit of Work** é introduzido para gerenciar transações.
- Necessidade de usar `await` em promessas para garantir a execução correta.

### Testes e Validações
- Criação de um arquivo de teste `schemas.spec.ts` para validar a criação de um partner.
- Importância de criar o schema do banco de dados antes de executar os testes.
- Consultas ao banco de dados para verificar dados persistidos.

### Problemas Comuns
- O **Entity Manager** pode manter objetos em cache, levando a resultados inesperados.
- Necessidade de usar `clear` para limpar o cache antes de realizar consultas.
- A integridade do modelo deve ser mantida tanto na persistência quanto na recuperação de dados.

### Conclusões e Recomendações
- Melhorar o mapeamento relacional é essencial para garantir que o modelo de domínio seja corretamente persistido e recuperado.
- Atenção especial deve ser dada ao uso do **Unit of Work** para evitar problemas durante a manipulação de dados.

### Dicas para Estudo
1. **Revisar conceitos de ORM** e como eles interagem com bancos de dados.
2. **Praticar a criação de entidades e schemas** utilizando o microRM.
3. **Familiarizar-se com a sintaxe do TypeScript** e a utilização de promessas.
4. **Testar diferentes cenários** de persistência e recuperação de dados para entender o comportamento do Entity Manager.

### Palavras-Chave
- _Mapeamento Relacional_
- _Entity Schema_
- _Entity Manager_
- _Unit of Work_
- _Decorators_



---

## modulo_8_11121.mp4

# Resumo da Aula: Mapeamento em Entidade Relacional com microRM

## Introdução
Nesta aula, o foco foi o **mapeamento de entidades** utilizando o microRM, abordando como evitar a poluição do domínio por influências tecnológicas e mantendo a integridade do modelo de dados.

## Mapeamento de Entidades
- O mapeamento pode ser feito diretamente nas entidades utilizando **decorators**.
- A utilização de bibliotecas como **Hibernate** e **Doctrine** é comum, mas é preciso evitar a mistura de lógica de domínio com tecnologia.

### Estrutura do Mapeamento
- Usamos um **Entity Schema** para definir os campos da entidade.
- Exemplos de tipos de campos:
  - `String`: mapeado como `varchar`.
  - `ID`: pode ser uma *primary key* e pode ser definido como `uuid` ou `char`.

## Implementação do Partner Schema
- Criar uma instância do **Partner Schema** que representa a entidade `partner`.
- Os campos definidos são:
  - `name`: tipo `varchar`.
  - `id`: tipo `uuid`, com tamanho 36.

### Estrutura de Diretórios
- As classes de schema são organizadas na pasta `infra`, dentro da pasta `DB`.

## Testando a Criação de um Partner
1. Criar um arquivo de teste chamado `schemas.spec.ts`.
2. Importar o driver do MySQL e configurar a conexão.
3. Utilizar **Entity Manager** para gerenciar as entidades.
   - O método `persist` apenas gerencia a entidade, sem gravar no banco de dados.
   - O método `flush` é necessário para persistir as alterações.

### Exemplo de Código
- Iniciar uma instância do microRM e criar um `partner` utilizando:
  ```typescript
  const partner = await partner.create({ name: 'Nome do Partner' });
  ```

## Problemas e Soluções
- **Erro de Conexão**: Ajustar o `host` e a `porta` no código de configuração.
- **Tabela Inexistente**: Usar `orm.schema.refreshDatabase` para criar as tabelas automaticamente.
- **Persistência e Recuperação**: O `persist` mantém o objeto na memória, o que pode causar confusão na recuperação dos dados.

### Importância do Clear
- Utilizar `clear` para limpar o **Unit of Work** antes de realizar consultas, evitando que o Entity Manager retorne objetos da memória ao invés de acessar o banco de dados.

## Considerações Finais
- Atenção ao realizar testes com o **data mapper**.
- Garantir que o modelo rico seja persistido e recuperado corretamente.
- Continuar a adaptação do mapeamento relacional para assegurar a integridade do modelo.

## Conclusão
A aula abordou o mapeamento relacional utilizando microRM, destacando práticas para evitar problemas comuns e garantindo a integridade do modelo de dados. A próxima aula continuará a desenvolver essas práticas.



---

## modulo_8_11122.mp4

# Resumo da Aula: Mapeamento em Entidade Relacional com microRM

## Introdução ao Mapeamento Relacional
- O foco da aula é o *mapeamento em entidade relacional* utilizando o microRM.
- O uso de *decorators* para mapear entidades é comparado a frameworks como Hibernate e Doctrine.
- A preocupação com a poluição do domínio pela influência da tecnologia é destacada.

## Estrutura do Mapeamento
- O mapeamento é realizado através de um *Entity Schema*.
- Campos podem ser definidos, por exemplo:
  - `name` como *varchar*.
  - `id` como *primary key* (UUID ou CHAR).
- É importante que o mapeamento não gere valores automaticamente, como o UUID.

### Exemplo Prático: Partner Schema
- Criação de um `partnerSchema` a partir do *Entity Schema*.
- Importação da entidade `partner` do domínio.
- Localização do esquema dentro da pasta `infra` e `DB`.

## Testes e Estrutura do Código
- Criação de um arquivo de teste `schemas.spec.ts` para validar a criação de um partner.
- Importação do driver MySQL e definição das configurações do banco de dados.
- Utilização do *Entity Manager* para gerenciar entidades.

### Fluxo de Criação de um Partner
1. Iniciar uma instância do microRM.
2. Configurar o banco de dados e as entidades.
3. Criar um partner utilizando `partner.create`.
4. Persistir a entidade com `entityManager.persist`.

## Problemas e Soluções
- O `persist` não atualiza o banco de dados diretamente; é necessário o uso do *Unit of Work* e o método `flush`.
- O teste inicial falha devido à falta da tabela `partner`.
- O método `orm.schema.refreshDatabase` pode ser utilizado para criar automaticamente o esquema.

### Consultando o Banco de Dados
- Após a persistência, é possível consultar a tabela `partner` no banco de dados.
- Importância do método `toString` no *value object* para evitar problemas durante a persistência.

## Desafios com a Recuperação de Dados
- Ao recuperar dados, o *Entity Manager* pode não consultar o banco se a entidade já estiver em cache.
- Uso do método `clear` para limpar o *Unit of Work* e forçar uma nova consulta ao banco de dados.

## Conclusão
- É crucial adaptar o mapeamento para garantir que o modelo rico seja persistido e recuperado corretamente.
- A aula enfatiza a importância de testar e validar o comportamento do mapeamento relacional com atenção às particularidades do microRM.

## Dicas de Estudo
- Revise os conceitos de *decorators* e *Entity Schema*.
- Pratique escrevendo e testando o código para criação e recuperação de entidades.
- Analise os problemas comuns ao trabalhar com ORMs e como solucioná-los.
- Teste diferentes configurações e observe os comportamentos do *Entity Manager*.



---

## modulo_8_11123.mp4

# Resumo da Aula sobre Domain Driven Design

## Introdução
Nesta aula, o professor discute a implementação de repositórios dentro do contexto de Domain Driven Design (DDD). O foco é a criação e configuração de repositórios para diferentes entidades, além de conceitos importantes sobre mapeamento e persistência de dados.

## Estrutura dos Repositórios

### Interfaces
- Foi adicionada uma interface para o repositório de *customer*.
- A interface de *customer* não apresenta mudanças significativas em relação às de *partner* e *evento*.
- O estilo de nomeação foi alterado de ponto para traço, utilizando o *kebab case* (tudo minúsculo).

### Repositório de Evento
- O repositório é implementado apenas para a entidade *evento*, sem repositórios específicos para *event session* e *event spot*.
- A persistência dos dados é feita em uma transação única, salvando todos os dados relacionados ao evento de uma vez.

## Mapeamento Relacional

### Tipos e Identificadores
- Os tipos de dados devem ser definidos adequadamente para cada entidade:
  - **CPF** do *customer*: deve ser um objeto de valor único no banco de dados.
  - Identificadores (*ID*) para eventos e seções são todos definidos como `varchar(36)`.

### Unicidade e Chaves
- O CPF do *customer* é uma chave natural e deve ser único.
- O campo de chave deve ser tratado como um tipo personalizado no mapeamento.

### Relacionamentos
- Implementação de relacionamentos entre entidades:
  - Um para muitos (*one to many*): exemplo de *event* para *event sessions*.
  - Muitos para um (*many to one*): mapeamento inverso para *event session*.
- As anotações de mapeamento definem como os relacionamentos devem ser tratados no banco.

## Carregamento de Dados

### Abordagens de Carregamento
- **Eager Loading** (carregamento antecipado): os dados relacionados são carregados junto com a entidade principal.
- **Lazy Loading** (carregamento preguiçoso): os dados são carregados sob demanda.
- Recomenda-se o uso de *eager loading* para garantir que o agregado esteja completo ao ser retornado.

### Políticas de Cascata
- Políticas de persistência, atualização e exclusão devem ser definidas para os relacionamentos:
  - **Persist**: cria todos os dados relacionados.
  - **Update**: atualiza todos os dados relacionados.
  - **Exclusão**: exclui todos os dados relacionados.

## Conclusão
- A aula conclui com a promessa de testar a persistência das entidades na próxima sessão.
- O professor incentiva os alunos a continuarem explorando o conteúdo e a praticar o que foi aprendido.

## Pontos Importantes para Estudo
- Compreender a importância das interfaces e a nomeação adequada dos repositórios.
- Familiarizar-se com os conceitos de mapeamento relacional e tipos personalizados.
- Estudar as diferentes abordagens de carregamento de dados e suas implicações no desempenho.
- Analisar as políticas de cascata e como elas afetam a manipulação de entidades no banco de dados.

### Dicas de Estudo
- Revisar os conceitos de *Domain Driven Design* e como eles se aplicam a repositórios e entidades.
- Praticar a implementação de repositórios em projetos pessoais para solidificar o conhecimento.
- Discutir com colegas sobre as melhores práticas de mapeamento e persistência de dados.



---

## modulo_8_11124.mp4

# Resumo da Aula sobre Domain Driven Design

## Introdução
- Continuação da série sobre **Domain Driven Design**.
- Discussão sobre a implementação de repositórios.

## Interfaces dos Repositórios
- Adicionada uma interface para o repositório de **Customer**.
- Mudanças nas interfaces:
  - Alteração do ponto (.) para traço (-) na nomenclatura.
  - Adoção do estilo **kebab case** (tudo minúsculo).
- Repositórios de **Event Session** e **Event Spot** não foram criados, apenas o repositório de **Event**.

## Abstração dos Repositórios
- Sugestão de criar um repositório abstrato para evitar repetição de código.
- O repositório pode ser estendido para incluir métodos comuns.

## Persistência e Mapeamento
- O repositório deve lidar com a persistência de um evento e seus componentes em uma única transação.
- Utilização de **data mapper** e **unit of work** para facilitar o salvamento dos dados.
- Importância de criar tipos para documentação no banco de dados, como:
  - CPF do **Customer** deve ser único.
  - IDs (event ID, event section ID, event spot ID) definidos como **varchar(36)**.

## Relacionamentos entre Entidades
- Mapeamento de relacionamentos:
  - **One-to-many** e **many-to-one**.
- Exemplo de relacionamento:
  - **Event** com **Event Sessions** e **Event Spots**.

### Considerações sobre Mapeamento
- O uso de *annotations* para definir relacionamentos e chaves estrangeiras.
- Importância de omitir campos não necessários durante a manipulação da entidade.
- Estrutura de chaves personalizadas para IDs, utilizando **string**.

## Carregamento de Dados
- Discussão sobre as duas formas de carregamento em **ORMs**:
  1. **Eager loading** (carregamento imediato).
  2. **Lazy loading** (carregamento retardado).
- Recomenda-se o uso de **eager loading** para garantir que todos os dados necessários sejam carregados.

## Políticas de Cascata
- Definição de políticas de cascata para operações de persistência:
  - **Persist**: cria todos os registros relacionados.
  - **Update**: atualiza os registros relacionados.
  - **Excluir**: remove todos os registros relacionados.
  
## Conclusão
- O código será disponibilizado para consulta.
- Próxima aula focará em testar a persistência das implementações discutidas.

## Pontos Importantes para Estudo
- **Domain Driven Design**: Compreender os princípios e práticas.
- **Repositórios**: Entender a importância da abstração e a estrutura dos repositórios.
- **Persistência**: Saber como o data mapper e unit of work funcionam na prática.
- **Relacionamentos e Mapeamento**: Estar ciente das anotações e da configuração dos relacionamentos.
- **Carregamento de Dados**: Diferenciar entre eager e lazy loading e suas implicações.
- **Políticas de Cascata**: Saber como gerenciar operações de persistência em relacionamentos.



---

## modulo_8_11125.mp4

# Resumo da Aula sobre Domain Driven Design

## Introdução
- Continuação do estudo sobre **Domain Driven Design (DDD)**.
- Discussão sobre a implementação de repositórios, focando em **interfaces** e **mapeamento**.

## Interfaces de Repositório
- Foi adicionada uma nova interface para o repositório de **customer**.
- Mudanças na nomenclatura das interfaces:
  - Passagem de ponto para traço na nomenclatura.
  - Utilização do *kebab case* (tudo em minúsculas).
  
### Repositórios de Evento
- Não foram criados repositórios separados para **event session** e **event spot**; apenas o repositório de **evento** é necessário.
- Sugestão de criação de um repositório abstrato:
  - Métodos comuns podem ser definidos uma única vez.
  
## Persistência de Dados
- O repositório salva todos os dados em uma única transação.
- Importância do uso de **data mapper** e **unit of work** para simplificar a persistência.
- Necessidade de criar tipos para mapear corretamente os dados no banco de dados.

### Exemplo de Mapeamento
- **Customer:**
  - O **CPF** deve ser único no banco de dados.
  - Uso de *custom type* para lidar com objetos de valor.
- **Eventos:**
  - Configurações de campos como ID, nome, descrição e data.
  - Relacionamentos entre entidades devem ser bem definidos.

## Relacionamentos entre Entidades
- Relacionamentos **one-to-many** e **many-to-one**:
  - Importância de mapear corretamente as chaves estrangeiras.
  - Utilização de anotações para definir o comportamento do ORM.
  
### Carregamento de Dados
- Dois tipos de carregamento em ORMs:
  - **Eager Loading** (carregamento completo).
  - **Lazy Loading** (carregamento retardado).
- Preferência por **Eager Loading** para garantir que os dados sejam carregados na forma completa.
  
### Políticas de Cascateamento
- Definição de políticas para ações como persistência, atualização e exclusão:
  - **Persistência:** Cria todos os registros relacionados.
  - **Atualização:** Atualiza todos os registros relacionados.
  - **Exclusão:** Remove todos os registros relacionados.

## Conclusão
- Discussão sobre as configurações e o código que será disponibilizado.
- Preparação para a próxima aula, onde serão testadas as operações de persistência.

### Próximos Passos
- Testar a persistência das entidades na próxima aula.
- Continuar a exploração do **Domain Driven Design**. 

## Observações Finais
- A importância de manter a qualidade do código e a estrutura correta das entidades ao trabalhar com DDD.
- A prática e a experimentação são fundamentais para a compreensão dos conceitos apresentados.



---

## modulo_8_11126.mp4

# Resumo da Aula sobre Domain Driven Design

## Introdução
- Continuação da discussão sobre **Domain Driven Design** (DDD).
- Foco na criação e implementação de repositórios.

## Estruturas de Repositórios
- Adição de uma interface para o repositório de **Customer**.
- Repositórios de **Partner** e **Event** não apresentam mudanças significativas.

### Alterações nas Interfaces
- Mudança na nomenclatura de "ponto" para "traço" nas interfaces.
- Uso do estilo **kebab case** (tudo em minúsculas).

## Repositório de Eventos
- Eventos possuem múltiplas seções e locais, mas somente um repositório.
- Importância do **data mapper** para salvar informações em uma única transação.

### Persistência de Dados
- O repositório deve lidar com a persistência de eventos e suas seções de forma integrada.
- Necessidade de criar tipos para documentar os dados no banco de dados.

## Mapeamento Relacional
- **CPF** do **Customer** deve ser único no banco de dados.
- Definição de tipos personalizados para as chaves primárias e estrangeiras.

### Estrutura dos Eventos
- Campos a serem definidos:
  - **ID**: `varchar(36)`
  - **Nome**: `string(255)`
  - **Descrição**: texto sem limite de tamanho.
  - **Data**: tipo data.
  - **Publicação**: booleano (inicialmente falso).
  - **Total de Spots**: começa em zero.
  - **Spots Reservados**: também começa em zero.

## Relacionamentos em DDD
- Definição dos relacionamentos entre entidades:
  - Um para muitos (one-to-many).
  - Muitos para um (many-to-one).

### Políticas de Carregamento
- **Eager Loading**: Carregamento imediato de todos os dados relacionados.
- **Lazy Loading**: Carregamento adiado, que pode economizar memória.

### Configuração de Cascade
- Políticas de **cascade** para persistência, atualização e exclusão das entidades.
- Impacto total na exclusão de eventos e seus relacionados.

## Considerações Finais
- Revisão das configurações e implementação dos repositórios.
- Próxima aula focará em testes de persistência para garantir que tudo funcione corretamente.

## Dicas de Estudo
- **Revisar a diferença entre Eager e Lazy Loading**.
- **Familiarizar-se com o conceito de data mapper** e sua importância no DDD.
- **Praticar a implementação de repositórios** com base nos conceitos discutidos.

### Conclusão
- Importância de entender as relações entre entidades e como elas são mapeadas no banco de dados.
- Preparação para a próxima aula, onde serão testadas as implementações discutidas.



---

## modulo_8_11127.mp4

# Estudo sobre Domain Driven Design: Camada de Aplicação

## Introdução
Neste módulo, discutiremos a camada de aplicação dentro do contexto do Domain Driven Design (DDD). Faremos uma conexão entre as regras de negócio e as necessidades dos usuários, enfatizando a importância da camada de aplicação na orquestração dessas interações.

## Camada de Aplicação
- **Definição**: A camada de aplicação é responsável por orquestrar as necessidades dos usuários, utilizando os agregados e outros componentes do sistema.
- **Objetivo**: Satisfazer as necessidades dos usuários que vão além das regras de negócio dos agregados.

### Funções da Camada de Aplicação
- **Intermediar Interações**: A camada de aplicação não permite que os usuários interajam diretamente com os agregados ou repositórios.
- **Expor Interface**: Ela expõe métodos que os usuários podem chamar para realizar operações específicas.
- **Orquestração de Regras**: A camada une diferentes regras de negócio para formar uma operação que atenda aos interesses dos usuários.

## Regras de Negócio vs. Necessidades do Usuário
- **Regras de Negócio**:
  - São independentes e não necessariamente satisfazem totalmente os interesses dos usuários.
  - Focam na lógica de domínio e não na persistência de dados.
  
- **Necessidades do Usuário**:
  - Incluem a necessidade de salvar informações e acessar dados posteriormente, o que não é tratado diretamente nas regras de negócio.

## Application Services
- **Definição**: Serviços de aplicação que expõem métodos para interação do usuário.
- **Exemplo**: Um `CustomerService` que permite:
  - Listar clientes por administradores.
  - Registrar novos clientes pelos próprios consumidores.

### Estrutura de um Application Service
1. **Injeção de Dependências**: É necessário injetar um repositório, como `iCustomerRepository`, para realizar operações.
2. **Métodos**: Os métodos dentro do serviço devem ser desenhados para serem reutilizáveis.

## Comparação com Clean Architecture
- **Semelhanças**: Ambas as abordagens têm uma camada de aplicação que lida com casos de uso.
- **Diferenças**: Embora conceitualmente semelhantes, existem abordagens distintas que não serão abordadas neste módulo.

## Conclusão
- A camada de aplicação é crucial para atender às necessidades dos usuários, servindo como uma interface entre eles e as regras de negócio do sistema.
- Faremos uma integração com o Nest e gerenciaremos eventos posteriormente.

### Próximos Passos
- Continuar explorando a construção de application services que atendam às necessidades dos usuários de forma eficiente.
- Discutir o ciclo de vida da aplicação e como esses serviços interagem com o restante do sistema.

--- 

**Nota**: Este resumo serve como guia de estudo para compreender a importância e a função da camada de aplicação dentro do paradigma do Domain Driven Design.



---

## modulo_8_11128.mp4

# Estudo sobre Camada de Aplicação no Domain Driven Design

## Introdução
- Continuação do estudo sobre *Domain Driven Design (DDD)*.
- Foco na *camada de aplicação* e suas interações com regras de negócio.

## Camada de Aplicação
### Conceito
- A camada de aplicação orquestra as necessidades do usuário.
- É responsável por integrar vários componentes como agregados e objetos de valor.
- O usuário não interage diretamente com os agregados ou repositórios, mas sim com a camada de aplicação.

### Regras de Negócio
- Regras de negócio são independentes e podem não atender totalmente às necessidades do usuário.
- A camada de aplicação combina essas regras e expõe métodos que o usuário pode utilizar.

## Estrutura da Camada de Aplicação
### Application Services
- Serviços de aplicação expõem métodos que os usuários interagem diretamente.
- Exemplo: um *Customer Service* pode permitir que administradores listem consumidores e clientes registrem-se.

### Implementação
- Utiliza repositórios para realizar operações.
- O repositório é responsável pela persistência de dados.
- Exemplo de injeção de dependência:
  - `iCustomerRepository` é injetado no serviço para orquestrar regras.

## Comparação com Outras Abordagens
- Embora existam outras arquiteturas como a *Clean Architecture*, o conceito de camada de aplicação se mantém.
- Neste módulo, o foco será apenas em Application Services, sem entrar na Clean Architecture.

## Estrutura em Camadas
### Interação do Usuário
- O usuário não interage diretamente com:
  - Entidades
  - Agregados
  - Repositórios
- A aplicação define esses limites e expõe uma interface acessível ao usuário.

### Gerenciamento das Necessidades do Usuário
- A camada de aplicação deve:
  - Gerenciar operações de forma eficiente.
  - Satisfazer as necessidades do usuário.
  - Integrar com outras partes do sistema, como eventos e frameworks (ex: Nest).

## Conclusão
- A camada de aplicação é fundamental para unir as regras de negócio e as necessidades do usuário.
- O próximo passo será explorar mais sobre a integração e gerenciamento de eventos.

### Próximos Passos
- Continuar a exploração da camada de aplicação e sua interação com o sistema.
- Analisar o ciclo de vida da aplicação e a integração com outras tecnologias.

--- 

**Observações Finais:**
- É importante entender que a camada de aplicação serve como um intermediário que facilita a interação do usuário com a lógica de negócio do software.
- Estar ciente das diferenças entre as abordagens ajudará na aplicação prática dos conceitos em projetos futuros.



---

## modulo_8_11129.mp4

## Resumo da Aula sobre Domain Driven Design

### Introdução
- A aula foca na criação da primeira entidade dentro do conceito de Domain Driven Design (DDD).
- A estrutura de pastas é organizada, com todas as entidades localizadas na pasta `Domain`, especificamente em `Entities`.

### Estrutura de Pastas
- **Pasta Domain**: Local onde se concentra a lógica de domínio.
- **Pasta Entities**: Abriga entidades e agregados.

### Criação da Entidade `Customer`
- **Arquivo**: `Customer.Entity.ts`
  - Sufixo `.Entity` é uma convenção de nomenclatura utilizada para fácil identificação em projetos.

### Campos da Entidade
1. **ID**: Utilizado como chave primária no banco de dados, deve ser um `uuid`.
2. **CPF**: Uma string, não um número, para preservar o zero à esquerda.
3. **Nome**: Nome do cliente.

### Identidade da Entidade
- **Identidade Natural**: CPF do cliente, utilizado para identificá-lo em interações.
- **Identidade Substituta**: ID gerado (uuid ou inteiro) que facilita a indexação e performance no banco de dados.

### Construtor da Entidade
- Preferência por usar um objeto como parâmetro no construtor para melhor clareza.
- **Type**: `CustomerConstructorProps` que inclui ID, CPF e Nome para facilitar a criação de instâncias.

### Operações com a Entidade
- **Criação**: Representada pela instância da classe `Customer`.
- **Salvar**: Relaciona-se à persistência no banco de dados.
- **Diferenciação**: O construtor inicia a instância, enquanto a operação de criação é feita em um método separado para refletir a lógica de DDD.

### Métodos Adicionais
- **Método toJSON()**: Para conversão da entidade em string, útil para debugging e serialização.
- **Comparação de Entidades**: Método para comparar entidades com base em IDs.

### Considerações Finais
- A criação da entidade é um passo importante na implementação de DDD.
- O entendimento das operações e da estrutura é crucial para o desenvolvimento eficaz de sistemas baseados em DDD.

### Próximos Passos
- Continuar a explorar conceitos de DDD e a implementação de métodos adicionais nas entidades.
- Discutir abstrações e comparações entre entidades na próxima aula.

### Dicas de Estudo
- Revise os conceitos de *identidade natural* e *identidade substituta*.
- Pratique a criação de entidades e métodos utilizando a estrutura e convenções discutidas.
- Explore a documentação de TypeScript para entender melhor tipos e construtores.



---

## modulo_8_11130.mp4

# Estudo sobre Domain Driven Design (DDD) - Criando a Primeira Entidade

## Introdução
- O objetivo da aula é criar a primeira entidade no contexto de Domain Driven Design (DDD).
- A estrutura do projeto seguirá a convenção de organizar tudo dentro da pasta **Domain**.

## Estrutura do Projeto
- Criar uma pasta chamada **Entities** para abrigar entidades e agregados.
- Nomeação do arquivo da entidade:
  - Exemplo: **Customer.Entity.ts**
  - O sufixo **.Entity** é uma convenção pessoal, mas pode variar entre diferentes linguagens e comunidades.

## Definindo a Entidade Customer
### Campos da Entidade
- Os principais campos definidos para a entidade **Customer**:
  - **id**: Tipo UUID (identificador único universal).
  - **cpf**: String (não pode ser numérico, pois pode começar com zero).
  - **nome**: String.

### Identidade da Entidade
- **Identidade Natural**: O CPF pode ser considerado uma identidade natural do **Customer**.
- **Identidade Substituta**: O ID (UUID) é mais adequado como chave primária em bancos de dados por questões de eficiência e indexação.

## Implementação da Entidade
### Construtor da Entidade
- **Preferência**: Utilizar um objeto para o construtor ao invés de passar múltiplos parâmetros.
- Criação de um tipo TypeScript:
  - Exemplo: `type CustomerConstructorProps = { id?: string; cpf: string; nome: string; }`
  
### Criação do Método de Instanciação
- O método de criação da entidade deve ser distinto do construtor.
- Operação de criação: `return new Customer(command)`
- O ID pode ser gerado automaticamente, tornando-o um campo opcional no construtor.

## Métodos Adicionais
### Método toJSON
- Importância de ter um método que converta a entidade para um formato string (útil para debug).
- Exemplo de implementação:
  - `toJSON()`: Retorna um objeto simplificado com ID, CPF e nome.

### Comparação de Entidades
- É importante implementar métodos de comparação para verificar se duas entidades são equivalentes, geralmente através do ID.

## Conclusão
- A aula finaliza com a criação da entidade **Customer** e a distinção entre a operação de criação e a persistência.
- O próximo passo será aprofundar em como essas operações interagem com o banco de dados.

## Pontos Importantes para Estudo
- Entender a diferença entre **identidade natural** e **identidade substituta**.
- Praticar a implementação de entidades e suas operações em TypeScript.
- Familiarizar-se com conceitos de DDD, como **agregados** e **comandos**.
- Explorar a estrutura de projetos e convenções de nomenclatura em diferentes linguagens de programação.



---

## modulo_8_11131.mp4

# Resumo da Aula sobre Domain Driven Design: Criando a Entidade Customer

## Introdução
- A aula continua a temática de *Domain Driven Design* (DDD).
- O foco principal é a criação da primeira entidade, que será a `Customer`.

## Estrutura do Domínio
- **Pasta Domain**: Todos os elementos do domínio serão organizados nesta pasta.
- **Subpasta Entities**: Criada para abrigar as entidades e agregados.
  
## Criação da Entidade Customer
- **Arquivo**: `Customer.Entity.ts`
  - Sufixo “Entity” utilizado por convenção, especialmente para quem trabalha com frameworks como Angular e NestJS.

## Campos da Entidade Customer
- **Identificação dos Campos**:
  - `id`: Será um UUID.
  - `cpf`: Uma string (não pode ser um número, pois pode começar com zero).
  - `nome`: Nome do cliente.

## Identidade da Entidade
- O *cpf* pode ser utilizado como a identidade da entidade, pois identifica o cliente.
- *Identidade Natural*: CPF.
- *Identidade Substituta*: ID (UUID ou inteiro) utilizado como chave primária no banco de dados.
  - É mais eficiente para operações de indexação e recuperação de dados.

## Construtor da Entidade
- Preferência por passar um objeto no construtor em vez de múltiplos parâmetros.
- **Type**: `CustomerConstructorProps` para definir os campos que o construtor receberá.
  
### Exemplo de Construtor
```typescript
class Customer {
  id?: string;
  cpf: string;
  name: string;

  constructor(props: CustomerConstructorProps) {
    this.id = props.id;
    this.cpf = props.cpf;
    this.name = props.name;
  }
}
```

## Operações da Entidade
- **Operação de Criar**:
  - Representa a criação de uma instância da entidade.
- **Persistência**:
  - A operação de salvar é diferente da operação de criar.
  - O repositório será responsável por persistir a entidade no banco de dados.

### Método de Criação
- Recomenda-se ter um método específico para a operação de criação:
```typescript
function createCustomer(command: CustomerConstructorProps): Customer {
  return new Customer(command);
}
```

## Método de Conversão
- Implementar um método para converter a entidade em string (útil para debug).
  - Exemplo: `toJSON()` para simplificar a visualização dos dados.

### Exemplo de Método toJSON
```typescript
toJSON() {
  return {
    id: this.id,
    cpf: this.cpf,
    name: this.name,
  };
}
```

## Considerações Finais
- Discussão sobre métodos mágicos em outras linguagens que podem ser utilizados para comparação de entidades.
- A próxima aula abordará mais sobre abstrações e comparações entre entidades.

## Conclusão
- A aula proporcionou uma compreensão prática sobre a criação de entidades dentro do conceito de DDD.
- Importância de entender a diferença entre operação de criar e persistir.

**Próximos Passos:**
- Continuar explorando o DDD e suas práticas em aulas futuras.



---

## modulo_8_11132.mp4

# Resumo da Aula sobre Domain Driven Design (DDD)

## Introdução
- A aula foca na criação da primeira entidade dentro do contexto de Domain Driven Design (DDD).
- A organização do projeto é fundamental, com tudo relacionado ao domínio dentro da pasta **Domain**.

## Estrutura do Projeto
- **Pasta Entities**: 
  - Criada para abrigar entidades e agregados.
  - Referência a agregados como entidades é comum, por isso a escolha do nome.

## Criação da Entidade Customer
- Arquivo criado: **Customer.Entity.ts**.
- Nomeação de arquivos seguindo uma convenção pessoal, influenciada por frameworks como Angular e Nest.

### Campos da Entidade
- Campos definidos:
  - `id`: Utilização de **UUID**.
  - `cpf`: Tipo **string**, não pode ser numérico (pode começar com zero).
  - `name`: Nome do cliente.
  
### Identidade da Entidade
- **Identidade Natural**: O `cpf` como identificação única do cliente.
- **Identidade Substituta**: O `id` (UUID) como chave primária no banco de dados.
  - Vantagens do uso de ID:
    - Melhor performance.
    - Eficiência na indexação e recuperação de dados.

## Construtor da Entidade
- Preferência por passar um objeto no construtor ao invés de múltiplos parâmetros:
  - Facilita a criação e entendimento do código.
- Criação de um tipo chamado **CustomerConstructorProps** para definir os campos do construtor.

### Operações de Criação
- A operação de **criar** é representada pela instância de `Customer`.
- Distinção entre **criação** e **salvamento**:
  - **Criar**: Ação de instanciar a entidade.
  - **Salvar**: Persistência da entidade no banco de dados.

### Métodos Adicionais
- Adição de um método para converter a entidade em string:
  - Útil para **debug** e **serialização**.
  - Sugestão de implementação do método **toJSON** para retornar um objeto simples.

## Conclusão
- A criação da entidade está completa com a operação de criação definida.
- A discussão sobre comparação entre entidades e métodos padrões será abordada na próxima aula.

## Próximos Passos
- Continuação do aprendizado sobre DDD e implementação de mais funcionalidades e entidades. 

## Notas Finais
- Importância de manter uma boa organização e nomenclatura no código.
- Compreensão clara das identidades e operações é essencial para um design eficaz.



---

## modulo_8_11133.mp4

# Estudo sobre Domain Design e Identificadores Únicos (UID)

## Introdução
Nesta aula, discutimos a importância do identificador único (UID) em Domain Design, abordando sua implementação e utilização em entidades no contexto de um sistema.

## Principais Conceitos

### O que é o UID?
- **UID** (Identificador Único) é uma string que serve para identificar entidades de forma única.
- Pode ser utilizado em URLs, garantindo segurança, já que o ID real do usuário não é exposto.

### Geração do UID
- O UID pode ser gerado automaticamente ao iniciar um cliente (customer).
- A lógica de geração do UID não deve estar diretamente na entidade, mas sim em um **Objeto de Valor**.

### Objeto de Valor
- Um objeto de valor é uma estrutura que encapsula um valor, neste caso, o UID.
- Utilizamos a biblioteca nativa `crypto` do **Node.js** para gerar o UUID.
- Validação do UUID é feita através de uma biblioteca específica, evitando a necessidade de expressões regulares.

## Implementação do Customer ID

### Estrutura do Customer ID
- O `Customer ID` será uma classe que estende de um objeto de valor (UUID).
- O construtor pode receber um `Customer ID` existente ou uma string para gerar um novo ID.

### Lógica do Construtor
- Utilização de lógica ternária para verificar o tipo de entrada.
  - Se for uma string, cria-se um novo `Customer ID`.
  - Se for uma instância do `Customer ID`, utiliza-se esse valor.
  - Caso contrário, gera-se um novo ID.

### Testes
- A implementação deve ser testada para garantir que o `Customer ID` é gerado e validado corretamente.
- Exemplos de verificações em testes:
  - Se o ID está definido.
  - Se o nome e CPF estão corretos.

## Comportamento e Segurança
- Utilizar objetos de valor aumenta a segurança, pois o TypeScript ajuda a evitar erros de tipos.
- A implementação do método `equals` permite comparar instâncias de entidades de forma segura.

### Exemplo de Implementação do Método Equals
- O método `equals` deve verificar:
  - Se o objeto passado é válido.
  - Se os IDs das entidades são iguais.

## Conclusão
- A utilização de **UIDs** e **Objetos de Valor** em Domain Design proporciona uma estrutura mais robusta e segura para o gerenciamento de entidades.
- A implementação segue os princípios do **Domain-Driven Design (DDD)**, promovendo consistência e segurança ao longo do sistema. 

## Próximos Passos
- Continuar a exploração de **DDD** e sua aplicação em contextos mais complexos, como eventos e interações entre entidades.

## Dicas para Estudo
1. **Revise** os conceitos de UID e Objetos de Valor.
2. **Pratique** a implementação do Customer ID em um projeto de exemplo.
3. **Teste** a lógica do construtor e do método equals em diferentes cenários.
4. **Estude** a utilização de bibliotecas de validação de UUID para aprimorar seu conhecimento prático.



---

## modulo_8_11134.mp4

# Estudo sobre Domain Design e UID

## Introdução
Neste estudo, abordamos a importância do UID (Identificador Único) no Domain Design, suas aplicações e como implementá-lo de forma eficaz em entidades.

## O que é o UID?
- **UID** é um identificador único que serve para:
  - Garantir a segurança ao trabalhar com URLs.
  - Normalizar a identificação de usuários e entidades.

## Geração do UID
- O UID pode ser gerado no momento da criação de um cliente (customer).
- Utiliza-se a biblioteca nativa do Node.js para geração de UUID.
- Validação do UUID é feita através da mesma biblioteca.

### Implementação da Geração
- Um objeto de valor foi criado para lidar com o UUID, evitando a necessidade de passar um valor manualmente.
- Se o valor não for passado, um novo UUID é gerado automaticamente.

### Exemplo de Validação
- Se o UUID passado não for válido, um erro é lançado:
  - `if (!validateUUID(value)) throw new Error("Invalid UUID");`

## Uso do Objeto de Valor
- **Customer ID** é criado como uma classe que estende o objeto de valor (value object).
- Isso garante que o ID do agregado seja sempre um objeto de valor, proporcionando:
  - Melhor segurança de tipo.
  - Validação automática.

## Lógica do Construtor
- O construtor pode receber:
  - Um `customer ID` já existente.
  - Uma string, que será convertida em um `customer ID`.
- Usando lógica ternária:
  - `const id = typeof props.id === 'string' ? new CustomerID(props.id) : props.id;`

## Testes de Validação
- Os testes devem verificar:
  - Se o ID está definido.
  - Se o nome e o CPF estão corretos.
- Utilização do `instanceof` para garantir que o ID é uma instância do `CustomerID`.

## Comportamento do Objeto de Valor
- O método **equals** é implementado para comparar IDs de entidades.
- Garante que duas entidades com o mesmo ID sejam consideradas iguais.

### Implementação do Método Equals
- O método deve verificar:
  - Se o parâmetro é nulo ou indefinido.
  - Se os IDs das entidades são iguais.

## Vantagens do Uso do Objeto de Valor
- **Segurança**: Reduz o risco de passar valores inválidos.
- **Consistência**: Garante que todos os IDs seguem o mesmo comportamento.
- **Facilidade de Uso**: Simplifica a lógica de criação e validação de entidades.

## Conclusão
- O uso de objetos de valor, como o `CustomerID`, é fundamental para manter a integridade e a segurança no Domain Design.
- A implementação correta do UID e das comparações entre entidades é crucial para o sucesso de um sistema bem estruturado.

## Próximos Passos
- Continuar explorando o Domain Driven Design (DDD).
- Implementar eventos e outras funcionalidades seguindo as boas práticas discutidas.



---

## modulo_8_11135.mp4

# Estudo sobre ID e Utilização de UUID no Domain Design

## Introdução
Nesta aula, discutimos a importância do UID (Identificador Único) no design de domínio, especialmente em relação à criação e validação de entidades e objetos de valor. O uso de UUIDs é enfatizado para garantir a integridade e segurança dos IDs.

## Principais Pontos

### O que é UID?
- **UID** é um identificador único utilizado para normalizar dados.
- Pode ser utilizado em URLs de forma segura, ocultando o ID real do usuário.

### Geração e Validação do UID
- O UID pode ser gerado durante a inicialização de um cliente.
- Uma biblioteca nativa do Node.js (biblioteca *crypto*) é usada para gerar UUIDs.
- O uso da biblioteca UUID para validação é recomendado para garantir que o ID gerado seja válido.

### Implementação do Objeto de Valor
- Um objeto de valor `CustomerID` é criado, que estende de um objeto de valor genérico.
- O objeto de valor permite:
  - Gerar um UUID automaticamente se nenhum valor for passado.
  - Validar um UUID se um valor for fornecido.
  
### Lógica do Construtor
- O construtor do cliente pode aceitar tanto um `CustomerID` quanto uma string.
- Utilização de operadores do TypeScript para facilitar a verificação e a geração de IDs.

### Testes e Validações
- Importância de realizar testes para garantir que IDs estejam definidos e sejam válidos.
- Utilização de `instanceof` para verificar se um ID é uma instância de `CustomerID`.

### Vantagens do Uso de Objetos de Valor
- Melhoria na tipagem e segurança do código.
- Redução do risco de erros em produção devido a tipos inadequados.
- Implementação de métodos como `equals` para comparação de entidades.

### Implementação do Método Equals
- O método `equals` é implementado para verificar se duas entidades são idênticas.
- A comparação envolve:
  - Verificação de nulidade e indefinição.
  - Comparação dos IDs das entidades.

## Conclusão
Utilizar *UUIDs* e objetos de valor no design de domínio traz vantagens significativas em termos de segurança, validação e organização do código. O uso de métodos como `equals` para garantir a integridade das entidades é fundamental no desenvolvimento de sistemas complexos.

## Dicas de Estudo
- **Pratique a implementação de objetos de valor e métodos de comparação** em projetos de estudo.
- **Experimente diferentes cenários** de validação e geração de IDs para entender melhor como funcionam.
- **Revisite os conceitos de DDD** (Domain-Driven Design) e como eles se aplicam na prática através de exemplos.



---

## modulo_8_11136.mp4

# Resumo da Aula sobre Domain Design e Identificadores Únicos (UID)

## Introdução
Nesta aula, discutimos a implementação e a utilidade do Identificador Único (UID) no contexto de Domain Design. O UID é fundamental para a normalização e segurança das URL, além de ser utilizado em outras entidades e agregados.

## Objetivos do UID
- **Normalização**: O UID permite que trabalhemos com identificadores de forma segura e estruturada.
- **Geração Automática**: O UID pode ser gerado automaticamente no momento da criação de uma entidade, evitando a necessidade de passar valores manualmente.

## Implementação do UID
1. **Criação do Objeto de Valor**:
   - Um objeto de valor para o UUID foi criado, estendendo de `value object`.
   - O UID é gerado utilizando a biblioteca nativa `crypto` do Node.js.

2. **Validação do UUID**:
   - Utiliza-se o método `validate` da biblioteca UUID para garantir que o UID gerado é válido.
   - Se um UID inválido é passado, um erro é lançado.

3. **Uso do Customer ID**:
   - O ID do agregado (como o Customer ID) é tratado como um objeto de valor, melhorando a lógica do construtor.
   - Permite que o construtor receba tanto um `CustomerID` quanto uma string, gerando um novo `CustomerID` quando necessário.

## Lógica do Construtor
- **Lógica Ternária**: 
  - Se a variável `id` for uma string, um novo `CustomerID` é gerado.
  - Se um `CustomerID` já for passado, ele é utilizado diretamente.
  - Caso contrário, um novo UID é gerado.

## Testes e Validações
- Os testes incluem a criação de um cliente e validações de:
  - Se o ID está definido.
  - Se o `name` e o `CPF` estão corretos.
- Utilização do `console.log` para verificar a estrutura do objeto criado.

## Comportamento do Objeto de Valor
- O uso do objeto de valor normaliza o comportamento das entidades, garantindo que todos os IDs sejam válidos e consistentes.
- Aumenta a segurança do código, pois permite o uso de `instanceof` para verificar a validade do ID.

## Método Equals
- Implementação do método `equals` na entidade para comparar se duas entidades são iguais com base em seus IDs.
- Verificações incluem:
  - Se o ID é null ou undefined.
  - Comparação dos IDs para garantir que são equivalentes.

## Conclusões
- O uso de objetos de valor e a implementação de UID trazem vantagens significativas para a segurança e estrutura do código.
- A abordagem discutida é alinhada com as práticas recomendadas de Domain Driven Design (DDD).
- O padrão estabelecido facilita a manutenção e a evolução do sistema.

## Próximos Passos
- Continuar a exploração dos conceitos de DDD e como aplicá-los em projetos reais.
- Implementar mais práticas de teste e validação para garantir a robustez do sistema. 

---

Esses pontos fornecem uma visão estruturada da aula, facilitando a revisão e o entendimento dos conceitos abordados no Domain Design e na implementação de UIDs.



---

## modulo_8_11137.mp4

# Resumo da Aula sobre Domain Drone Design

## Introdução
- O foco da aula é trabalhar com o **agregado de eventos**.
- O instrutor discute a importância de se desvincular dos **ORMs** para manter a essência da programação.

## Manipulação de Sessões em Eventos
### Construtor de Eventos
- O construtor permite passar uma sequência de **sessões** ou iniciar um conjunto vazio.
- É necessário implementar uma operação de negócio para adicionar sessões a um evento.

### Método `AddSection`
- **Definição**: O método `AddSection` será responsável por adicionar uma sessão ao evento.
- **Regra de Negócio**: Adicionar sessões é uma operação de negócio que deve ser claramente identificada.
- **Comando**: O uso de comandos facilita a compreensão da operação.

### Parâmetros Necessários
- Nome da sessão
- Descrição (opcional)
- Total de spots
- Preço

## Implementação do Método `addSection`
1. Criar uma nova sessão através do comando `addSectionCommand`, que contém os dados necessários.
2. Armazenar a sessão criada em uma variável para posterior manipulação.
3. Atualizar o total de spots do evento.

### Regra de Negócio
- Ao adicionar uma sessão, o total de spots deve ser atualizado:
  - `thisTotalSpots += totalDeSpotsAdicionados`

### Testes
- Verificar se:
  - O tamanho da sessão é igual a 1.
  - O total de spots é igual a 100 (inicialmente começando em 0).

## Geração de Spots
- Ao criar uma sessão, deve-se gerar automaticamente os spots correspondentes.
- Utilização de um loop `for` para criar spots baseados no total de spots informados.

### Organização do Código
- Criação de um método privado `initSpots` para organizar a lógica de criação dos spots.
- Retornar a sessão criada na função para garantir que o objeto esteja acessível.

## Regras de Negócio e SOLID
- Regras de negócio devem ser combinadas e modularizadas para facilitar o teste e a manutenção.
- Importância de seguir os princípios **SOLID**:
  - Cada método deve ter uma única responsabilidade.
  - Evitar fazer muitas operações em um único método, o que dificulta testes e manutenção.

## Conclusão
- A aula enfatiza a importância de criar operações menores e mais concisas para facilitar o desenvolvimento e a manutenção do código.
- Sugestão de continuar a saga de desenvolvimento no próximo encontro, abordando novos campos e modificações.

## Dicas de Estudo
- **Reveja os conceitos de SOLID** e como se aplicam em design de software.
- **Pratique a criação de métodos** pequenos e focados, seguindo regras de negócio claras.
- **Realize testes unitários** para garantir que cada parte do código funcione conforme esperado.



---

## modulo_8_11138.mp4

# Notas de Estudo: Domain Drone Design

## Introdução
- O foco da aula é trabalhar com operações em um agregado de eventos.
- Discussão sobre a importância de desvincular de ORMs para manter a essência da programação.

## Criação de Eventos
### Construtor de Eventos
- Possibilidade de passar uma sequência de sessões ou não passar nada, iniciando um conjunto padrão (set).
- A adição de sessões a um evento é uma operação de negócio que deve ser implementada.

### Método AddSection
- Criação do método `AddSection` como uma regra de negócio.
- É recomendado incluir um comando para facilitar a compreensão da operação.
- O comando `AddSection` pode conter:
  - Nome da sessão
  - Descrição (opcional)
  - Total de spots
  - Preço

## Implementação do Método AddSection
- A criação de uma sessão usa o comando `addSectionCommand`.
- Os dados necessários para a criação incluem:
  - Nome
  - Descrição
  - Total de spots
  - Preço

### Verificação e Testes
- Testar se o número total de spots é igual ao esperado após a adição de uma nova seção.
- Importância de manter a expressividade no código.

## Geração de Spots
### Regras de Negócio
- Cada vez que uma sessão é criada, os spots correspondentes devem ser gerados.
- Implementação de um loop para criar os spots de acordo com o total definido.

### Estrutura e Organização
- Sugestão de criar métodos privados para manter a lógica mais legível.
- A criação da sessão deve retornar o objeto correspondente para a fábrica.

## Testes e Validações
- Verificação do total de spots gerados após a criação da sessão.
- Uso de testes para garantir que a lógica de criação e modificação de spots esteja funcionando corretamente.

## Princípios SOLID
- Cada método deve ter uma responsabilidade única e clara.
- A separação de operações menores facilita testes e manutenção.
- Importância de combinar regras de negócio para atender às necessidades do usuário.

## Considerações Finais
- A necessidade de se "vacinar" contra a complexidade, dividindo operações em ações menores e mais concisas.
- A próxima aula abordará outros campos e modificações, ampliando o entendimento do sistema.

## Conclusão
- A aula se concentra na construção de regras de negócio para manipulação de eventos e sessões.
- A prática de manter o código organizado e testável é enfatizada.



---

## modulo_8_11139.mp4

# Resumo da Aula: Domain Drone Design

## Introdução
- O foco da aula é realizar operações em um *agregado de eventos*.
- O professor enfatiza a importância de se afastar de ORMs (Object-Relational Mappers) para manter a essência da programação.

## Estrutura do Evento
- O construtor de eventos pode receber uma sequência de sessões ou, se não for passado nada, inicia-se um *set*.
- A adição de sessões em um evento é uma operação de negócio que deve ser implementada como um método na classe.

### Adicionando Sessões
- O método **AddSection** é introduzido como parte das regras de negócio.
- É recomendado o uso de um comando (command) para facilitar a compreensão das operações realizadas.
- Os parâmetros para adicionar uma sessão incluem:
  - Nome da sessão
  - Descrição (opcional)
  - Total de spots
  - Preço

## Implementação do Método AddSection
- O método é implementado utilizando o comando `addSectionCommand`.
- A criação da seção utiliza os dados do comando e é armazenada em uma variável.
- O total de spots é atualizado conforme a nova seção é adicionada.
- A lógica é clara e expressiva, facilitando a manutenção do código.

### Geração de Spots
- Após a criação da sessão, é necessário gerar os spots correspondentes.
- Utiliza-se um loop `for` para criar os spots até o número total especificado.
- É sugerido que a lógica de criação de spots seja movida para um método privado para manter a organização do código.

## Testes
- Realizam-se testes para verificar se o total de spots está correto.
- O total de spots deve ser igual a 100, com base na criação de uma nova sessão.

## Regras de Negócio
- É importante manter as regras de negócio separadas e concisas.
- Os métodos devem ter uma única responsabilidade, seguindo os princípios do SOLID.
- O professor ressalta a importância de criar operações menores para facilitar testes e manutenção.

## Conclusão
- A aula termina com uma chamada para continuar a jornada de desenvolvimento, enfatizando a importância de organizar o código e manter a lógica clara.
- Sugestão de explorar operações adicionais e modificações em outros campos, como o Partner, em aulas futuras.

## Pontos Chave para Revisão
- **Agregado de Eventos**: Estrutura que permite organizar sessões e spots.
- **AddSection**: Método para adicionar sessões ao evento.
- **Command**: Estrutura que representa uma operação de negócio.
- **Regras de Negócio**: Lógica que define como as operações devem ser realizadas dentro do modelo.
- **SOLID**: Conjunto de princípios para manter a qualidade do código.

### Dicas de Estudo
1. **Revisar o Código**: Estudar a implementação do método AddSection e como ele interage com o agregado.
2. **Praticar Testes**: Criar testes para diferentes cenários de adição de sessões e geração de spots.
3. **Refletir sobre SOLID**: Analisar como os princípios SOLID podem ser aplicados em seu próprio código.
4. **Explorar Outras Linguagens**: Considerar a implementação dos conceitos apresentados em outras linguagens de programação, como Python.



---

## modulo_8_11140.mp4

# Resumo da Aula: Domain Drone Design

## Introdução
- O foco da aula é trabalhar com um agregado de eventos.
- O objetivo é sair do uso de ORMs e retornar à essência da programação.

## Estrutura do Evento
- O construtor de eventos aceita uma sequência de sessões ou inicia um conjunto vazio.
- A adição de sessões aos eventos é uma operação de negócio que será implementada como um método na classe.

### Operação de Negócio: AddSection
- **Método**: `AddSection`
- **Objetivo**: Adicionar uma sessão ao evento.
- **Componentes do Comando**:
  - Nome da sessão (obrigatório)
  - Descrição da sessão (não obrigatório, pode ser `null`)
  - Total de spots (obrigatório)
  - Preço (obrigatório)

## Criação da Sessão
- Utilização do comando `addSectionCommand` para criar uma nova seção.
- Os dados passados para a criação da seção são:
  - `nome`
  - `descrição`
  - `totalSpots`
  - `price`

### Implementação do Método
1. Criar a seção utilizando `section.create` com os dados do comando.
2. Adicionar a seção ao conjunto de seções do evento.
3. Atualizar o total de spots do evento.

### Expressividade do Código
- O código é escrito de forma que a lógica de negócios fique clara e expressiva.
- A modificação do total de spots é feita apenas através de operações, mantendo a integridade do estado.

## Geração dos Spots
- Após a criação de uma sessão, é necessário gerar os spots correspondentes.
- Implementação de um método para inicializar os spots:
  - Utilização de um loop `for` para adicionar spots até o total especificado.
- Regras de negócio devem ser encapsuladas em métodos privados para manter a legibilidade.

## Testes
- Verificar se o total de spots corresponde ao esperado após a adição da sessão.
- Exemplos de verificações:
  - O tamanho do array de seções deve ser igual a 1 após a adição.
  - O total de spots deve ser igual a 100 se inicialmente definido como tal.

## Regras de Negócio
- É importante pensar em operações menores e mais concisas.
- As regras de negócio podem ser combinadas em uma camada exterior para atender às necessidades do usuário.
- O uso do princípio SOLID:
  - Cada método deve ter uma única responsabilidade.

## Conclusão
- A implementação de regras de negócio menores facilita testes e manutenção.
- A próxima aula abordará modificações adicionais no sistema e conceitos relacionados.

## Próximos Passos
- Continuar a saga do Domain Drone Design e implementar mais funcionalidades.
- Estar preparado para discutir outras operações e como elas podem ser integradas no sistema.

--- 

**Notas Finais**:
- O objetivo desta aula foi enfatizar a importância de uma boa estrutura de código e a lógica de negócios ao desenvolver sistemas.
- Incentivo ao feedback para expor interesse em implementações em outras linguagens de programação.



---

## modulo_8_11141.mp4

# Notas de Estudo: Domain Driven Design - Modelo Rico e Entidades

## Introdução
Nesta aula, continuamos a discussão sobre *Domain Driven Design (DDD)*, focando na identificação de entidades dentro do modelo rico. Anteriormente, foi abordada a diferença entre o modelo rico e o modelo anêmico.

## Modelo Rico vs. Modelo Anêmico
- **Modelo Anêmico**: 
  - Focado na persistência de dados.
  - Não integra regras de negócio.
  
- **Modelo Rico**:
  - Integra regras de negócio nas entidades.
  - As entidades são objetos que queremos manipular e que possuem uma *identidade* única.

## Identificação de Entidades no DDD
### Perguntas para Identificação
1. **Devo diferenciar este evento de outros?**
   - Resposta: Sim.
2. **Como diferenciar este evento de outro?**
   - Através de uma *identidade*.

### Conceito de Identidade
- A identidade é um grupo de informações que diferencia uma entidade de outra.
- Exemplo de Identidade:
  - Código sequencial (ex: evento 001).
  - Data (ex: 1º de janeiro de 2023).

### Comparação de Entidades
- Para determinar se dois eventos são iguais, apenas a identidade é comparada.
- Exemplo: Chave primária em bancos de dados.

## Exemplos de Identidade
### Identidade de uma Pessoa
- O que torna uma pessoa única?
  - Nome: pode ser repetido.
  - RG: pode ser emitido por diferentes estados.
  - **CPF**: único e imutável, ideal para identificação.

### Importância do CPF
- O CPF é um exemplo de identidade que não muda ao longo do tempo.
- Em sistemas jurídicos, a identificação correta é crucial para evitar erros (ex: processos judiciais).

## Chaves Primárias e Identidade
### Questão Técnica
- O CPF pode ser uma chave primária?
  - Sim, mas pode haver outras considerações de performance.
  
### ID Substituto
- É possível usar um ID numérico (inteiro) para performance, enquanto mantém o CPF como a identidade única da pessoa.
- O ID é útil para consultas, mas não deve ser a linguagem principal ao se comunicar sobre entidades.

## Importância da Linguagem Ubíqua
- Ao discutir entidades, sempre se referir à identidade (ex: CPF) e não ao ID.
- Utilizar a mesma linguagem entre todos os envolvidos no projeto evita mal-entendidos.

## Resumo
- **Identidade** é um conceito central para a definição de entidades no DDD.
- As entidades têm características que podem mudar, mas sua identidade não se altera.
- A próxima aula abordará como tornar o modelo rico expressivo com as regras de negócio.

## Conclusão
O entendimento sobre entidades e suas identidades é fundamental para a aplicação correta do DDD. A comunicação clara e consistente sobre essas identidades é vital para o sucesso do desenvolvimento de software dentro desse paradigma.



---

## modulo_8_11236.mp4

# Estudo sobre Domain Driven Design: Camada de Aplicação

## Introdução
- O foco desta parte do Domain Driven Design (DDD) é a *camada de aplicação*.
- Baseado nos conceitos do livro de *Vernon* e *Evans*.

## Necessidades do Usuário
- Os usuários têm necessidades que vão além das regras de negócio dos agregados.
- Exemplo: Ao cadastrar um evento, o usuário quer que essas informações sejam salvas de alguma forma, mesmo sem conhecer a estrutura do banco de dados.

## Camada de Aplicação
- A camada de aplicação atua como orquestradora das necessidades dos usuários.
- É responsável por:
  - Integrar os *agregados*, *objetos de valor*, e outras camadas do projeto.
  - Expor uma interface que o usuário pode interagir.

### Funções da Camada de Aplicação
- *Orquestração*: Une as regras de negócio e as operações que os usuários precisam.
- *Interface de Usuário*: Não se trata de front-end, mas de métodos que os usuários usam para realizar ações.

## Regras de Negócio
- As regras de negócio são independentes e não necessariamente atendem todas as necessidades dos usuários.
- A camada de aplicação é responsável por:
  - Delimitar a interação dos usuários com as regras de negócio.
  - Expor *Application Services*.

### Application Services
- Serviços que expõem métodos que os usuários podem utilizar.
- Exemplo: Um *Customer Service* pode permitir que administradores listem consumidores e clientes registrem-se.

## Implementação
- O serviço de aplicação utilizará um repositório (ex: `iCustomerRepository`) para realizar operações.
- A camada de aplicação contém um conjunto de métodos que podem ser reutilizados conforme a necessidade.

## Comparação com Clean Architecture
- Embora não se queira aprofundar em Clean Architecture neste módulo, há similaridades conceituais:
  - Ambas as abordagens possuem uma camada de aplicação.
  - Clean Architecture trabalha com conceitos de casos de uso.

## Estrutura em Camadas
- O usuário **não interage diretamente** com entidades, agregados ou repositórios.
- A arquitetura em camadas separa responsabilidades, com a camada de aplicação delimitando a interação do usuário.

## Próximos Passos
- O foco agora é gerenciar as operações necessárias para satisfazer as necessidades do usuário.
- Integração com frameworks como Nest e gerenciamento de eventos.

## Conclusão
- A camada de aplicação é fundamental para que os usuários possam interagir eficientemente com o sistema, respeitando as regras de negócio e a estrutura definida.

### Referências
- Livros de *Vernon* e *Evans* sobre Domain Driven Design.
- Conceitos sobre Clean Architecture. 

## Dicas para Estudo
1. **Revisar conceitos de DDD**: Entender as diferenças entre agregados, repositórios e a camada de aplicação.
2. **Praticar Implementação**: Criar exemplos práticos de Application Services.
3. **Estudar a Arquitetura em Camadas**: Compreender como as camadas interagem e se complementam.



---

## modulo_8_11237.mp4

## Resumo da Aula sobre Domain Driven Design

### Introdução
Nesta aula, discutimos a relação entre *Application Services* e *agregados* no contexto do Domain Driven Design (DDD). O objetivo é esclarecer como estruturar métodos dentro dos serviços de aplicação, especialmente em relação a operações de atualização e criação de entidades.

### Tópicos Abordados

#### 1. Estrutura dos Métodos em Application Services
- Importância de definir o tamanho e a responsabilidade dos métodos.
- Um exemplo prático usando a entidade *Customer*:
  - Método `update` que recebe um ID e campos opcionais (e.g., nome).
  - Verificação se o *Customer* existe antes da atualização.
  - Tratamento de erros se o *Customer* não for encontrado.

#### 2. Lógica de Atualização
- Processo de atualização:
  - Consultar o repositório para verificar a existência do agregado.
  - Realizar modificações apenas se os dados forem fornecidos.
  - Realizar o `add` e o `commit` após as mudanças.

#### 3. Implementação para o Partner
- Similar ao *Customer*, o *Partner* pode ter métodos de atualização:
  - Método opcional para mudar o nome.
  - Possibilidade de retornar um erro se nenhuma informação for fornecida.

#### 4. Exemplo de Serviço de Evento
- Criação do *EventService*:
  - Importância de manter a consistência e a integridade do agregado *Event*.
  - Recebimento de dados como *Partner ID*, data, nome e descrição do evento.
  - Verificações de existência do *Partner* antes da criação do evento.

#### 5. Consultas e Retornos
- Possibilidade de consulta de seções de um evento:
  - Método `findSections` para retornar sessões de um evento específico.
  - Importância de sempre trabalhar com o agregado principal ao buscar dados.
  
#### 6. Mapeamento de Dados
- Discussão sobre a exposição de entidades nas camadas externas:
  - Preferência em não expor diretamente as entidades para evitar vazamentos de domínio.
  - Importância de mapear dados de retorno em um formato apropriado para consumo.

#### 7. Considerações Finais
- A camada de apresentação deve ser responsável por formatar dados, não o *Application Service*.
- O agregado protege a consistência e as invariâncias do projeto.
- Discussões sobre a estrutura de dados e a necessidade de criar novas camadas.

### Conclusão
A aula enfatiza a importância de uma estrutura clara e coesa nos *Application Services* e a responsabilidade dos agregados em manter a integridade dos dados. A próxima aula abordará mais operações para expandir o entendimento sobre a manipulação de eventos.

### Dicas para Estudo
- **Revisar os conceitos de DDD** e como eles se aplicam a *Application Services*.
- **Praticar a implementação** dos métodos discutidos em exemplos concretos.
- **Refletir sobre as melhores práticas** para evitar o vazamento de domínio e como mapear dados corretamente.



---

## modulo_8_11238.mp4

# Resumo da Aula sobre Domain Driven Design

## Introdução
- O tema da aula é o **Domain Driven Design** (DDD) e a relação entre **Application Services** e **agregados**.
- A discussão se concentra no tamanho dos métodos e na forma de interagir com os agregados.

## Estrutura de Métodos em Application Services

### Tamanho dos Métodos
- É importante considerar:
  - Se deve haver um método separado para cada método dos agregados.
  - A coesão e concisão dos métodos.

### Exemplo Prático com Customer
- Implementação de um método `update` para o agregado **Customer**:
  - Recebe **ID** e **name** (opcional).
  - Permite a atualização de outros campos conforme necessário.

#### Lógica do Método Update
1. **Consulta ao Repositório**: Verificar se o agregado existe.
2. **Tratamento de Erros**: Se o Customer não existir, lançar um erro.
3. **Atualização**: Modificar campos conforme os dados recebidos.
4. **Persistência**: Realizar o `add` e o `commit`.

### Organização e Regras
- As regras devem ser orquestradas para atender às necessidades do usuário.
- Exemplos de verificações adicionais:
  - Se o **name** não é passado, não precisa chamar a **unit of work**.

## Exemplo com Partner
- Implementação semelhante para o agregado **Partner**:
  - Recebe **id** e **name** (não obrigatório).
  - Se o **name** não é fornecido, pode retornar um erro ou o próprio partner.

## Serviço de Eventos

### Implementação do EventService
- Modificações para trabalhar com eventos:
  - Receber **partner ID** como string.
  - Verificar se o partner existe antes de criar um evento.

#### Criação de Eventos
- Recebe dados como:
  - **inputDate** (data de criação)
  - **inputName** (nome do evento)
  - **inputDescription** (descrição, opcional)

### Consultas e Retornos
- Exemplo de método para consultar sessões de eventos:
  - Método `findSections` que recebe **eventId**.
  - Retorna as sessões associadas ao evento.

### Práticas de Retorno
- Discussão sobre a exposição de entidades:
  - **Evans** e **Vernon** preferem evitar a exposição direta de entidades para camadas externas.
  - É importante avaliar a necessidade de criar uma camada de apresentação para evitar vazamento do domínio.

## Considerações Finais
- O agregado protege a consistência e as invariâncias do projeto.
- Importância de sempre manipular o agregado completo durante as operações.
- A próxima aula abordará outras operações e práticas dentro do contexto de eventos.

## Dicas para Estudo
- Reforce os conceitos de **Application Services** e **agregados**.
- Pratique a implementação de métodos de atualização e consulta.
- Estude as abordagens diferentes sobre a exposição de entidades e a criação de camadas de apresentação.
- Considere a importância do tratamento de erros e a consistência dos dados em seu projeto.



---

## modulo_8_11239.mp4

# Resumo da Aula sobre Domain Driven Design

## Introdução
Nesta aula, discutimos a relação entre *Application Services* e *agregados* no contexto de Domain Driven Design (DDD). O foco principal foi entender como estruturar métodos nos serviços de aplicação e a melhor maneira de interagir com agregados.

## Tamanho dos Métodos
- **Dúvida Comum**: Qual deve ser o tamanho dos métodos em Application Services? Devo criar um método para cada método do agregado?
- **Exemplo Prático**: Utilizamos o agregado *Customer* para ilustrar.

### Método de Atualização
- **Método `update`**: 
  - Recebe o **ID** do cliente e campos opcionais (como o **name**).
  - Verifica se o cliente existe consultando o repositório.
  - Se não existir, deve-se lançar um erro apropriado.
  - O tratamento de erro pode ser centralizado na camada de aplicação ou no framework utilizado.

- **Lógica do Método**:
  1. Consulta o repositório para verificar a existência do agregado.
  2. Se existir, atualiza os campos que foram passados.
  3. Realiza o **commit** após a operação.

## Regras de Negócio
- As operações dentro dos agregados devem ser:
  - **Concisas**: Focar em operações específicas relacionadas ao agregado.
  - **Coesas**: Manter a lógica de negócio encapsulada no agregado.

## Exemplo com Partner
- Processo semelhante ao do *Customer* foi aplicado ao *Partner*.
- Se o **name** não for passado, não é necessário chamar a unidade de trabalho, podendo retornar um erro ou o próprio partner.

## Serviço de Evento
- Introdução ao *EventService*:
  - Importância de verificar a existência do partner ao criar um evento.
  - Recebimento de dados para criar um evento (ex: partner ID, data, nome, descrição).
  
### Criação do Evento
1. **Receber Dados**: 
   - partner ID, data, nome, descrição (opcional).
2. **Verificação**:
   - Consultar o repositório de partners.
   - Lançar erro se o partner não existir.
3. **Persistência**:
   - Usar o repositório para salvar o evento.

## Consultas
- **Método `findSections`**: 
  - Permite consultar sessões de um evento específico.
  - Sempre trabalhar com o agregado para garantir a consistência.
  - Retornar as sessões do evento após realizar a consulta.

## Considerações Finais sobre Retorno
- **Exposição de Entidades**:
  - A comunidade tem opiniões divergentes sobre expor entidades diretamente nas camadas exteriores.
  - É recomendável criar um mapeamento para evitar o vazamento de domínio.

- **Avaliação de Dados**:
  - Avaliar se os dados retornados são significativamente diferentes do domínio pode justificar o uso de uma camada de apresentação.

## Conclusão
- A manipulação dos dados deve sempre respeitar as regras de consistência e invariância do modelo de domínio.
- O evento é o centro das operações, garantindo a proteção da lógica de negócio.

### Próximos Passos
- Na próxima aula, serão exploradas outras operações para ampliar a compreensão sobre a manipulação de eventos e agregados dentro do Domain Driven Design.



---

## modulo_8_11240.mp4

# Resumo da Aula sobre Domain Driven Design

## Introdução
Nesta aula, o foco é esclarecer as dúvidas sobre a criação de *Application Services* e a relação deles com os *agregados* no contexto do Domain Driven Design (DDD). Serão discutidos exemplos práticos, especialmente sobre o agregado *Customer* e sua implementação.

## Estrutura dos Métodos nos Application Services

### Questões Iniciais
- Qual é o tamanho dos métodos nos *Application Services*?
- Devo criar um método para cada método do agregado?

### Exemplo Prático: Atualização do Customer
- **Método Update**:
  - Recebe o ID do *Customer* para atualização.
  - O nome é um campo opcional.
  - Outros campos do *Customer* podem ser incluídos, se necessário.

### Lógica de Atualização
1. **Consulta ao Repositório**: Verificar se o *Customer* existe.
   - Se não existir, lançar um erro.
2. **Tratamento de Erros**:
   - Pode ser centralizado na camada de aplicação ou no framework utilizado.
   - Ex: Converter erro em status code HTTP.

3. **Operação Final**:
   - Realizar o `add` e depois o `commit` para efetivar a atualização.

## Coesão e Reutilização
- Métodos concisos e coesos nos agregados são mais reutilizáveis.
- Evitar a mentalidade de banco de dados ao desenvolver métodos.

## Exemplo Prático: Partner
- **Método de Atualização**:
  - Recebe ID e nome como parâmetros.
  - Se o nome não for fornecido, não precisa chamar a unit of work.

## Implementação do EventService
- **Mudanças Necessárias**:
  - Trocar instâncias de *Customer* por *Event*.
  - Ajustar a interface e os métodos para refletir essa mudança.

### Criando um Evento
1. **Dados Necessários**:
   - Partner ID (recebido como string).
   - Validar existência do Partner através do repositório.
   - Se não existir, lançar um erro.

2. **Dados do Evento**:
   - Data de criação, nome e descrição (todos podem ser facultativos).

3. **Commit**:
   - Finalizar a criação do evento.

### Consultando Sessões do Evento
- **Método findSections**:
  - Recebe o ID do evento.
  - Retorna as sessões do evento através do agregado, garantindo a consistência.

## Considerações sobre Retorno de Dados
- **Exposição de Entidades**:
  - Evans e Vernon recomendam não expor entidades diretamente para camadas externas.
  - Avaliar a necessidade de um mapeamento para evitar vazamento de domínio.

- **Formatação de Dados**:
  - A camada de apresentação deve se encarregar da formatação.
  - O *Application Service* deve retornar informações brutas, enquanto a apresentação lida com a formatação.

## Conclusão
- A manipulação dos eventos deve sempre preservar a integridade do agregado.
- A próxima aula abordará mais operações e conceitos para expandir a compreensão sobre *Application Services* e *agregados*.

---

## Dicas de Estudo
- **Revisar os conceitos de DDD**: Entender a importância da coesão e da reutilização.
- **Praticar a implementação**: Tente criar seus próprios *Application Services* com outros agregados.
- **Discutir em grupo**: Conversar sobre as melhores práticas de tratamento de erros e formatação de dados.



---

## modulo_8_11241.mp4

# Resumo da Aula: Criação de Order no Domínio Dream Design

## Introdução
Nesta aula, o foco é testar a criação de uma order dentro do domínio Dream Design. Várias regras de negócios estão em funcionamento, e o teste foi estruturado para verificar rapidamente se tudo está funcionando conforme esperado.

## Estrutura Inicial
- **Instâncias Criadas**:
  - MicroRM
  - Entity Manager
  - Unit of Work
- **Objetos Necessários**:
  - Customer
  - Partner
  - Event

## Criação de Customer, Partner e Event
- **Repositórios Utilizados**:
  1. Customer Repo
  2. Partner Repo
  3. Event Repo
- **Processo de Criação**:
  - Criar instância de *Customer* com dados simples.
  - Criar instância de *Partner*.
  - Inicializar o *Event* e adicionar a sessão necessária.

### Adicionando Sessão ao Evento
- **Parâmetros da Sessão**:
  - Descrição
  - Preço (R$100)
  - Total de spots (1.000)

## Teste do Order Service
- **Criação do Order Service**:
  - Instanciar *New Order Service*.
  - Importar repositórios necessários:
    - Order Repo
    - Customer Repo
    - Event Repo
    - Spot Reservation Repo
    - Unit of Work

### Execução do Método create
- **Parâmetros Necessários**:
  - ID do evento
  - ID da sessão (posição 0)
  - Validação do ID do Customer e do Spot

### Resolução de Erros
- **Erros Identificados**:
  - Spot não disponível durante a reserva.
  - Uso incorreto de ID em vez de Spot ID no repositório de Spot Reservation.
- **Correções**:
  - Ajustar o método de busca para usar Spot ID.
  - Adicionar `await` onde necessário para garantir que as operações assíncronas sejam concluídas.

## Finalização do Teste
- **Resultados**:
  - Após correções, o teste foi executado com sucesso sem erros.
  - Possibilidade de testar reservas já feitas.

## Marcação de Spots como Reservados
- **Nova Regra de Negócio**:
  - Após a criação da order, marcar o spot como reservado.
- **Implementação**:
  - Buscar a sessão correspondente e verificar se o spot já está reservado.
  - Implementar lógica para marcar o spot como reservado no evento.

## Conclusão
- O teste demonstrou que o *Order Service* está funcionando corretamente.
- Foram abordadas regras de negócio mais complexas e o uso de repositórios e agregados.
- Sugestão para continuar a implementação de testes automatizados e aprimorar a lógica do sistema.

## Próximos Passos
- Remover console logs desnecessários.
- Continuar a saga de desenvolvimento e testes no domínio Dream Design.

---

Esses pontos fornecem uma visão clara e estruturada da aula, ajudando no entendimento e na revisão dos conceitos discutidos.



---

## modulo_8_11242.mp4

# Resumo da Aula sobre Criação de Pedidos no Domínio Dream Design

## Introdução
- O tema da aula é a criação de pedidos.
- Foco em regras de negócio e testes de funcionalidade.

## Estrutura Inicial
- Criação de instâncias fundamentais:
  - **MicroRM**
  - **Entity Manager**
  - **Unit of Work**
- Necessidade de criar três entidades:
  1. **Customer**
  2. **Partner**
  3. **Event**

## Criação de Entidades
- **Customer**:
  - Criado com dados simples.
  
- **Partner**:
  - Criado de maneira similar ao Customer.

- **Event**:
  - Inicia-se o evento e adiciona-se uma sessão.
  - **Dados da Sessão**:
    - Descrição
    - Preço (R$ 100,00)
    - Total de spots (1.000)

## Execução de Testes
- Testar a criação de um pedido utilizando o **Order Service**.
- Instâncias necessárias:
  - **OrderRepo**
  - **CustomerRepo**
  - **EventRepo**
  - **Spot Reservation Repo**
  - **Unit of Work**

## Implementação do Order Service
- Chamada do método `OrderService.create`.
- Passagem de IDs:
  - ID do evento
  - ID da sessão (usando posição 0)
  - Cuidado com valores e objetos.

## Problemas Encontrados
- **Erros de Validação**:
  - Quando um `Spot` não está disponível.
  - Verificação de IDs incorretos (deve ser `Spot ID` ao invés de `ID`).

## Resolução de Erros
- Necessidade de:
  - **await** em algumas chamadas para garantir que o código seja executado na ordem correta.
  - Ajustar o repositório para buscar pelo `Spot ID`.

## Regras de Negócio
- Implementação de regras adicionais:
  - Marcar o spot como reservado após criar uma nova ordem.
  - Validação para garantir que um spot não possa ser reservado se já estiver reservado.

## Código e Estruturas
- Implementação de métodos para:
  - Marcar spots como reservados.
  - Atualizar estados de eventos e reservas.
  
## Conclusão
- Testes simples realizados para verificar a funcionalidade do **OrderService**.
- A necessidade de testes automatizados para garantir a integridade do sistema.
- Importância de seguir regras de negócio durante a implementação.

## Próximos Passos
- Continuar a implementação e testes no domínio **Dream Design**.
- Considerar mais regras de negócio e melhorias no código.

---
**Dicas para Estudo**:
- Revisar conceitos de **Unit of Work** e **Entity Manager**.
- Praticar a criação de repositórios e serviços.
- Experimentar com testes automatizados para familiarizar-se com o processo.



---

## modulo_8_11243.mp4

# Resumo da Aula: Criação de Order no Domínio Dream Design

## Introdução
Nesta aula, foi abordado o processo de criação de um pedido (order) dentro do domínio *Dream Design*, com foco nas regras de negócio e na implementação prática do código. 

## Estrutura do Teste
- **Componentes Criados:**
  - Instância do *microRM*
  - *Entity Manager*
  - Instância do *Unit of Work*
  
- **Entidades Necessárias:**
  - *Customer* (Cliente)
  - *Partner* (Parceiro)
  - *Event* (Evento)

## Criação de Entidades
1. **Criação do Customer:**
   - Dados simples utilizados para a criação.
  
2. **Criação do Partner:**
   - Seguiu um processo semelhante ao do Customer.
  
3. **Início do Event:**
   - Adição de uma sessão ao evento.
   - Definição de valores:
     - Preço: 100 reais
     - Total de spots: 1.000

## Execução dos Testes
- **Chamada do Commit:**
  - Utilização do *Entity Manager Flush* e do *Commit*.
  
- **Verificação de Publicação:**
  - O evento estava com a propriedade *Spublished* definida como *False*.

## Implementação do Order Service
1. **Criação do Order Service:**
   - Instância do *Order Service* criada para gerenciar pedidos.
  
2. **Repositórios Necessários:**
   - *Order Repo*
   - *Customer Repo*
   - *Event Repo*
   - *Spot Reservation Repo*
   - *Unit of Work*

3. **Chamada do Método create:**
   - Passagem de IDs do evento, sessão e outros dados necessários.

## Erros e Resoluções
- **Erro de Spot Não Disponível:**
  - Identificação de que o Spot não estava disponível durante o teste.
  
- **Correção no Repositório de Spot Reservation:**
  - A busca pelo ID foi corrigida para *Spot ID*.
  
- **Ajustes no Await:**
  - Inclusão de *await* faltantes que causavam falhas na execução.

## Finalização do Pedido
- **Marcação de Spot como Reservado:**
  - Implementação de uma regra para marcar o spot como reservado após a criação do pedido.
  
- **Mudanças no Evento:**
  - Atualização do evento para refletir a nova reserva.

## Conclusão
- O teste demonstrou que o *Order Service* está funcionando corretamente, embora seja um teste simples.
- Sugestão de realizar testes automatizados e explorar regras de negócio mais complexas.

## Próximos Passos
- Continuar explorando o domínio *Dream Design*.
- Implementar melhorias e ajustes com base nos testes realizados.

---

### Dicas para Estudo
- **Familiarize-se com os conceitos de:**
  - *Entity Manager*
  - *Unit of Work*
  - Repositórios e suas interações

- **Pratique a criação e manipulação de entidades:**
  - Experimente criar diferentes cenários de testes, alterando dados e verificando comportamentos.

- **Analise os erros comuns:**
  - Estude como resolver problemas relacionados a identificação de IDs e disponibilidade de recursos.

- **Explore testes automatizados:**
  - Considere a implementação de testes unitários para validar a lógica de negócio de forma sistemática.



---

## modulo_8_11244.mp4

# Estudo sobre Criação de Order no Domínio Dream Design

## Introdução
Este documento resume os principais pontos discutidos na lecture sobre a criação de uma ordem dentro do domínio *Dream Design*. O foco está na implementação de regras de negócio, testes e utilização de repositórios.

## Estrutura do Sistema

### Componentes Principais
- **MicroRM**: Instância do MicroRM.
- **Entity Manager**: Gerenciador de entidades.
- **Unit of Work**: Padrão de projeto utilizado para gerenciar transações e mudanças no estado das entidades.

### Entidades Criadas
1. **Customer**: Cliente da ordem.
2. **Partner**: Parceiro associado à ordem.
3. **Event**: Evento relacionado à ordem.

## Passos para Criação de uma Ordem

### 1. Criação de Entidades
- Criar instâncias de `Customer`, `Partner` e `Event`.
- Adicionar uma sessão ao evento.
  - **Descrição**: Informações sobre a sessão.
  - **Preço**: R$ 100.
  - **Total de Spots**: 1.000.

### 2. Persistência de Dados
- Utilizar `Entity Manager Flush` ou `Unit of Work Commit` para salvar as informações.

### 3. Teste do Order Service
- Criar uma instância do `Order Service`.
- Importar os repositórios necessários:
  - `Order Repo`
  - `Customer Repo`
  - `Event Repo`
  - `Spot Reservation Repo`
  - `Unit of Work`

### 4. Chamada para Criar Ordem
- Utilizar o método `OrderService.create`.
- Passar os IDs necessários:
  - ID do evento.
  - ID da sessão (posição 0).
  - ID do cliente e ID do spot, garantindo que estamos passando o valor correto.

## Erros e Soluções

### Problemas Encontrados
- **Erro de Spot Não Disponível**: Ocorreu ao tentar reservar um spot que já estava reservado.
- **Erro de ID Inexistente**: O método estava buscando pelo ID incorreto, ao invés de `Spot ID`.

### Correções Realizadas
1. Ajuste na lógica do `Spot Reservation` para utilizar `Spot ID`.
2. Adição de verificações para garantir que o spot não esteja reservado antes de marcar como reservado.
3. Inclusão de `await` nas operações assíncronas, especialmente antes de commits.

## Regras de Negócio
- Não é possível marcar um spot como reservado se ele já estiver reservado.
- Após a criação da ordem e reserva do spot, o evento deve ser atualizado para refletir essas mudanças.

## Conclusão
Este teste simples demonstrou a criação de uma ordem e a interação entre as diferentes entidades e repositórios no domínio Dream Design. Para um sistema mais robusto, recomenda-se a implementação de testes automatizados e a validação das regras de negócio.

## Próximos Passos
- Realizar testes adicionais para garantir a integridade do sistema.
- Implementar regras de negócio mais complexas conforme necessário.
- Remover logs de console e limpar o código para produção.

**Nota**: Este documento pode ser utilizado como guia para entender a implementação de serviços e repositórios no contexto de um domínio de aplicação.



---

## modulo_8_11245.mp4

# Notas de Estudo: Integração do Core com o Nest

## Introdução

Neste capítulo, abordaremos a integração do core com o framework Nest. É importante destacar que, durante o desenvolvimento prático, não precisamos de artefatos do Nest, exceto para referências como a configuração do TypeScript.

## Estrutura do Core e Integração

- **Core como Software Independente**: 
  - O framework depende do core, e não o contrário.
  - Possibilidade de integrar o core com outros projetos, como Express, Java, .NET, etc.

## Configuração do Banco de Dados

1. **Uso do npx-nest**:
   - Comando: `npx-nest` para gerar artefatos.
   - Criação do módulo de `database` para configurar o microRM.

2. **Configurações do MicroRM**:
   - Importação do módulo que se integra com o Nest.
   - Configurações necessárias:
     - Banco de dados
     - Host
     - Porta
     - Usuário
     - Senha
     - SQL
     - Forçamento de uso do construtor

3. **Importação do Módulo**:
   - Importação do microRM módulo com as configurações necessárias.
   - Configuração do **Unit of Work**:
     - Habilitação no módulo de banco de dados.
     - Uso de interfaces e tokens para provê-los.

## Implementação de Serviços

- **Providers do Nest**:
  - Configuração de todos os serviços dentro do projeto.
  - Importância de não usar a interface diretamente, pois ela é descartada na compilação do TypeScript.

- **Factory Method**:
  - Recebimento do Entity Manager (EM).
  - Criação de uma nova instância do microRM.

- **Habilitação do Unit of Work**:
  - Tornar o Unit of Work acessível a qualquer módulo do sistema.
  - Uso de um decorator global para facilitar o acesso.

## Criação do Módulo de Eventos

1. **Distinção entre Módulos**:
   - Não confundir o módulo de eventos do Nest com o módulo de eventos do Core.

2. **Configuração do Módulo de Eventos**:
   - Importação do microRM módulo for feature.
   - Importação de todas as entidades e esquemas necessários.

## Conclusão

- A configuração do banco de dados está em andamento e será complementada nas aulas seguintes.
- O foco é garantir que o sistema permaneça leve e compreensível para todos os envolvidos no desenvolvimento.

---

## Próximos Passos

- Continuar a construção e aprimoramento das configurações no módulo de banco de dados.
- Explorar mais sobre a criação de application services e outros módulos necessários no sistema. 

## Dicas de Estudo

- **Revisar a documentação do Nest** para entender melhor o funcionamento dos módulos e providers.
- **Praticar a criação de módulos** em pequenos projetos para ganhar familiaridade.
- **Experimentar a integração do core com diferentes frameworks** para solidificar o aprendizado sobre a flexibilidade do core.



---

## modulo_8_11246.mp4

# Resumo do Capítulo sobre Integração com o Nest.js

## Introdução
- O objetivo deste capítulo é realizar todas as integrações necessárias para que o core esteja integrado com o framework do Nest.js.
- O core é um software independente que pode ser utilizado com diferentes frameworks, como Express, Java, ou .NET.

## Estrutura do Core
- O core deve ser implementado de forma que o framework dependa dele, e não o contrário.
- Isso permite que o core seja facilmente reutilizado em outros projetos.

## Integração com o Banco de Dados
1. **Utilização do npx-nest**: 
   - Com o comando `npx-nest`, é possível gerar artefatos necessários para a configuração do banco de dados.
2. **Criação do Módulo de Database**:
   - O módulo deve ser chamado de `database` para configurar o microRM (Micro Relational Mapper).
   - As configurações incluem:
     - Database
     - Host
     - Porta
     - Usuário
     - Senha
     - SQL
     - Forçamento de uso do construtor

3. **Importação de Módulos**:
   - Importar o módulo do microRM ao integrar com o Nest.
   - A importação deve ser feita de forma a estar disponível para toda a aplicação.

## Configuração do Unit of Work
- O Unit of Work deve ser configurado no módulo de database.
- Na parte de providers do Nest, todos os serviços são configurados.
- **Boas Práticas**:
  - Usar tokens ao invés de passar interfaces diretamente (interfaces são descartadas na compilação do TypeScript).
  - Criar variáveis para reutilização de tokens em diferentes partes do código.

## Acesso Global ao Unit of Work
- O decorator global é utilizado para tornar o Unit of Work acessível a qualquer módulo do sistema.
- Isso evita a necessidade de múltiplas importações do módulo de database.

## Criação do Módulo de Eventos
- Um novo módulo de eventos deve ser criado, diferenciando-se do módulo de eventos do Nest.
- Importações necessárias:
  - Importar o `microRM módulo for feature`.
  - Copiar e importar todas as entidades e esquemas necessários para o módulo de eventos.

## Conclusão
- O banco de dados foi habilitado e algumas configurações estão concluídas.
- O desenvolvimento será contínuo nas próximas aulas, visando a leveza e a compreensão do que é necessário.

## Próximos Passos
- Continuar a construção do sistema com foco em manter a clareza e a funcionalidade.
- Preparar a implementação dos application services e outras funcionalidades conforme avançamos. 

**Dicas para Estudo:**
- Revisar as práticas de modularização no Nest.js.
- Estudar a implementação de Unit of Work e suas vantagens na arquitetura de software.
- Praticar a criação de módulos e importações no Nest.js para reforçar o aprendizado.



---

## modulo_8_11247.mp4

# Resumo da Aula: Integrações do Core com o NestJS

## Introdução
- O objetivo da aula é integrar o core desenvolvido com o framework NestJS.
- O core é um software independente que pode ser utilizado com diferentes frameworks, como Express, Java, .NET, etc.

## Estrutura do Core
- O core serviu como referência para a configuração do TypeScript, mas não utilizamos artefatos do NestJS até agora.
- A integração do core com o Nest é feita de forma que o framework depende do core e não o contrário.

## Integração com Banco de Dados
1. **Uso do npx-nest**:
   - Para iniciar a configuração do banco de dados, utilizamos o comando `npx-nest`.
   - O módulo criado para o banco de dados será chamado de `database`.

2. **Configuração do MicroRM**:
   - As configurações do microRM serão importadas e configuradas no novo módulo de banco de dados.
   - Importar o módulo que integra com o Nest é essencial para a configuração.

3. **Configurações Necessárias**:
   - Configurações a serem incluídas:
     - Database
     - Host
     - Porta
     - Usuário
     - Senha
     - SQL
     - Forçamento de uso do construtor
   - Importar todos os esquemas relacionados ao banco de dados.

4. **Unit of Work**:
   - A configuração do Unit of Work será feita no módulo de banco de dados.
   - Utilizar uma interface para prover o serviço, mantendo boas práticas.
   - O Entity Manager deve ser injetado corretamente.

5. **Habilitação Global do Unit of Work**:
   - O Unit of Work será habilitado como global, permitindo o acesso a qualquer módulo do sistema.
   - Isso elimina a necessidade de múltiplas importações.

## Criação do Módulo de Eventos
- Criação de um novo módulo chamado `events`.
- Importante não confundir o módulo de eventos do NestJS com o módulo de eventos do core.
- Importação do `microRM módulo for feature` para o módulo de eventos.
- Copiar todas as entidades e esquemas necessários para o novo módulo.

## Considerações Finais
- A aula abordou a configuração inicial do banco de dados e a criação do módulo de eventos.
- O desenvolvimento será feito de forma incremental, para facilitar o entendimento dos alunos.
- O próximo passo será continuar a trabalhar nas configurações e implementação dos serviços da aplicação.

## Dicas de Estudo
- **Revisar o conceito de microRM** e sua integração com o NestJS.
- **Praticar a criação de módulos** e a configuração de serviços no NestJS.
- **Explorar a documentação** do NestJS para entender melhor a modularidade e as práticas recomendadas.
- **Familiarizar-se** com o conceito de Unit of Work e como ele se aplica em aplicações com NestJS.



---

## modulo_8_11248.mp4

# Resumo da Aula: Camada de Aplicação no Domain Driven Design

## Introdução ao Domain Driven Design (DDD)
- A aula foca na camada de aplicação dentro do contexto do DDD.
- Referência aos livros de *Vernon* e *Evans*.

## Importância da Camada de Aplicação
- A camada de aplicação orquestra as necessidades do usuário.
- Os usuários têm necessidades que vão além das regras de negócio dos agregados.
- A operação realizada pelo usuário deve ser salva e acessível, o que não é uma preocupação da lógica de negócio.

## Diferença entre Regras de Negócio e Camada de Aplicação
- As regras de negócio são independentes e podem não satisfazer completamente os interesses dos usuários.
- A camada de aplicação:
  - Une os diversos componentes (agregados, objetos de valor).
  - Expondo métodos que os usuários podem interagir.

## Estrutura da Camada de Aplicação
- **Application Service**: Serviços que expõem os métodos para interação do usuário.
  - Exemplo: `CustomerService` para gerenciar consumidores.
- A camada de aplicação não interage diretamente com:
  - Agregados
  - Repositórios

## Componentes da Camada de Aplicação
1. **Repositórios**: Responsáveis pela persistência dos dados.
2. **Métodos de Serviço**: Métodos reutilizáveis que atendem às necessidades dos stakeholders.
   - Exemplo: Listar consumidores ou registrar novos clientes.
3. **Injeção de Dependências**: Uso do repositório dentro do serviço para operações.

## Comparação com Clean Architecture
- Embora haja uma similaridade conceitual entre a camada de aplicação no DDD e a Clean Architecture, a aula se concentrará apenas nos *Application Services*.

## Princípios da Arquitetura em Camadas
- O usuário não deve interagir diretamente com:
  - Entidades
  - Agregados
  - Repositórios
- A camada de aplicação delimita a interface para usuários (clientes da aplicação).

## Próximos Passos
- Gerenciar as operações para satisfazer as necessidades do usuário de forma eficiente.
- Estudar o ciclo de vida da aplicação, integração com *Nest* e gerenciamento de eventos.

## Conclusão
- A aula conclui com um convite para continuar a saga do DDD, enfatizando a importância da camada de aplicação.

### Observações Finais
- A camada de aplicação é fundamental para garantir que as operações do usuário sejam realizadas de forma estruturada e organizada, alinhando as regras de negócio com as necessidades reais dos usuários.



---

## modulo_8_11249.mp4

# Resumo da Aula sobre Integrações no Core com Nest

## Introdução
- O objetivo da aula é integrar o *core* com o framework *Nest*.
- O *core* é visto como um software independente que pode ser utilizado com diferentes frameworks.

## Estrutura do Core
- O *core* não depende do Nest, mas sim o contrário.
- A integração pode ser feita com outros frameworks, como *Express*, *Java* e *NET*.

## Integração com o Banco de Dados
1. **Uso do npx-nest**:
   - Comando para gerar artefatos: `npx-nest`.
   - Criação do módulo de database para configurar o *microRM*.

2. **Configurações do Módulo de Database**:
   - Importação do módulo que se integra com o Nest.
   - Configurações necessárias:
     - *database*
     - *host*
     - *porta*
     - *usuário*
     - *senha*
     - *SQL*
     - *forçamento de uso do construtor*

3. **Importação de Schemas**:
   - Importar todos os esquemas relacionados ao módulo de database.
   - Habilitação do *unit of work* no módulo de database.

## Configuração de Providers no Nest
- Todos os serviços são configurados na parte de providers.
- Importância de trabalhar com interfaces:
  - Não pode passar a interface diretamente, pois é descartada na compilação do TypeScript.
  - Sugestão de usar tokens para facilitar a importação em outros lugares.

## Injeção de Dependências
- Utilização do *Entity Manager*:
  - Injeção do *Entity Manager* para criar o *microRM Unit of Work*.
  - Uso de factory method para devolver um novo microRM.

## Habilitação do Unit of Work
- Tornar o *Unit of Work* global na aplicação usando um decorator global.
- Acesso facilitado a partir de qualquer módulo do sistema.

## Criação do Módulo de Eventos
- Criação de um novo módulo de eventos (não confundir com o módulo de eventos do Nest).
- Importação do *microRM* como *for feature* dentro do módulo de eventos.
- Importação de entidades e esquemas necessários para o módulo de eventos.

## Conclusão
- Estrutura do banco de dados está em progresso.
- A aula se propõe a ser gradual, permitindo melhor entendimento.
- Continuação prevista para as próximas aulas.

### Dicas de Estudo
- Revise a relação de dependência entre o *core* e o Nest.
- Pratique a configuração do módulo de database e a injeção de dependências.
- Familiarize-se com a terminologia usada, como *unit of work* e *Entity Manager*.
- Explore a criação e importação de módulos, especialmente o de eventos.

## Próximos Passos
- Continuar a construção do sistema aos poucos nas aulas seguintes.
- Verificar como aplicar os conceitos de forma prática em projetos reais.



---

## modulo_8_11250.mp4

# Resumo da Aula: Construindo Endpoints da API REST com Domain Driven Design (DDD)

## Introdução
- Continuação da série sobre *Domain Driven Design (DDD)*.
- Foco na construção dos endpoints restantes da API REST, especificamente para eventos e pedidos (orders).

## Estrutura da API REST
- A API REST deve ser desenhada de forma a não influenciar os *application services*.
- O design deve ser conveniente e adequado aos serviços da aplicação.

## Controllers

### Events Controller
1. **Registro no Módulo de Eventos**
   - Necessário registrar o *events controller* no módulo de eventos para utilizá-lo.
   
2. **Operações com Eventos**
   - Listar eventos.
   - Criar um novo evento.
   - Publicar todos os eventos.

3. **Métodos do Application Service**
   - Uso de métodos como `list` e `findEvents` para busca eficiente.

4. **Data Transfer Object (DTO)**
   - Utilização de um DTO para encapsular dados e realizar validações.
   - Uso das bibliotecas *class-validator* e *class-transformer* para validações e serialização.
   - Validação de dados na requisição (ex: formatação de datas).

5. **Validação Global**
   - Ativação do *validation pipe* no `main` para aplicar regras de validação.

6. **Publicação de Eventos**
   - Método `publishAll` para modificar registros.

### Sessões e Spots
1. **Design de API para Sessões**
   - Endpoint aninhado (nested) usando o ID do evento.
   - Consultar e criar sessões associadas a eventos.

2. **Operações com Sessões**
   - Consultar sessões utilizando o ID do evento.
   - Criar uma nova sessão com dados relevantes (nome, descrição, total, spots, preço).

3. **Atualizações**
   - Métodos para atualizar sessões existentes.
   - Design da API que favorece a clareza na relação entre eventos e sessões.

### Orders (Pedidos)
1. **Consulta de Pedidos**
   - Implementação de endpoints para consultar e criar pedidos.

2. **Criação de Reservas**
   - Necessidade de passar parâmetros como *customer ID*, *section ID*, *spot ID* e *event ID*.
   - Validação de disponibilidade de spots.

3. **Tratamento de Erros**
   - Sugestão de uso de *exception filters* do NestJS para tratamento de erros.

## Banco de Dados
- Avaliação do banco de dados usando comandos SQL.
- Importância de manter uma linguagem ubíqua nos nomes de tabelas e campos.

## Conclusão
- Integração completa da aplicação construída com NestJS e DDD.
- Importância de seguir as práticas de DDD para a estrutura do projeto e do banco de dados.

## Dicas Finais
- **Linguagem Ubiqua:** Manter a consistência na nomenclatura entre código e banco de dados.
- **Validações:** Separar validações simples da lógica de negócios que devem ser realizadas dentro dos agregados.
- **Organização do Código:** Não sobrecarregar um único controller; utilizar múltiplos controllers quando necessário.

**Próximos Passos:** Continuar explorando e aprimorando a implementação do DDD em projetos reais.



---

## modulo_8_11251.mp4

# Resumo da Aula sobre Domain Driven Design e API REST

## Introdução
- Continuação do estudo sobre **Domain Driven Design (DDD)**.
- Foco na implementação dos endpoints restantes da API REST, especificamente para eventos e pedidos (orders).

## Estrutura da API REST
- A API REST deve ser desenhada de forma a não influenciar os **application services**.
- É importante utilizar esses serviços de maneira adequada.

## Controller de Eventos
### Registro do Controller
- O controller de eventos deve ser registrado no módulo de eventos para ser utilizável.
- Operações principais:
  - Listar eventos (`GET`)
  - Criar um evento (`POST`)
  - Publicar todos os eventos.

### Implementação
- Utilização de um **DTO (Data Transfer Object)** para encapsular dados da requisição.
- Sugestão de usar bibliotecas como **class-validator** e **class-transformer** para validação e serialização de dados.

### Validações
- Validações primárias ocorrem na camada de **application services**, enquanto validações de negócio são realizadas dentro dos agregados e entidades.
- Habilitar o **validation pipe** no main para aplicar validações.

### Publicação de Eventos
- Método para publicar todos os eventos utilizando o ID do evento.
- Pode ser utilizado um método `PATCH` por questões semânticas.

## Controller de Sessões
### Estrutura de Endpoints
- Utilização de um endpoint aninhado para gerenciar sessões relacionadas a eventos.
- Operações principais:
  - Consultar sessões
  - Criar uma nova sessão
  - Atualizar uma sessão

### Implementação de Sessões
- Passagem do ID do evento como parte do recurso na rota.
- Utilização de métodos do **application service** para adicionar e atualizar sessões.

## Controller de Spots
- Endpoint deve receber o ID do evento e o ID da sessão.
- Métodos disponíveis incluem:
  - **findSpots** para consultar todos os spots.
  - Atualização de informações de spots através de um `PUT`.

## Controller de Orders
### Consulta e Criação de Pedidos
- Consultas de pedidos já foram realizadas em aulas anteriores.
- Para criar um pedido, é necessário o **customer ID**, **section ID**, **spot ID**, e **event ID** na URL.

### Tratamento de Erros
- Implementação de tratamento de erros utilizando **exception filters** do NestJS.
- Importância de manter a linguagem ubíqua em nomes de tabelas e campos do banco de dados.

## Conclusão
- Integração completa da aplicação usando **NestJS** e **DDD**.
- A aplicação está funcionando conforme o esperado, com todos os endpoints implementados e testados.

## Dicas para Estudo
1. **Revisar conceitos de DDD**: Certifique-se de entender os princípios do Domain Driven Design e como eles se aplicam na construção de APIs.
2. **Praticar com DTOs**: Explore a criação e utilização de DTOs em suas aplicações.
3. **Validar dados**: Aprenda a utilizar bibliotecas de validação e transformação no NestJS.
4. **Trabalhar com endpoints**: Pratique a construção de endpoints aninhados e como eles interagem com os **application services**.
5. **Realizar testes**: Teste os endpoints criados para garantir que estão funcionando corretamente e que os erros são tratados adequadamente. 

Estudar esses pontos ajudará a consolidar o conhecimento sobre a implementação de APIs REST utilizando DDD.



---

## modulo_8_11252.mp4

# Resumo da Aula sobre Domain Driven Design e API REST

## Introdução
- Continuação da implementação de endpoints da API REST utilizando **Domain Driven Design (DDD)**.
- Foco no desenvolvimento dos controllers para eventos e pedidos (orders).

## Estrutura da API REST
- A **API REST** não deve influenciar os **application services**.
- O design deve ser orientado à conveniência e uso adequado dos **application services**.

## Controller de Eventos
### Funcionalidades
- Listar eventos.
- Criar um evento.
- Publicar todos os eventos.

### Implementação
- Necessário registrar o controller no módulo de eventos.
- Utilização do **application service** para operações.

### Métodos
1. **Listar Eventos**: 
   - Método renomeado para `findEvents` para maior clareza.
   - Implementação de rota GET.
2. **Criar Evento**:
   - Uso de um **DTO** (Data Transfer Object) para encapsular dados.
   - Validação de dados utilizando as bibliotecas **class-validator** e **class-transformer**.
   - Conversão de datas no formato adequado para JavaScript.
   - Rota POST para criação.

### Validação
- Ativação do **Validation Pipe** no arquivo principal (`main`).
- Validações de negócios realizadas dentro dos agregados e entidades.

## Publicação de Eventos
- Implementação do método `publishAll` que recebe o ID do evento.
- Uso de um input para modificar registros.

## Controller de Sessões e Spots
### Estrutura
- API desenhada com endpoints aninhados, como `/event/:id/section`.
- Métodos para:
  - Consultar sessões.
  - Criar nova sessão.
  - Atualizar sessão.

### Implementação
- Recebimento de parâmetros de rota (`eventId`, `sectionId`).
- Chamada ao método `addSession` para adicionar novas sessões.
- Possibilidade de atualizar informações de sessões.

## Controller de Spots
### Funcionalidades
- Consultar todos os spots.
- Atualizar localização de spots.
- Implementação de métodos específicos para operações relacionadas a spots.

## Controller de Orders
### Funcionalidades
- Consultar e criar pedidos (orders).
- Necessidade de passar um **card token** para criação de pedidos.
- Validação do **customer ID**, **section ID**, **spot ID** e **event ID**.

## Integração com Banco de Dados
- Uso do **Docker** para acessar o banco de dados.
- Verificação das tabelas e dados inseridos (ex: `orders`, `spot_reservation`).
- Importância de manter uma linguagem ubíqua nos nomes de tabelas e campos.

## Conclusão
- Aplicação construída com **NestJS** e seguindo os princípios de **DDD**.
- Prática de manter a linguagem consistente entre o código, projeto e banco de dados para facilitar a compreensão e manutenção.

### Observações Finais
- Importância de tratamento de erros na API.
- Sugestão de uso de **exception filters** no NestJS para melhor gerenciamento de erros.

---

### Dicas para Estudo
- Revisar os conceitos de **DTO**, **Validation Pipe**, e **application services**.
- Praticar a implementação de endpoints REST com foco em DDD.
- Analisar exemplos de validações e transformações de dados no NestJS.
- Explorar o uso de Docker para gerenciar bancos de dados em projetos de desenvolvimento.



---

## modulo_8_11253.mp4

# Resumo da Aula: Implementação de Endpoints em uma API REST com Domain Driven Design

## Introdução
Nesta aula, o foco foi na implementação dos endpoints restantes da API REST utilizando o conceito de *Domain Driven Design (DDD)*. A discussão abrangeu a estruturação dos controllers, a utilização de *application services* e a validação de dados.

## Estrutura dos Controllers
- **Eventos e Orders**: O objetivo é criar controladores para gerenciar eventos e pedidos.
- **Desenho da API**: É fundamental que a API REST não influencie os *application services*. O desenho deve ser conveniente e funcional.

### Events Controller
- **Registro**: O controlador de eventos deve ser registrado no módulo de eventos.
- **Métodos Principais**:
  - `list`: Listar todos os eventos.
  - `create`: Criar um novo evento.
  - `publishAll`: Publicar todos os eventos.

#### Uso de DTOs
- Implementação de *Data Transfer Objects (DTOs)* para encapsular os dados recebidos e enviados.
- Validação e transformação de dados usando as bibliotecas:
  - **class-validator**
  - **class-transformer**

### Validações
- As validações primárias ocorrem na camada de requisições, enquanto as validações de negócio são gerenciadas dentro dos agregados e entidades.
- Habilitar o *validation pipe* no `main` da aplicação.

### Publicação de Eventos
- Método `publishAll`: Utiliza o ID do evento para modificar registros e publicá-los. Pode ser implementado como um `PATCH`.

## Sessões e Spots
- **Design de API**: A API pode ser desenhada para que as sessões sejam dependentes do evento, usando rotas aninhadas.
- Métodos para sessões:
  - `addSession`: Adicionar uma nova sessão.
  - `updateSession`: Atualizar informações de uma sessão.
  - `findSessions`: Consultar todas as sessões de um evento específico.

### Estrutura de Dados
- Ao criar sessões, os dados como nome, descrição e preço devem ser considerados.
- As respostas da API podem incluir dados agregados, mas a necessidade de retornar todos os dados deve ser avaliada.

## Orders
- **Consulta de Pedidos**: Implementação de endpoints para consultar e criar pedidos.
- **Criação de Reserva**: Para criar uma reserva, os IDs do cliente, seção, spot e evento são necessários.
- Tratamento de erros: Considerar o uso de *exception filters* do NestJS para gerenciar erros de forma eficaz.

### Linguagem Ubíqua
- Importância de manter a linguagem ubíqua nas entidades e nomes de campos, tanto no código quanto no banco de dados.
- Facilita a comunicação entre as equipes de desenvolvimento e as de banco de dados.

## Conclusão
Através da implementação dos endpoints e da integração dos conceitos de DDD, foi possível construir uma aplicação robusta utilizando NestJS. A aula finalizou com a validação do funcionamento da aplicação e a importância de manter uma linguagem consistente ao longo do projeto.

## Pontos Chave para Estudo
1. **Compreensão do DDD**: Entender como o DDD se aplica ao design de APIs.
2. **Controller e Application Services**: Saber como os controllers interagem com os *application services*.
3. **Implementação de DTOs**: Práticas recomendadas para a criação e validação de DTOs.
4. **Validações e Transformações**: Como utilizar *class-validator* e *class-transformer*.
5. **Estrutura de API**: A importância de rotas aninhadas e de um desenho claro e funcional.

## Sugestões de Prática
- Implementar um novo endpoint seguindo as práticas discutidas.
- Criar testes para verificar a funcionalidade dos endpoints.
- Explorar mais sobre *exception filters* e como eles podem ser integrados na API.



---

## modulo_8_11254.mp4

# Notas de Estudo: Domain Driven Design - Integração com Processos de Negócio

## Introdução
- Continuação do estudo sobre *Domain Driven Design*.
- Criação do *Domain Event Manager* na aula anterior.
- Foco na integração com processos de negócio.

## Conceitos Fundamentais

### Gerenciamento de Eventos
- **Eventos de Domínio**: Criados quando uma entidade (ex: partner) é criada.
- **Listeners**: Recebem eventos e executam processos de negócio antes do commit.

### Ciclo de Vida do Application Service
- O *Application Service* tem um ciclo de vida que inclui:
  - **Início**: Quando o processo é iniciado.
  - **Finalização**: Quando o processo termina.
  - **Falhas**: Tratamento de erros que podem ocorrer.

## Implementação do Application Service

### Estrutura do Application Service
- Criação de uma classe chamada `ApplicationService`.
- Recebe duas dependências no construtor:
  - `Unit of Work`: Interface para gerenciamento de transações.
  - `DomainEventManager`: Gerenciamento de eventos de domínio.

### Métodos Importantes
1. **Start**: Inicia o ciclo de vida do processo.
2. **Finish**: Realiza o commit do `Unit of Work` e publica os eventos.
3. **Fail**: Lida com possíveis falhas durante o processo.

### Exemplo de Implementação
- Implementação do método `Finish`:
  - Recupera todos os *aggregate routes* da transação.
  - Publica eventos de domínio para cada *aggregate route*.
  - Utiliza `await` para garantir a execução sequencial.

### Tratamento de Erros
- Uso de `try/catch` para capturar erros durante a execução.
- Chamada ao método `fail` caso ocorra um erro.

## Melhoria da Legibilidade
- Sugestão de criar um método `run`:
  - Recebe um callback e retorna uma promessa com resultado.
  - Melhora a organização do código e a legibilidade.

## Conclusão
- Integração do *Application Service* foi realizada com sucesso.
- Testes práticos ficarão para a próxima aula.
- Continuação do aprendizado sobre *Domain Driven Design*.

## Pontos para Revisão
- Compreender as diferenças entre *Unit of Work* e *Domain Event Manager*.
- Praticar a implementação de *Application Services* e seus ciclos de vida.
- Refletir sobre o tratamento de eventos e erros em aplicações complexas.

## Próximos Passos
- Preparar-se para os testes práticos na próxima aula.
- Revisar conceitos de *Domain Driven Design* e sua aplicação em projetos reais.



---

## modulo_8_11255.mp4

# Resumo da Aula sobre Domain Driven Design

## Introdução
- Continuação da saga sobre **Domain Driven Design**.
- Criação do **Domain Event Manager** na aula anterior.
- Integração com os processos de negócio.

## Contexto da Aula
- Cenário: Criação de um parceiro (partner) e registro do evento de criação.
- Importância de um listener para receber eventos e processar o negócio antes do commit no banco de dados.
- O papel do **Unit of Work** em mesclar e executar operações no banco.

## Abordagem Proposta
- Delegar a gestão de eventos a um serviço específico, evitando registros diretos em cada **Application Service**.
- Criação de uma classe chamada **ApplicationService**.

### Ciclo de Vida do Application Service
1. **Início**: Quando o processo de negócio é iniciado.
2. **Finalização**: Quando o processo é concluído (finish).
3. **Falha**: Quando ocorre um erro (fail).

## Implementação do Application Service
- O **Application Service** deve ser importado na camada de aplicação.
- Receberá como parâmetros:
  - **Unit of Work**: referência da interface.
  - **DomainEventManager**: para gerenciar eventos.

### Estrutura do Application Service
- Métodos importantes:
  - `Start`: Início do ciclo de vida.
  - `Finish`: Finalização, onde ocorre o commit do **Unit of Work** e a publicação dos eventos.
  - `Fail`: Tratamento de erros.

## Publicação de Eventos
- No método **Finish**:
  - Recuperar todos os agregados envolvidos na transação através do **Unit of Work**.
  - Implementar um método para obter todas as **aggregate routes**.
  
### Manipulação de Agregados
- Usar o **Entity Manager** ou **Unit of Work** para:
  - Obter entidades gerenciadas (persist stack).
  - Obter entidades removidas (remove stack).
- Concatenar os resultados em um array.

## Lógica do Método Run
- Utilização de `await` para garantir que os eventos sejam publicados de forma sequencial.
- Possibilidade de um listener publicar eventos que outros listeners podem ouvir.
  
### Execução do Método
- Implementação da lógica de execução com um método **run** que recebe um callback e retorna uma promessa.
- Uso de `try/catch` para tratar erros durante a execução.

## Conclusão
- A aula abordou a integração do **Application Service** e a gestão de eventos.
- Próxima aula: realização de testes para integração do sistema.

## Próximos Passos
- Revisar a implementação do **Application Service**.
- Preparar para a aula de testes e validação do sistema.

---

### Observações Finais
- Importância de manter a legibilidade do código durante a implementação.
- O ciclo de vida do **Application Service** é crucial para o gerenciamento de eventos e processos de negócio.

### Dicas de Estudo
- **Revisar conceitos** de Domain Driven Design e suas práticas.
- **Praticar** a implementação do Application Service em pequenos projetos.
- **Participar de discussões** sobre padrões de design e arquitetura de software.

---

Com esses pontos, você terá uma visão clara da aula e poderá se preparar adequadamente para as próximas etapas no aprendizado sobre Domain Driven Design.



---

## modulo_8_11256.mp4

# Resumo da Aula sobre Domain Driven Design

## Introdução
- Continuação da saga sobre *Domain Driven Design*.
- Revisão do que foi feito na aula anterior: criação do *Domain Event Manager*.
- Objetivo da aula: integrar eventos com processos de negócio.

## Integração com Processos de Negócio
- Quando um *partner* é criado, um evento de criação é registrado.
- Um listener deve receber esse evento e processar o negócio antes do commit.
- Importância de não registrar eventos diretamente em cada *Application Service* para evitar duplicidade e complexidade.

## Ciclo de Vida do Application Service
- O *Application Service* terá um ciclo de vida que inclui:
  - Início do processo de negócio.
  - Finalização do processo (finish).
  - Tratamento de falhas (fail).
  
### Abstração do Application Service
- Criação de uma nova classe chamada `ApplicationService`.
- No construtor da classe, receber referências para:
  - *Unit of Work* (interface).
  - *Domain Event Manager*.

## Estrutura do Application Service
- O ciclo de vida deve ser estruturado da seguinte maneira:
  1. **Início**: Chamar `ApplicationService Start`.
  2. **Finalização**: Chamar `ApplicationService Finish`.
  3. **Falha**: Lidar com erros chamando `fail`.

### Funcionalidades do Application Service
- O *Application Service* pode realizar:
  - Logs.
  - Gerenciamento do ciclo de vida do processo.
- O commit do *Unit of Work* ocorre no método `finish`.

## Gerenciamento de Eventos
- É necessário obter todos os *aggregate roots* envolvidos na transação.
- Adição de um método na interface do *Unit of Work* para pegar todos os *aggregate roots*:
  - `getPersistStack` para entidades gerenciadas.
  - `getRemoveStack` para entidades removidas.
- Criação de um array para armazenar os *aggregate roots*.

## Publicação de Eventos
- Para cada *aggregate root*, o *Domain Event Manager* deve publicar o evento.
- Uso de `await` para garantir que os eventos sejam publicados sequencialmente.
- Possibilidade de listeners manipularem outros agregados ou gerarem novos eventos.

## Estrutura do Método Run
- Sugestão de criar um método `run` que recebe um callback e retorna uma promessa.
- Estrutura do método `run`:
  - Início do processo com `await`.
  - Uso de `try` para erro e chamada do método `fail` em caso de exceção.

### Exemplos de Implementação
- O método `run` pode ser utilizado para processamento de negócios, como:
  - Criação.
  - Atualização.
- O commit do *Unit of Work* deve ocorrer no final do processamento.

## Conclusão
- Integração do *Application Service* concluída.
- Na próxima aula, serão feitos testes para validar a integração criada.
- Continuação da saga no aprendizado de *Domain Driven Design*.

## Próximos Passos
- Revisar conceitos abordados.
- Preparar exemplos práticos para a próxima aula.
- Focar na implementação e testes dos processos discutidos.



---

## modulo_8_11257.mp4

# Notas de Estudo: Integração em Domain Driven Design

## Introdução
- Continuação do estudo sobre **Domain Driven Design** (DDD).
- Foco na integração de processos de negócio com o **Domain Event Manager**.

## Contexto da Aula Anterior
- Criação do **Gerenciador de Eventos** (Domain Event Manager).
- Objetivo da aula: integrar eventos de domínio com processos de negócio.

## Fluxo de Eventos de Negócio
- **Criação de um Partner**:
  - Registro do evento de criação.
  - Listener recebe o evento e executa processos de negócio.
- Importância da execução **antes do commit**:
  - Permite que o **Unit of Work** gerencie e execute todas as mudanças no banco de dados.

## Delegação de Eventos
- Não é ideal registrar eventos diretamente em cada Application Service.
- Sugestão: delegar o gerenciamento a um outro tipo de serviço.
- Introdução de um conceito de **ciclo de vida** do Application Service:
  - Início, finalização e possibilidade de falha.

## Estrutura do Application Service
1. **Criação da Classe ApplicationService**:
   - Responsável por gerenciar o ciclo de vida dos processos de negócio.
   - Localização na camada de aplicação do Common.

2. **Construtor do ApplicationService**:
   - Recebe:
     - **Unit of Work** (referência da interface).
     - **Domain Event Manager** (gerenciador de eventos).

3. **Ciclo de Vida do Processo de Negócio**:
   - **Início** (`Start`):
     - Chamada para iniciar o processo.
   - **Finalização** (`Finish`):
     - Execução do commit do **Unit of Work**.
   - **Falha** (`Fail`):
     - Lidar com erros ocorridos durante o processo.

## Implementação de Métodos
- Adicionar métodos para obter **Aggregate Routes**:
  - Método no **Unit of Work** para retornar todas as entidades gerenciadas (persist stack).
  - Utilização de `getRemoveStack` para coletar entidades removidas.
  
### Manipulação de Aggregate Routes
- Concatenar resultados em um único array utilizando o operador rest.
- Publícação dos eventos para cada aggregate route no **Domain Event Manager**:
  - Atenção ao uso de `await` para garantir a execução sequencial dos listeners.

## Execução do Método Run
- Sugestão de criar um método `run` que:
  - Receba um callback.
  - Retorne uma promessa com o resultado da execução.

### Estrutura do Método Run
- Uso de `try-catch` para lidar com erros:
  - Chamar o método `fail` em caso de erro.
- Simplificação do código ao evitar a necessidade de `await` no commit.

## Conclusão
- Integração do **Application Service** concluída.
- Próxima aula focará em testes e a integração total do sistema.
- Continuação da jornada no aprendizado de DDD.

## Chaves para Estudo
- **Domain Driven Design**: Estrutura e conceitos fundamentais.
- **Unit of Work**: Importância na transação de dados.
- **Ciclo de Vida do Application Service**: Etapas de início, finalização e falha.
- **Aggregate Routes**: Compreensão e manipulação de entidades no contexto de eventos de domínio.
- **Eventos de Domínio**: Publicação e manejo de eventos no sistema.

## Sugestões de Prática
- Implementar um projeto de exemplo utilizando os conceitos discutidos.
- Testar a integração do **Domain Event Manager** com diferentes processos de negócio.
- Experimentar a criação de logs e o tratamento de erros durante o ciclo de vida do Application Service.



---

## modulo_8_11261.mp4

# Resumo do Módulo de Domain Driven Design (DDD)

## Introdução
- O módulo está chegando ao final, e algumas dúvidas recorrentes serão abordadas.
- O foco principal é sobre **agregados** e suas regras.

## Regras dos Agregados
### Definição de Agregado
- Um agregado deve ser uma *transação atômica*:
  - Se um agregado contém subentidades ou objetos de valor, deve-se salvar tudo ou nada.
  - Se não puder salvar tudo, deve-se descartar o que foi tentado.

### Proteção das Invariantes
- O agregado protege as *invariantes de consistência*.
- Todo comando deve passar pelo agregado, que garante que todas as regras de negócio sejam satisfeitas.

### Referências entre Agregados
- Um agregado pode se referenciar a outro apenas por *identidade*.
  - Exemplo: Um evento se refere a um parceiro através do ID do parceiro.

## Transações e Agregados
### Regra Crítica
- Somente **um agregado** deve ser processado por transação.
  - Isso significa que, durante a persistência, deve-se evitar manipular múltiplos agregados ao mesmo tempo.
  
### Exemplo Prático
- No método `create` do `orderService`, a persistência envolve três agregados: `spotReservation`, `order`, e `event`. Isso é considerado uma violação da regra.

### Abordagem Recomendada
- Processar um único agregado e, se necessário, usar *fila de mensagens* para processar outros agregados posteriormente.
- A lógica de negócios pode ser dividida em etapas, onde algumas podem ser processadas com um atraso.

## Consistência Eventual
- A consistência pode ser *eventual* em sistemas de grande escala:
  - É aceitável que um processo de negócio não seja finalizado instantaneamente.
  - Domain experts podem compreender atrasos pequenos na consistência.

## Quebra das Regras de Agregados
### Razões para Quebrar Regras
1. **Conveniência da Interface**:
   - Necessidade de lidar com múltiplos agregados ao mesmo tempo.
2. **Falta de Mecanismos Técnicos**:
   - Em situações em que não é possível implementar a consistência futura.
3. **Aplicações Legadas**:
   - Respeitar transações globais em sistemas existentes.

### Justificativa
- Quebrar regras deve ser bem justificado, respeitando as questões de negócio.
- O DDD não fornece respostas universais; é necessário adaptar as regras às realidades do negócio.

## Conclusão
- O ideal é manter um agregado por transação e minimizar o impacto sobre outros agregados.
- O uso de *listeners* e mensageria pode facilitar a manutenção da consistência.
- O DDD deve ser aplicado com flexibilidade, considerando as necessidades do negócio.

## Próximos Passos
- Continuar a explorar outras perguntas e conceitos dentro do módulo.
- Manter a prática e a discussão sobre o DDD em contextos reais de desenvolvimento.



---

## modulo_8_11262.mp4

# Resumo da Aula sobre Domain-Driven Design (DDD)

## Introdução
- O módulo de DDD está chegando ao fim.
- Discussão sobre dúvidas recorrentes, especialmente sobre agregados.

## Regras dos Agregados

### Definição de Agregado
- Todo *agregado* deve ser uma transação *atômica*.
  - Se parte do agregado for salva, tudo deve ser descartado.
  - O agregado protege as invariantes de consistência.

### Consistência
- Todo comando passa pelo agregado, que garante a consistência das regras de negócio.
- Não se deve acessar subentidades diretamente; sempre através do agregado.

### Referência entre Agregados
- Um agregado só pode se referir a outros por *identidade*.
  - Exemplo: em um evento, a identidade de um parceiro é utilizada, mantendo acoplamento fraco.

## Processamento de Transações

### Regra Fundamental
- **Somente um agregado deve ser processado por transação.**
  - Exemplo: no método `create` do `orderService`, deve-se considerar quantos agregados estão sendo persistidos.

### Visão do Vernon
- Utilizar um único agregado para processar regras de negócio.
- Se outros agregados forem afetados, o processamento deve ser feito posteriormente, de forma assíncrona (ex: filas de mensagens).

### Importância do Tempo Real
- Em sistemas grandes, não é viável processar todos os agregados na mesma transação.
- Reconhecer que a consistência pode demorar alguns segundos é essencial.

## Quebra das Regras de Agregados

### Motivos para Quebrar as Regras
1. **Conveniência da Interface de Usuário**:
   - Às vezes, é necessário lidar com múltiplos agregados simultaneamente.
  
2. **Falta de Mecanismos Técnicos**:
   - Limitações técnicas podem forçar a quebra das regras.
  
3. **Condições de Negócio**:
   - Em alguns casos, a consistência precisa ser imediata (como pagamentos).

### Exemplos de Quebra
- Em um cenário de pagamento com cartão de crédito, a reserva deve ser confirmada imediatamente.
- É possível usar listeners para processar ações de forma assíncrona.

### Importância da Justificação
- Quebrar regras deve ser bem justificado, respeitando as questões técnicas e de negócio.
- As regras do DDD não são absolutas; o foco deve ser sempre nas necessidades de negócio.

## Conclusão
- A aula enfatiza a importância de manter um agregado por transação e de adiar o impacto em outros agregados quando possível.
- A flexibilidade e a compreensão do contexto de negócio são cruciais na aplicação das regras de DDD.

## Próximos Passos
- Continuar a explorar e responder dúvidas ao longo do módulo.
- Preparar-se para discussões futuras sobre outros tópicos relacionados ao DDD.



---

## modulo_8_11263.mp4

# Resumo da Aula sobre Domain-Driven Design (DDD)

## Introdução
- A aula faz parte do módulo de DDD e aborda questões recorrentes sobre agregados e transações no contexto de design de software.
- O foco principal é esclarecer dúvidas sobre a regra dos agregados.

## Regra dos Agregados
### Definição
- **Agregados**: Conjuntos de entidades e objetos de valor que são tratados como uma unidade.
- Cada agregado deve ser uma **transação atômica**:
  - Ou se salva tudo, ou não se salva nada.
  - Se uma parte do agregado não puder ser salva, todo o agregado deve ser descartado.

### Função dos Agregados
- Proteger as *invariantes de consistência*:
  - Todas as transações e comandos passam pelo agregado.
  - O agregado garante que todas as regras de negócio estão satisfeitas.

### Referência entre Agregados
- Um agregado pode referenciar outros agregados apenas por **identidade**:
  - Exemplo: um evento pode referenciar um parceiro apenas pelo ID, mantendo um acoplamento fraco.

## Processamento de Transações
### Regra Crítica
- **Somente um agregado deve ser processado por transação**:
  - Importante para evitar complexidade em sistemas de grande escala.
  - Exemplos de agregados em um serviço podem incluir `spotReservation`, `order`, e `evento`.

### Estratégia de Processamento
- Se um processo de negócio afeta vários agregados, deve-se:
  - Processar um agregado de cada vez.
  - Usar filas de mensagens para atrasar o processamento de outros agregados.

### Consistência Eventual
- Reconhecer que nem todos os processos precisam ser instantâneos.
- Em sistemas grandes, é aceitável que haja um pequeno atraso na consistência dos dados.

## Quebra das Regras dos Agregados
### Razões para Quebrar as Regras
1. **Conveniência na Interface do Usuário**:
   - Necessidade de salvar múltiplos agregados ao mesmo tempo.
  
2. **Falta de Mecanismos Técnicos**:
   - Limitações na infraestrutura que não permitem a implementação ideal das regras.

3. **Aplicações Legadas**:
   - Respeitar o funcionamento de sistemas existentes que não podem ser alterados facilmente.

4. **Desempenho nas Consultas**:
   - Em algumas situações, referências diretas por ID podem ser insuficientes para garantir um bom desempenho.

### Justificação Necessária
- É crucial justificar claramente qualquer quebra de regra.
- As decisões devem sempre priorizar as *questões de negócio*, que são consideradas sagradas no DDD.

## Conclusão
- O DDD não fornece respostas absolutas. Cada projeto pode exigir adaptações nas regras.
- Tente sempre manter um agregado por transação e adiar o impacto em outros agregados quando possível.
- Continuaremos a explorar mais perguntas e tópicos relevantes durante o módulo.

## Próximos Passos
- As aulas seguintes abordarão mais perguntas e aprofundarão outros aspectos do DDD.
- É importante continuar praticando e aplicando os conceitos discutidos.



---

## modulo_8_11264.mp4

## Resumo da Aula sobre Domain-Driven Design (DDD)

### Introdução
- A aula faz parte do módulo de DDD e aborda questões recorrentes sobre o tema.
- O foco principal é discutir os **agregados** e suas regras.

### Regras dos Agregados
- **Transação Atômica**: 
  - Um agregado deve ser salvo como uma única transação; se não for possível salvar tudo, deve-se descartar a operação.
  
- **Proteção de Invariantes**:
  - O agregado garante que todas as regras de negócio sejam mantidas e consistentes.
  - Nenhuma subentidade pode ser acessada sem passar pelo agregado.

- **Referência por Identidade**:
  - Um agregado só pode referenciar outros agregados por sua identidade.
  - Exemplo: Um evento pode referenciar um parceiro apenas por seu ID, resultando em um acoplamento fraco.

### Regra de Processamento de Agregados
- **Somente um Agregado por Transação**:
  - A regra é que apenas um agregado deve ser processado por transação.
  - Exemplo: Em um serviço de pedidos (`orderService`), se vários agregados estão envolvidos (como `spotReservation`, `order`, e `event`), isso pode indicar um problema.

- **Dificuldades em Sistemas de Grande Escala**:
  - Em sistemas grandes, é comum que um processo de negócio seja dividido em várias etapas, que podem levar tempo entre si.
  - O conceito de **consistência eventual** é introduzido, reconhecendo que nem tudo precisa ser processado ao mesmo tempo.

### Delegação e Processamento Assíncrono
- **Uso de Listeners e Mensageria**:
  - É possível usar listeners para processar operações em segundo plano.
  - Exemplo: Um listener pode ser configurado para ouvir quando um pedido é pago e, em seguida, processar a reserva de um spot.

- **Adiar Processamento**:
  - Quanto mais se puder adiar o processamento de agregados, melhor será a gestão da consistência de dados e das regras de negócio.

### Quebrando as Regras dos Agregados
- O livro de Vernon menciona situações em que as regras podem ser quebradas:
  1. **Conveniência da Interface de Usuário**: 
     - Às vezes, a interface exige que vários agregados sejam manipulados simultaneamente.
  2. **Falta de Mecanismos Técnicos**: 
     - Em algumas situações, não há como implementar a consistência futura devido a restrições técnicas ou de negócio.
  3. **Aplicações Legadas**:
     - Em sistemas legados, pode ser necessário trabalhar com transações globais.

### Considerações Finais
- **Justificativa para Quebras**:
  - Sempre que uma regra for quebrada, é essencial ter uma justificativa sólida e compreender o impacto no negócio.
  
- **Regras de DDD como Diretrizes**:
  - As regras do DDD não são absolutas; é importante respeitar as necessidades do negócio e adotar um modelo que funcione para a situação específica.
  
- **Próximos Passos**:
  - A aula continuará a explorar outras perguntas sobre DDD nos próximos encontros.

### Conclusão
- O entendimento e a aplicação correta das regras dos agregados são fundamentais para garantir a consistência e a eficácia dos sistemas desenvolvidos com DDD.



---

## modulo_8_11265.mp4

# Resumo do Módulo de Domain Driven Design

## Introdução
- O módulo de Domain Driven Design (DDD) foi complexo e desafiador.
- A *experimentação* é fundamental para entender e aplicar DDD.

## Livros Recomendados
- Para uma boa compreensão de DDD, é essencial ler:
  - **Livro Azul**: "Domain-Driven Design" de Eric Evans.
  - **Livro Vermelho**: "Implementing Domain-Driven Design" de Vaughn Vernon.
- Outros livros sobre DDD também são recomendados para aprofundar o conhecimento.

## Prática e Aplicação
- Para se tornar proficiente em DDD, é necessário:
  - Identificar um problema real na sua empresa ou um projeto.
  - Desenvolver os *subdomínios* do problema.
  - Começar com o *design estratégico* e, em seguida, o *design tático*.
  - Modelar os *agregados* e trabalhar com testes para garantir a funcionalidade.

## Refinamento do Modelo
- O conhecimento sobre o domínio se aprofunda com a prática.
- O *refinamento* das entidades e do modelo é um processo contínuo:
  - À medida que você aprende mais, o modelo se torna mais robusto.
  - A prática leva ao desenvolvimento de um software que realmente atende às necessidades do usuário.

## Desafios Técnicos
- Cada linguagem de programação apresenta seus próprios desafios:
  - Algumas têm bibliotecas mais adequadas para DDD, enquanto outras podem não ter.
- É importante saber contornar os aspectos técnicos da implementação de DDD.

## Considerações Finais sobre DDD
- DDD não é uma solução universal:
  - Deve ser aplicado onde é realmente necessário, não em todo tipo de software.
  - Não é uma "bala de prata" para todos os problemas de desenvolvimento.
- Em projetos simples, uma *arquitetura hexagonal* ou uma *camada de serviços* pode ser suficiente.

## Agradecimentos e Encerramento
- Agradecimento pela oportunidade de ensinar e pela participação dos alunos.
- Incentivo para continuar os estudos e buscar esclarecimento de dúvidas.

## Dicas de Estudo
1. **Leitura dos livros recomendados**: Comece com os livros de Evans e Vernon.
2. **Prática contínua**: Trabalhe em projetos reais para aplicar os conceitos de DDD.
3. **Revisão e Reflexão**: Revise o que aprendeu e como pode aplicar na prática.
4. **Participação em fóruns**: Utilize canais disponíveis para tirar dúvidas e trocar experiências com outros.

Mantenha-se motivado e continue explorando o vasto mundo do Domain Driven Design!



---

## modulo_8_11266.mp4

## Resumo do Módulo de Domain Driven Design

### Introdução
- O módulo sobre *Domain Driven Design (DDD)* foi desafiador e complexo.
- É essencial entender que DDD não é uma abordagem simples e requer muita prática e experimentação.

### Livros Recomendados
- Para entender DDD, é fundamental ler:
  - **"Domain-Driven Design"** de Eric Evans (livro azul)
  - **"Implementing Domain-Driven Design"** de Vaughn Vernon (livro vermelho)
- Outros livros de Vaughn Vernon também abordam DDD e podem ser explorados.

### Prática e Aplicação
- A prática é crucial para dominar DDD:
  1. Escolha um problema real da sua empresa ou uma aplicação que deseja desenvolver.
  2. Inicie com o *design estratégico*.
  3. Prossiga para o *design tático*.
  4. Modele os *agregados*.
  5. Realize testes para garantir o funcionamento adequado.
  
- O refinamento do modelo é um processo contínuo em que o entendimento do domínio se aprofunda.

### Desafios Técnicos
- Diferentes linguagens de programação apresentam desafios variados:
  - Algumas possuem bibliotecas melhores para DDD.
  - É importante saber contornar os aspectos técnicos.

### Considerações Finais sobre DDD
- **DDD não é uma solução universal**:
  - Não deve ser aplicado em todos os contextos; não é uma "bala de prata".
  - Pode ser desnecessário em softwares simples, onde uma arquitetura hexagonal ou uma camada de serviços pode ser suficiente.
  
- A implementação de DDD pode tornar o desenvolvimento mais burocrático, mas essa estruturação é necessária para:
  - Separar responsabilidades.
  - Manter a qualidade do software ao longo do tempo.
  - Atender às necessidades dos usuários.

### Conclusão
- A jornada de aprendizado em DDD requer meses de trabalho e dedicação.
- O instrutor expressa gratidão pela oportunidade de ensinar e se coloca à disposição para tirar dúvidas.
- Encorajamento para continuar os estudos e explorar outros canais de aprendizado.

### Agradecimentos
- Agradecimentos aos participantes do curso e à equipe da FullCycle.
- Expectativa de encontros futuros e continuidade dos estudos.

--- 

### Dicas para Estudo
- **Leia os livros recomendados** para entender os fundamentos teóricos de DDD.
- **Pratique regularmente** para aplicar os conceitos aprendidos em situações reais.
- **Participe de discussões e tire dúvidas** com colegas e instrutores para aprofundar seu entendimento.
- **Explore diferentes linguagens e ferramentas** que facilitam a implementação de DDD.



---

## modulo_8_11267.mp4

# Resumo do Módulo de Domain Driven Design (DDD)

## Introdução
- Encerramento do módulo de Domain Driven Design (DDD).
- DDD é uma abordagem complexa que requer **experiência** e **prática**.

## Leituras Recomendadas
- É fundamental ler os seguintes livros para entender DDD:
  - **Livro Azul** (de Eric Evans)
  - **Livro Vermelho** (de Vaughn Vernon)
- Outros livros sobre DDD também são recomendados.

## Prática é Essencial
- Para se tornar proficiente em DDD, é necessário:
  - **Escolher um problema** na sua empresa ou uma aplicação para desenvolver.
  - Trabalhar com:
    - **Design estratégico**: identificação de subdomínios.
    - **Design tático**: modelagem e refinamento de agregados.
    - **Testes**: garantir que a aplicação funcione corretamente.
  
## Refinamento do Modelo
- O conhecimento sobre o domínio aumenta com o tempo, permitindo:
  - **Aperfeiçoamento das entidades** e do modelo.
  - Superação dos desafios associados a diferentes linguagens de programação.

## Considerações Técnicas
- DDD não é uma solução universal:
  - **Não é uma "bala de prata"** que resolve todos os problemas.
  - Deve ser aplicado somente onde é apropriado.
- Para aplicações simples, considere:
  - Uma **arquitetura hexagonal**.
  - Uma **camada de serviços** como alternativa suficiente.

## Burocracia e Manutenção
- A estrutura de DDD cria mais arquivos e pode parecer burocrática, mas:
  - **Separação de responsabilidades**: crucial para a manutenção do software.
  - Garante que o software satisfaça as necessidades do usuário ao longo do tempo.

## Conclusão
- A jornada de aprendizado em DDD é longa e trabalhosa, mas recompensadora.
- Incentivo à continuidade dos estudos e à busca por esclarecimentos.

## Agradecimentos
- Agradecimento pela oportunidade de ensinar e pela participação no curso.
- Disponibilidade para tirar dúvidas e suporte contínuo.

## Dicas Finais
- **Continuem estudando** e praticando.
- Participem ativamente dos canais de comunicação para resolver dúvidas e compartilhar experiências.



---

## modulo_8_11268.mp4

# Resumo do Módulo de Domain Driven Design

Salve, Deus! Este resumo finaliza o módulo sobre *Domain Driven Design (DDD)*, uma abordagem complexa que requer dedicação e prática. Vamos explorar os principais pontos discutidos.

## Introdução ao DDD

- **DDD não é simples**: É uma metodologia que exige tempo e esforço para ser compreendida e aplicada corretamente.
- **Experiência prática**: É vital praticar DDD em projetos reais para aprimorar a habilidade.

## Leitura Recomendada

- **Livros Essenciais**:
  - *Domain-Driven Design* - Eric Evans (Livro Azul)
  - *Implementing Domain-Driven Design* - Vaughn Vernon (Livro Vermelho)
  
- **Outros Recursos**: Existem outros livros e materiais sobre DDD que podem ser úteis.

## Fases do DDD

1. **Design Estratégico**:
   - Identificação dos subdomínios.
   - Definição de limites contextuais.
  
2. **Design Tático**:
   - Modelagem de agregados.
   - Refinamento das entidades conforme o entendimento do domínio evolui.

## Importância da Prática

- **Desenvolvimento Iterativo**: Ao trabalhar em um problema específico, você vai refinando seu modelo e aprendendo sobre os desafios técnicos.
- **Testes**: A prática de testes é fundamental para garantir que o software funcione conforme esperado.

## Desafios Técnicos

- Cada linguagem de programação tem suas particularidades e desafios:
  - Algumas linguagens têm bibliotecas que facilitam a implementação de DDD.
  - É importante saber como contornar as limitações técnicas.

## Considerações Finais sobre DDD

- **Uso Adequado**: DDD não deve ser aplicado em todos os projetos; é importante avaliar se é a abordagem correta.
- **Não é uma solução mágica**: Não resolve todos os problemas de software. Para aplicações simples, uma arquitetura hexagonal ou uma camada de serviços pode ser suficiente.
  
## Agradecimentos e Conclusão

- Agradecimento pela participação no curso e incentivo à continuidade dos estudos.
- Disponibilidade para esclarecimento de dúvidas por parte do instrutor e da equipe.

## Dicas para Estudo

- **Pratique com projetos reais**: Tente aplicar DDD em problemas que você enfrenta na sua empresa ou em projetos pessoais.
- **Revisite os conceitos frequentemente**: O entendimento do DDD melhora com a repetição e a aplicação prática.
- **Participe de comunidades**: Troque experiências com outros profissionais que estão aprendendo ou já aplicam DDD.

Espero que este resumo ajude a consolidar os conceitos de DDD e a preparar você para aplicar esses conhecimentos na prática! Até a próxima!



---

## modulo_8_11303.mp4

# Resumo da Aula: Mapeamento em Entidade Relacional com microRM

## Introdução
- O foco da aula é sobre *mapeamento em entidade relacional* utilizando o microRM.
- A abordagem envolve o uso de *decorators* para simplificar o mapeamento sem comprometer o domínio da aplicação.

## Mapeamento de Entidades
- Utilização de *Entity Schema* para definir campos e tipos de dados.
- Exemplos de como configurar os campos:
  - `name`: tipo *varchar*.
  - `id`: chave primária, com possibilidade de usar *uuid* ou valor binário.

### Estrutura do Código
- Criação do arquivo `partnerSchema`.
- Importação da entidade `partner` do domínio.
- Organização do código em uma única classe para limpar a estrutura.

## Configuração do MicroRM
- Importação do driver MySQL e configuração do banco de dados.
- Criação de uma instância do *Entity Manager*.
- Necessidade de usar *async/await* ao trabalhar com promessas.

### Exemplo de Criação de Entidade
1. Criação de um `partner` utilizando `partner.create()`.
2. Persistência da entidade com o método `persist`.
3. Uso do método `flush` para efetivar a operação no banco de dados.

## Testes e Validações
- Verificação da criação da tabela `partner` no banco de dados.
- Consulta dos dados inseridos utilizando SQL:
  - `SELECT * FROM partner`.
- Importância de verificar se os dados estão sendo persistidos corretamente.

### Problemas Comuns
- O método `persist` apenas mantém a entidade na memória, não realizando a verificação no banco.
- Utilização do método `clear` para limpar o *Unit of Work* e garantir a integridade dos dados.
- A necessidade de forçar a consulta ao banco para obter dados atualizados.

## Conclusão
- A persistência e recuperação correta dos dados são fundamentais para a integridade do modelo.
- Importância de ajustes no mapeamento relacional para garantir que o modelo rico seja preservado tanto na persistência quanto na recuperação de dados.

## Dicas Importantes
- Sempre utilize `await` em chamadas que retornam promessas.
- Limpe o *Unit of Work* antes de realizar consultas para evitar resultados inconsistentes.
- Teste frequentemente para verificar se as operações de CRUD estão funcionando como esperado.

## Próximos Passos
- Continuar a otimização do mapeamento relacional.
- Explorar mais sobre padrões como *Unit of Work* e sua aplicação prática.



---

## modulo_8_11653.mp4

# Resumo da Palestra: Domain Driven Design MBA Full Cycle Architecture

## Introdução
- Título da palestra: **Domain Driven Design MBA Full Cycle Architecture**.
- O foco será:
  1. O que é Domain Driven Design (DDD)?
  2. Por que usar DDD?
  3. Padrões estratégicos e táticos.
  4. Arquitetura de software que suporta DDD.

## O que é Domain Driven Design (DDD)?
- **DDD** é uma abordagem para o design de modelos de software.
- Envolve uma equipe que trabalha em conjunto com **especialistas técnicos** e **especialistas de domínio** para resolver problemas de negócios complexos.
- O termo *domínio* refere-se a uma esfera de conhecimento.

### Definição de Domínio
- Um domínio pode ser visto como:
  - Um **reino** ou **propriedade** de conhecimento.
  - Uma *esfera de conhecimento* que a equipe explora para resolver problemas.

### Trabalho em Equipe
- A equipe deve incluir:
  - **Especialistas de domínio** (expertos do negócio).
  - **Profissionais técnicos** (desenvolvedores de software).
- O trabalho conjunto é essencial para a *modelagem de problemas complexos*.

## Contextualidade do DDD
- DDD é **contextual**, focando em problemas complexos.
- Não é adequado para soluções de software simples.
- Um conceito-chave é o **bounded context** (contexto delimitado):
  - Um ambiente no qual uma linguagem é desenvolvida.
  - A linguagem é *restrita* ao que é necessário para suportar o modelo de software.

### Linguagem Ubíqua
- A linguagem desenvolvida dentro do *bounded context* é chamada de **linguagem ubíqua**.
- Características da linguagem ubíqua:
  - Utilizada apenas dentro do contexto da equipe.
  - Permite comunicação clara sobre o problema de negócios.
  - As definições são precisas e aplicáveis apenas dentro desse contexto.

## Padrões de Modelagem em DDD
- DDD inclui ferramentas de modelagem **estratégicas** e **táticas**.
- As ferramentas estratégicas focam na **inovação**.
- As ferramentas táticas ajudam em decisões de modelagem de software mais detalhadas.

## Conclusão
- A palestra cobre a importância do DDD na modelagem de software para resolver problemas complexos.
- A colaboração entre equipes técnicas e de negócios é fundamental.
- A criação de uma linguagem comum e um contexto delimitado são essenciais para o sucesso do DDD.

## Estrutura para Estudo
- **Revisão dos conceitos principais**:
  - DDD, domínio, contexto delimitado, linguagem ubíqua.
- **Prática em equipe**:
  - Exercitar a formação de uma linguagem ubíqua em um projeto fictício.
- **Estudo de padrões**:
  - Analisar exemplos de ferramentas estratégicas e táticas em DDD.

Com essa estrutura, você terá uma visão clara dos conceitos abordados na palestra sobre Domain Driven Design, bem como os fundamentos para aplicar esses conceitos em projetos de software.



---

## modulo_8_11654.mp4

# Notas de Estudo: Design Orientado a Domínio (DDD) na Arquitetura de Ciclus Completo

## Introdução
- **Título**: Design Orientado a Domínio MBA Arquitetura de Ciclo Completo
- **Objetivos da palestra**:
  1. O que é Design Orientado a Domínio (DDD)?
  2. Por que usar DDD?
  3. Padrões estratégicos e táticos.
  4. Arquitetura de software que suporta DDD.

## O que é Design Orientado a Domínio (DDD)?
- **Definição**: DDD é uma abordagem para o *design* de modelos de software, focando na colaboração entre equipes técnicas e especialistas do domínio para resolver problemas de negócios complexos.
- **Equipe**: Composta por especialistas técnicos e de domínio, que realizam um processo de "crunching" de conhecimento.

### Domínio
- O termo *domínio* refere-se a uma esfera de conhecimento, semelhante a um "reino" ou "propriedade".
- O foco do DDD é em problemas *complexos*, não em soluções de propósito geral para desenvolvimento de software simples.

## Contextualização do DDD
- **Contexto Bounded**: O conceito de *bounded context* é crucial, onde uma linguagem específica é desenvolvida para suportar o modelo de software.
- **Linguagem Ubíqua**: 
  - A equipe desenvolve uma *linguagem ubíqua*, que é um vocabulário compartilhado dentro do contexto do projeto.
  - Esta linguagem é restrita ao que é necessário para o modelo de software, garantindo clareza e precisão na comunicação.

## Elementos do DDD
### Arquiteturas Envolvidas
- **Arquitetura de Negócios**: Estrutura organizacional e modelo de negócios.
- **Arquitetura Social**: Interações e dinâmicas entre membros da equipe.
- **Arquitetura Técnica**: Aspectos técnicos do desenvolvimento de software.

### Padrões de Modelagem
- **Padrões Estratégicos**: Focados na inovação e no mapeamento do domínio.
- **Padrões Táticos**: Ajudam na tomada de decisões de modelagem de software em detalhes finos.

## Conclusão
- O Design Orientado a Domínio é uma abordagem poderosa para enfrentar desafios complexos em desenvolvimento de software, enfatizando a colaboração e a definição precisa de linguagens dentro de contextos específicos.
- O uso de DDD pode transformar a forma como equipes lidam com problemas de negócios complexos, resultando em soluções mais eficazes e adaptadas às necessidades específicas do domínio. 

## Estrutura de Estudo
- **Revisar conceitos chave**: DDD, domínio, contexto bounded e linguagem ubíqua.
- **Exemplos práticos**: Analisar cases de uso de DDD em empresas.
- **Discussão em grupo**: Debater como a abordagem pode ser aplicada em diferentes cenários de negócios.

## Sugestões para Estudo
- **Leitura adicional**: Livros e artigos sobre DDD.
- **Prática**: Tentar aplicar os conceitos em projetos reais ou simulados.
- **Reflexão**: Considerar como a arquitetura de software pode impactar a implementação de DDD em ambientes de trabalho.

