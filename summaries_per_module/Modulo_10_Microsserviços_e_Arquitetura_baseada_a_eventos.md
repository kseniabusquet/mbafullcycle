# Resumos dos vídeos

## modulo_10_11510.mp4

# Módulo sobre Arquitetura Baseada em Micro-serviços

## Introdução
- **Saudação**: O palestrante dá as boas-vindas aos participantes.
- **Objetivo do módulo**: Apresentar os fundamentos da arquitetura baseada em micro-serviços.

## Expectativas do Módulo
- **Conceitos Fundamentais**: A maioria das falhas em implementações de micro-serviços ocorre pela falta de entendimento dos conceitos.
  - **Público-alvo**: Desenvolvedores sêniors, tech leads e arquitetos.
- **Motivos para Falhas**:
  - Falta de compreensão dos *conceitos* por trás da arquitetura.
  - Uso da arquitetura por motivos inadequados.

## Conteúdos Abordados
O módulo abordará os seguintes tópicos:

1. **Fundamentos da Arquitetura de Micro-serviços**
   - Quando utilizar micro-serviços.
   - Quando evitar o uso de micro-serviços.
   - Funcionamento da arquitetura.

2. **Minimizando Riscos**
   - Estratégias para evitar a "estrela da morte".
   - Compreensão das diferenças entre *coreografia* e *orquestração* de micro-serviços.

## Importância da Teoria
- **Simplicidade dos Sistemas**: Desenvolver sistemas pequenos é relativamente simples.
- **Desafio da Composição**: O verdadeiro desafio está em como organizar e compor esses pequenos sistemas.

## Relevância no Mercado
- **Empresas Grandes**: A arquitetura baseada em micro-serviços é comum em grandes empresas.
- **Motivação Correta**: Muitas empresas adotam micro-serviços por razões erradas, o que pode levar ao insucesso.

## Conclusão
- **Importância do Módulo**: Este é um dos módulos mais importantes do curso.
- **Preparação para o Futuro**: O conhecimento adquirido será útil em qualquer empresa que utilize essa arquitetura.

## Dicas para Estudo
- **Revisar os Conceitos**: Revisar os fundamentos de micro-serviços regularmente.
- **Refletir sobre Aplicações Práticas**: Pensar sobre como esses conceitos se aplicam às situações reais em empresas.
- **Participar Ativamente**: Engajar-se nas discussões e práticas propostas durante o módulo para melhor compreensão.



---

## modulo_10_11511.mp4

# Resumo da Aula sobre Arquitetura de Microserviços

## Introdução
Nesta aula, discutimos as características e desafios da arquitetura de microserviços, além de compará-la com sistemas monolíticos. Focamos em vantagens como deploy menos arriscado e a especialização das equipes, mas também ressaltamos a complexidade envolvida.

## Características da Arquitetura de Microserviços

### 1. Deploy Menos Arriscado
- **Vantagem Principal**: Se um microserviço falha durante o deploy, os demais continuam funcionando.
  - Exemplo: Em um sistema com 100 microserviços, se um falha, 99 ainda estão operacionais.
- **Mecanismos de Fallback**: Implementação de políticas que permitem a degradação gradual do sistema, mantendo a capacidade de atender requisições.

### 2. Complexidade Aumentada
- **Desafios do Setup**:
  - Cada microserviço exige seu próprio processo de configuração.
  - Necessidade de múltiplas *pipelines* de CI/CD (Integração Contínua/Entrega Contínua).
  - Diversidade de sistemas para análise estática de código e revisões.
- **Comunicação Complexa**: Comunicação frequente entre múltiplos microserviços, aumentando a complexidade do ambiente.

## Cuidados ao Escolher Microserviços
- A escolha por microserviços deve ser cuidadosa para evitar decisões inconsequentes.
- Empresas grandes frequentemente têm equipes de plataformas dedicadas para organizar e padronizar o setup.

## Vantagens da Especialização de Equipes
### 1. Equipes Especializadas por Microserviços
- Desenvolvimento de expertise em domínios específicos.
  - Exemplo: Uma equipe focada em emissão de notas fiscais pode tornar-se altamente eficiente nessa tarefa.
- **Benefícios**:
  - Melhora na performance e na resolução de problemas de negócio.
  - Aumento do valor agregado à empresa pelo desenvolvimento de funcionalidades específicas.

### 2. Eficiência na Resolução de Problemas
- Equipes que se especializam em um domínio tendem a resolver problemas de forma mais ágil e eficaz.
  - Exemplo: Um time dedicado ao *Digital Rights Management* (DRM) em uma plataforma como a Netflix se torna mais competente ao longo do tempo.

## Conclusão
- A arquitetura de microserviços apresenta vantagens significativas, mas também traz desafios relacionados à complexidade e à necessidade de uma boa organização.
- No próximo vídeo, abordaremos o tema da escala e os pontos importantes relacionados a este aspecto.

## Próximos Passos
- Estudar sobre os desafios e estratégias para escalar uma arquitetura de microserviços.
- Refletir sobre a importância da especialização das equipes e a adoção de melhores práticas no desenvolvimento.



---

## modulo_10_11512.mp4

# Estudo sobre Micro-serviços

## Introdução
No vídeo anterior, discutimos quando optar por sistemas monolíticos. Agora, vamos explorar quando é apropriado escolher arquiteturas baseadas em micro-serviços.

## Quando optar por Micro-serviços

### 1. **Necessidade de Escala**
- *Escalabilidade de times*: 
  - Micro-serviços são ideais quando há uma grande quantidade de desenvolvedores.
  - Sistemas monolíticos podem escalar, mas gerenciar grandes equipes em um único sistema se torna complexo.
  - Escalar times é um desafio maior em sistemas monolíticos.

### 2. **Contextos de Unidades de Negócio Definidos**
- Definição clara dos contextos:
  - É necessário saber onde começa e termina cada parte do sistema.
  - Micro-serviços fazem mais sentido quando os contextos de negócio estão bem definidos.
  - Em projetos com muitos contextos desconhecidos, micro-serviços podem não ser a melhor escolha.

### 3. **Escalabilidade de Partes Específicas do Sistema**
- Escalar partes sem escalar o sistema inteiro:
  - Exemplo: em eventos como Black Friday, escalar apenas o catálogo de produtos é mais eficiente do que escalar todo o sistema.
  - Em grandes sistemas, como o da Amazon, a economia de custo pode ser significativa ao escalar apenas partes específicas.

### 4. **Necessidade de Tecnologias Específicas**
- Ambientes que requerem eficiência:
  - Quando é necessário usar diferentes tecnologias para resolver problemas específicos, como machine learning ou processamento em tempo real.
  - Um portfólio tecnológico diverso pode oferecer uma vantagem competitiva.
  - Para negócios pequenos, com baixo risco e orçamento, a separação em micro-serviços pode não ser vantajosa.

## Considerações Finais
- A decisão de adotar micro-serviços ou sistemas monolíticos deve ser feita com base no contexto do projeto.
- Em situações de baixo volume e baixo risco, micro-serviços podem não trazer benefícios significativos.

## Próximos Passos
- No próximo vídeo, serão abordados pontos importantes para começar a trabalhar com micro-serviços e entender suas complexidades.

---

Este guia serve como uma referência para entender quando e por que optar por arquiteturas de micro-serviços em vez de sistemas monolíticos, destacando a importância do contexto e das necessidades do negócio.



---

## modulo_10_11513.mp4

# Resumo da Aula sobre Arquitetura Baseada em Microsserviços

## Introdução ao 12-Factor App
- O 12-Factor App é um conjunto de princípios que orientam o desenvolvimento de aplicações modernas.
- É importante ter em mente esses princípios ao adotar uma arquitetura baseada em microsserviços.

## Arquitetura Baseada em Microsserviços
### Definição
- A arquitetura de microsserviços é uma abordagem onde cada componente de um sistema monolítico é transformado em um serviço independente.
- Essa mudança impacta significativamente a estrutura e o funcionamento da aplicação.

### Comunicação entre Microsserviços
- **Comunicação**: Os microsserviços se comunicam entre si, podendo seguir regras de rede definidas.
- **Latência**: Cada chamada a um microsserviço gera latência, que não ocorre em um monolito.
  - Exemplo: Se cada chamada demora 20 milissegundos e há 5 chamadas encadeadas, a latência total pode chegar a 100 milissegundos.
- **Cuidado**: É fundamental evitar a chamada em cascata (chamadas dominó) para não aumentar a latência.

### Desafios e Considerações
- A arquitetura de microsserviços pode ser mais lenta que a arquitetura monolítica, dependendo de como os serviços são organizados.
- **Motivo para uso**: A adoção de microsserviços deve ter uma justificativa clara; caso contrário, pode resultar em custos mais altos e maior latência.

### Estratégias para Gerenciamento
- Desenvolvedores devem ter estratégias para:
  - Minimizar chamadas entre microsserviços.
  - Compreender a necessidade de dados em tempo real.
- Com o aumento da complexidade, a entrega de dados em tempo real se torna mais rara.

### Banco de Dados em Microsserviços
- Cada microsserviço geralmente possui seu próprio banco de dados.
  - Exemplos de bancos: QValueStore, bancos de dados relacionais.
- **Escolha do banco de dados**: É essencial escolher um banco de dados apropriado para cada microsserviço e entender as tecnologias envolvidas.
- **Liberdade tecnológica**: Os desenvolvedores têm mais liberdade para escolher tecnologias e bancos de dados, podendo usar mais de um banco na mesma aplicação.

### Comunicação Síncrona vs. Assíncrona
- Os microsserviços normalmente se comunicam de forma **síncrona**.
- A comunicação assíncrona altera completamente a dinâmica do sistema e será discutida em vídeos futuros.

## Conclusão
- A arquitetura baseada em microsserviços traz complexidades e desafios que devem ser cuidadosamente gerenciados.
- O entendimento claro dos princípios e das estratégias de implementação é crucial para o sucesso dessa abordagem.

## Próximos Passos
- Nos próximos vídeos, serão abordados os efeitos colaterais da arquitetura de microsserviços e como lidar com eles. 

### Dicas Finais
- Sempre questionar o motivo da adoção dos microsserviços.
- Analisar a latência e a comunicação entre serviços.
- Escolher tecnologias com base em conhecimento e não apenas em tendências.



---

## modulo_10_11514.mp4

# Estudo sobre Arquiteturas Baseadas em Micro-serviços

## Introdução
Neste vídeo, o palestrante discute as condições e necessidades que levam à adoção de arquiteturas baseadas em *micro-serviços* em comparação com sistemas *monolíticos*. Abaixo estão os principais pontos abordados.

## Quando optar por Micro-serviços

### 1. Necessidade de Escala
- A escolha por micro-serviços é indicada quando há:
  - **Alta necessidade de escala**, principalmente em relação a *equipes*.
  - Dificuldades em escalar grandes equipes em sistemas monolíticos.
- **Monolíticos** podem escalar, mas:
  - O gerenciamento de muitos desenvolvedores em um único sistema é complexo.
  - Escalar times em um sistema monolítico é um desafio significativo.

### 2. Definição de Contextos
- Micro-serviços são mais eficazes quando:
  - Há *contextos de unidades de negócio* bem definidos.
  - É possível identificar onde começa e termina uma parte do sistema.
- Contextos definidos ajudam a criar micro-serviços que atendem a necessidades específicas.

### 3. Escalabilidade de Partes Específicas
- Possibilidade de escalar partes do sistema em vez de todo o sistema.
- Exemplo prático:
  - Durante eventos de alta demanda, como *Black Friday*, escalar apenas o catálogo de produtos, sem precisar escalar o sistema inteiro, é uma vantagem.
  - Em grandes plataformas, como Amazon, escalar apenas o que é necessário pode resultar em economia de recursos.

### 4. Necessidade de Tecnologias Específicas
- Ambientes que exigem:
  - Tecnologias variadas para resolver problemas específicos (ex: *machine learning*, processamento em tempo real).
  - Um portfólio maior de tecnologias pode trazer uma vantagem competitiva.
- Em contrapartida:
  - Para sites pequenos ou com baixo volume de acessos, a separação em micro-serviços pode não ser vantajosa.

### 5. Contextualização é Fundamental
- A escolha entre micro-serviços e monolíticos depende do:
  - **Risco** envolvido.
  - **Orçamento** disponível.
  - **Volume** de acessos ou operações.
- Para ambientes com baixo risco e baixo volume, micro-serviços podem não trazer grandes benefícios.

## Conclusão
- O palestrante enfatiza que a decisão de usar micro-serviços deve ser baseada no contexto específico do projeto.
- No próximo vídeo, serão apresentados pontos adicionais para entender como trabalhar com micro-serviços.

## Pontos Finais
- **Importância da Análise Contextual**: Sempre avaliar o cenário antes de decidir pela arquitetura.
- **Preparação para Micro-serviços**: Estar ciente das complexidades e requisitos necessários para implementar micro-serviços de forma eficaz.



---

## modulo_10_11515.mp4

# Estudo sobre Arquiteturas Baseadas em Micro-Serviços

## Introdução
Neste vídeo, discutimos quando optar por arquiteturas baseadas em micro-serviços, contrastando com sistemas monolíticos. A escolha entre essas arquiteturas depende de diversos fatores relacionados à escala, complexidade e contexto do sistema.

## Quando Optar por Micro-Serviços

### 1. Necessidade de Escalabilidade
- **Escala de Times**: A necessidade de micro-serviços surge principalmente quando há uma grande quantidade de desenvolvedores trabalhando em um projeto. 
- **Limitações dos Monolíticos**: Sistemas monolíticos podem escalar, mas a escalabilidade das equipes se torna complexa e inviável.
- **Ambientes Grandes**: Em grandes ambientes com muitos desenvolvedores, micro-serviços se tornam uma necessidade.

### 2. Contextos de Unidades de Negócio
- **Definição de Contextos**: Trabalhar com micro-serviços é mais viável quando há contextos de unidades de negócio bem definidos.
  - Isso permite a criação de micro-serviços que atendem a contextos específicos.
- **Zonas Cinzentas**: Existem áreas onde os contextos podem se sobrepor, mas a definição clara ajuda na organização do trabalho entre os times.

### 3. Escalabilidade de Partes Específicas do Sistema
- **Escala Seletiva**: Micro-serviços permitem escalar partes específicas de um sistema sem a necessidade de escalar o sistema inteiro.
  - Exemplo: Durante eventos de alta demanda, como a Black Friday, é mais eficiente escalar apenas o catálogo de produtos em vez de toda a plataforma.
- **Custo-Benefício**: Em sistemas grandes, escalar partes específicas pode economizar tempo e recursos financeiros.

### 4. Necessidade de Tecnologias Específicas
- **Ambientes Complexos**: Quando um ambiente exige tecnologias específicas para resolver problemas complexos, a arquitetura de micro-serviços se torna vantajosa.
  - Exemplo: Processamento em tempo real ou machine learning.
- **Baixo Risco e Volume**: Para e-commerces com baixo volume de acesso e risco, micro-serviços podem não trazer vantagens significativas.

## Considerações Finais
- **Importância do Contexto**: A adoção de micro-serviços deve sempre considerar o contexto da aplicação e as necessidades do negócio.
- **Próximos Passos**: O próximo vídeo trará provocações sobre pontos importantes para trabalhar com micro-serviços.

## Resumo
- Micro-serviços são recomendados quando:
  - Há uma necessidade significativa de escalabilidade de times.
  - Existem contextos de unidades de negócio bem definidos.
  - É necessário escalar partes específicas do sistema.
  - Tecnologias específicas são requeridas para resolver problemas complexos.
  
- **Cuidado**: A escolha deve ser feita levando em conta o contexto, orçamento e volume de acessos do sistema.



---

## modulo_10_11516.mp4

# Estudo sobre Arquiteturas de Micro-serviços

## Introdução
No vídeo anterior, discutimos quando optar por sistemas monolíticos. Agora, vamos explorar quando é apropriado escolher arquiteturas baseadas em micro-serviços.

## Quando optar por Micro-serviços

### 1. Escalabilidade
- A necessidade de escalabilidade **de equipes**, não apenas de sistemas.
- Sistemas monolíticos podem escalar, mas **gerenciar grandes equipes** em um único sistema é complexo.
- Com muitos desenvolvedores (milhares), o sistema monolítico se torna **inviável**.

### 2. Contextos de Unidades de Negócio
- Micro-serviços são úteis quando você tem **contextos de negócios bem definidos**.
- Conhecer onde começa e termina uma parte do sistema ajuda na definição de micro-serviços.
- Se os contextos não estão claros, pode ser mais complicado trabalhar com micro-serviços.

### 3. Escalonamento de Partes Específicas do Sistema
- Possibilidade de escalar apenas partes específicas de um sistema em vez de todo o sistema.
- Exemplo: durante grandes eventos (como a Black Friday), é mais eficiente escalar apenas o catálogo de produtos.
- Em sistemas com alta demanda, escalar partes específicas pode **economizar custos**.

### 4. Necessidade de Tecnologias Específicas
- Ambientes grandes podem exigir **tecnologias diversificadas** para resolver problemas específicos (ex: machine learning, processamento em tempo real).
- Um portfólio tecnológico amplo oferece uma **vantagem competitiva**.
- Em casos de baixo risco e volume, micro-serviços podem não ser a melhor escolha.

## Considerações Finais
- A decisão de usar micro-serviços deve levar em conta o **contexto**.
- Micro-serviços são mais vantajosos em ambientes grandes e complexos.
- Em contextos menores, a implementação de micro-serviços pode resultar em **custos desnecessários**.

## Próximos Passos
- O próximo vídeo abordará provocações e pontos importantes para começar a trabalhar com micro-serviços.

### Dicas para Estudo
- Reflita sobre as **vantagens e desvantagens** dos micro-serviços em diferentes contextos.
- Considere exemplos práticos de empresas que utilizam micro-serviços versus sistemas monolíticos.
- Prepare-se para discutir os **contextos** em que cada abordagem é mais eficaz.



---

## modulo_10_11517.mp4

# Estudo sobre Microserviços

## Introdução
No vídeo anterior, discutimos as várias tecnologias que podem ser adotadas em arquiteturas de microserviços e os problemas que podem surgir. Este vídeo foca em características essenciais dos microserviços, ressaltando suas vantagens e desvantagens.

## Características dos Microserviços

### 1. Processo de Deploy Menos Arriscado
- **Definição**: Em uma arquitetura de microserviços, o processo de deploy é menos arriscado em comparação a sistemas monolíticos.
- **Cenário**:
  - Se um deploy falha em um sistema com 100 microserviços, apenas um será afetado.
  - Os outros 99 continuarão operando, permitindo que o sistema degrade parcialmente e ainda atenda requisições.
- **Comparação com Monolíticos**:
  - Em sistemas monolíticos, um erro no deploy pode derrubar todo o sistema.

### 2. Complexidade Aumentada
- **Desvantagens**:
  - A implementação de microserviços traz uma complexidade consideravelmente maior.
- **Exemplos de Complexidade**:
  - Se há 10 microserviços, existem 10 processos de setup e 10 pipelines de CI/CD.
  - Cada microserviço pode exigir comunicação entre diferentes sistemas, aumentando a complexidade.

### 3. Necessidade de Equipes Especializadas
- **Vantagem**:
  - Possibilidade de ter equipes especializadas em cada microserviço.
- **Benefícios da Especialização**:
  - Equipes podem se aprofundar em domínios específicos, como a emissão de notas fiscais, aumentando a eficiência.
  - A especialização melhora a performance e a entrega de resultados.
- **Exemplo**:
  - Em uma empresa como a Netflix, o time responsável pelo Digital Rights Management (DRM) se tornará mais competente ao longo do tempo, entendendo melhor tecnologias como Widevine, PlayReady e Fairplay.

## Conclusão
- **Importância do Tema**: Compreender as vantagens e desvantagens dos microserviços é crucial para evitar decisões inconsequentes.
- **Próximos Passos**: No próximo vídeo, abordaremos a questão da escala em sistemas de microserviços, que apresenta pontos importantes a serem considerados.

## Considerações Finais
- Ao trabalhar com microserviços, é vital balancear a complexidade com as vantagens que eles oferecem.
- A especialização das equipes pode trazer um valor significativo para a empresa, melhorando o desempenho em resolver problemas de negócio.

---

Esses pontos são fundamentais para entender a dinâmica de microserviços e devem ser revisados para uma melhor absorção do conteúdo apresentado.



---

## modulo_10_11518.mp4

# Resumo da Aula sobre Microserviços

## Introdução
- Na aula anterior, discutimos as tecnologias de arquitetura de microserviços e seus potenciais problemas.
- Hoje, vamos explorar características importantes dos microserviços.

## Vantagens dos Microserviços

### Processo de Deploy Menos Arriscado
- **Definição**: A capacidade de fazer deploy de microserviços de forma independente.
- **Exemplo**: 
  - Com 100 microserviços, se um deploy falhar, 99 continuam operacionais.
  - Isso permite que o sistema degrade parcialmente, ainda atendendo requisições.
- **Comparação**: 
  - Em um *sistema monolítico*, um erro no deploy torna o sistema inteiro fora do ar.

### Complexidade do Setup
- **Desvantagem**: 
  - Apesar da independência no deploy, a complexidade aumenta significativamente.
- **Fatores a considerar**:
  - Múltiplos processos de setup (10 microserviços = 10 setups).
  - Necessidade de 10 pipelines de CI/CD e sistemas de análise de código.
  - Comunicação entre os microserviços pode ser complexa e exigir mais coordenação.

### Especialização de Equipes
- **Vantagem**:
  - Equipes podem se especializar em microserviços específicos.
- **Benefícios da especialização**:
  - Aumento da eficiência no tratamento de problemas complexos.
  - Exemplos de especializações:
    - Desenvolvimento de sistemas de emissão de nota fiscal.
    - Gestão de servidores de DRM (Digital Rights Management) em plataformas como Netflix.
- **Resultado**: 
  - Melhor solução para problemas de negócio e maior valor agregado à empresa.

## Considerações Finais
- A escolha por microserviços deve ser feita com cautela, considerando a complexidade e a necessidade de especialização.
- No próximo vídeo, abordaremos o tema da escala e suas implicações.

## Pontos Importantes para Estudar
1. **Vantagens dos Microserviços**:
   - Menos arriscado no deploy.
   - Possibilidade de especialização de equipes.
   
2. **Desvantagens**:
   - Complexidade aumentada no setup e manutenção.
   
3. **Importância da Especialização**:
   - Como a especialização pode trazer eficiência e valor.

## Próximos Passos
- Acompanhar a próxima aula sobre escala e suas implicações em microserviços.



---

## modulo_10_11519.mp4

# Resumo das Características dos Microserviços

## Introdução
No vídeo anterior, discutimos as várias tecnologias que podem ser adotadas em arquiteturas de microserviços e os problemas associados a elas. Neste vídeo, vamos explorar características importantes dos microserviços e suas implicações.

## Vantagens dos Microserviços

### 1. Processo de Deploy Menos Arriscado
- **Implantação Independente**: Em um sistema de microserviços, se um deploy falha, apenas o microserviço específico é afetado.
- **Resiliência**: Mesmo que um microserviço tenha problemas, os outros 99 podem continuar funcionando, permitindo que o sistema degrade parcialmente e ainda atenda requisições.
- **Comparação com Sistemas Monolíticos**: Em um sistema monolítico, um erro no deploy pode derrubar todo o sistema, resultando em inatividade total.

### 2. Especialização de Equipes
- **Equipes Focadas**: Com microserviços, é possível ter equipes especializadas em cada serviço, aumentando a eficiência e a qualidade do trabalho.
- **Domínio de Conhecimento**: Equipes que se concentram em problemas específicos (por exemplo, emissão de nota fiscal) se tornam mais proficientes e eficazes com o tempo.
- **Exemplo Prático**: Em empresas como a Netflix, equipes dedicadas ao gerenciamento de direitos digitais (DRM) aprofundam seu conhecimento em tecnologias específicas como Widevine, PlayReady e Fairplay.

## Desvantagens dos Microserviços

### 1. Complexidade Aumentada no Setup
- **Múltiplos Processos de Setup**: Para cada microserviço, há um processo de configuração, pipeline de CI/CD e análise de código, aumentando a carga de trabalho.
- **Comunicação Entre Sistemas**: A necessidade de comunicação entre diversos microserviços pode complicar a arquitetura e o fluxo de trabalho.
- **Desafios Operacionais**: O aumento do número de microserviços requer um gerenciamento mais cuidadoso e estruturado, especialmente em grandes organizações.

## Considerações Finais
- **Decisões Conscientes**: É crucial tomar decisões informadas ao optar por uma arquitetura de microserviços, considerando tanto as vantagens quanto as desvantagens.
- **Organização de Times**: Empresas grandes frequentemente têm times de plataforma para gerenciar a complexidade e garantir uma configuração eficiente.

## Próximos Passos
- No próximo vídeo, discutiremos a **escala** em microserviços e pontos importantes a serem considerados nesse contexto.

---

> **Dica de Estudo**: Para entender melhor esses conceitos, considere explorar casos de uso de empresas que implementaram microserviços, identificando como superaram os desafios e aproveitaram as vantagens mencionadas.



---

## modulo_10_11573.mp4

# Resumo da Arquitetura Baseada em Microsserviços

## Introdução
- O conceito de **12-Factor App** foi introduzido como base para entender o desenvolvimento de aplicações modernas.
- A transição para uma **arquitetura baseada em microsserviços** implica em mudanças significativas na forma como as aplicações são estruturadas e comunicadas.

## Arquitetura Baseada em Microsserviços
- **Definição**: Cada componente que antes fazia parte de um monolito pode agora ser transformado em um microsserviço independente.
- **Comunicação entre Microsserviços**:
  - Os microsserviços se comunicam entre si, podendo estabelecer regras de rede.
  - A comunicação é um ponto crucial a ser considerado durante o desenvolvimento.

### Latência e Performance
- Cada chamada de um microsserviço para outro pode introduzir **latência**.
  - Exemplo: Se cada chamada demora 20 milissegundos, a soma pode resultar em uma resposta total de até 100 milissegundos.
- **Comparativo com Monolitos**:
  - Em arquiteturas monolíticas, a latência é geralmente menor, pois todos os componentes estão integrados.
  - Isso não significa que microsserviços sejam sempre mais lentos, mas a organização e separação dos serviços pode impactar a performance.

### Justificativa para Uso de Microsserviços
- **Motivações**: Às vezes, a escolha por microsserviços não é justificada, levando a:
  - Aumento de custos
  - Maior latência nas respostas
- É essencial ter uma estratégia clara para quando e por que usar microsserviços.

## Estratégias de Implementação
- **Gerenciamento de Chamadas**:
  - Evitar o que foi chamado de "chamada dominó", onde um microsserviço chama outro, em uma cadeia que aumenta a latência.
- **Tempo Real vs. Dados Quentes**:
  - Avaliar quando é necessário disponibilizar dados em tempo real, considerando a complexidade do sistema.

### Banco de Dados e Tecnologia
- Cada microsserviço geralmente possui seu **próprio banco de dados**.
- A escolha do banco de dados deve ser feita com base no contexto e na necessidade, não apenas por ser uma tendência.
  - **Liberdade de Tecnologia**: É permitido usar múltiplos tipos de bancos de dados em uma única aplicação, conforme a necessidade.

## Comunicação Síncrona vs. Assíncrona
- A comunicação direta entre microsserviços é normalmente **síncrona**.
- A transição para uma abordagem **assíncrona** pode mudar significativamente a dinâmica de interação entre os serviços.

## Conclusão
- Compreender as complexidades e os efeitos colaterais da arquitetura baseada em microsserviços é fundamental para o sucesso do desenvolvimento.
- A discussão sobre esses pontos será aprofundada em vídeos futuros. 

---

### Dicas de Estudo
- **Revisar os conceitos de 12-Factor App** e como se relacionam com microsserviços.
- **Praticar** a identificação de casos em que a arquitetura de microsserviços é preferível.
- **Analisar** as vantagens e desvantagens de implementar uma arquitetura baseada em microsserviços em projetos reais.



---

## modulo_10_11574.mp4

# Resumo da Arquitetura Baseada em Microsserviços

## Introdução ao 12-Factor App
- O 12-Factor App é um conjunto de princípios para construção de aplicações que facilitam a escalabilidade, a manutenção e o desenvolvimento.
- Importante considerar esses princípios ao se trabalhar com microsserviços.

## Arquitetura Baseada em Microsserviços
- A arquitetura de microsserviços representa uma mudança significativa em relação ao modelo monolítico.

### Características Principais
- **Desagregação dos Componentes**: Cada componente de um monolito pode se tornar um microsserviço independente.
- **Comunicação entre Microsserviços**: 
  - Os microsserviços se comunicam entre si.
  - A comunicação pode ser controlada por regras de rede.

### Latência na Comunicação
- Cada chamada entre microsserviços pode resultar em latência:
  - Exemplo: Se cada chamada leva 20 milissegundos, 5 microsserviços em cascata podem resultar em até 100 milissegundos para retornar uma resposta ao usuário.
- **Importante**: A arquitetura de microsserviços não é inerentemente mais lenta que a monolítica, mas a forma como os serviços são organizados pode impactar a performance.

### Custos e Latência
- **Cuidado**: Adotar microsserviços sem uma justificativa clara pode aumentar os custos e a latência.
- A entrega de dados pode ser mais lenta do que em uma arquitetura monolítica, especialmente se não houver planejamento adequado.

## Estratégias para Microsserviços
- É necessário ter estratégias para:
  - **Evitar chamadas em cascata** (chamada dominó).
  - **Determinar a necessidade de dados em tempo real**, visto que sistemas maiores raramente requerem dados instantâneos.

### Banco de Dados em Microsserviços
- Cada microsserviço geralmente possui seu próprio banco de dados.
- **Liberdade de Escolha**: É possível utilizar diferentes tipos de bancos de dados conforme a necessidade de cada microsserviço (ex: QValueStore, bancos de dados relacionais).
- **Cuidado na Escolha**: Não escolher um banco de dados apenas porque está na moda; deve-se entender bem a tecnologia para fazer uma escolha adequada.

## Comunicação Síncrona vs. Assíncrona
- **Comunicação Síncrona**: Um microsserviço chama diretamente outro de forma síncrona.
- **Comunicação Assíncrona**: A abordagem assíncrona muda completamente a dinâmica e será explorada em vídeos futuros.

## Conclusão
- A arquitetura baseada em microsserviços oferece flexibilidade e escalabilidade, mas traz complexidades que devem ser cuidadosamente gerenciadas.
- Nos próximos conteúdos, serão abordados efeitos colaterais e melhores práticas ao trabalhar com microsserviços. 

### Próximos Passos
- Fique atento aos próximos vídeos que irão aprofundar os conceitos apresentados.



---

## modulo_10_11575.mp4

# Notas de Estudo sobre Arquitetura Baseada em Microsserviços

## Introdução ao 12-Factor App
- O 12-Factor App é um conjunto de práticas recomendadas para construir aplicações que são:
  - Escaláveis
  - Manuteníveis
  - Portáveis

## Arquitetura Baseada em Microsserviços

### Definição
- A arquitetura baseada em microsserviços é uma abordagem que:
  - Divide uma aplicação em múltiplos serviços menores e independentes.
  - Cada componente que estava em um monolito se torna um *serviço*.

### Comunicação entre Microsserviços
- Os microsserviços precisam se comunicar entre si.
  - *Comunicação direta* entre serviços é comum.
  - Pode haver regras de rede para limitar a comunicação entre certos microsserviços.
- **Latência**:
  - Cada chamada entre microsserviços tem uma latência associada.
  - Exemplo: Se cada chamada leva 20 milissegundos, uma sequência de chamadas pode resultar em um tempo total de 100 milissegundos.

### Comparação com Monolitos
- A arquitetura de microsserviços não é necessariamente mais lenta que a arquitetura monolítica.
  - Dependendo da organização e separação dos microsserviços, a latência pode aumentar.
- **Cuidado**: Usar microsserviços sem justificativa pode resultar em:
  - Custos elevados
  - Aumento da latência na entrega de dados

### Estruturas e Estratégias
- É importante ter estratégias para:
  - Evitar chamadas em cadeia (chamada dominó).
  - Determinar quando é necessário disponibilizar dados em tempo real.
- Em sistemas grandes, raramente os dados precisam ser entregues instantaneamente.

### Banco de Dados
- Cada microsserviço, normalmente, tem seu próprio banco de dados.
  - Permite o uso de diferentes tipos de bancos de dados conforme a necessidade.
  - Exemplo: Um microsserviço pode usar um *QValueStore*, enquanto outro pode usar um banco de dados relacional.
- **Escolha do Banco de Dados**:
  - Não escolha um banco de dados apenas por estar na moda ou ser "cool".
  - É essencial entender as características e requisitos do banco de dados para fazer uma escolha informada.

### Síncrono vs Assíncrono
- A comunicação entre microsserviços é frequentemente *síncrona*.
  - Em breve, será abordada a diferença entre comunicação síncrona e assíncrona, que altera a dinâmica da arquitetura.

## Conclusão
- A arquitetura baseada em microsserviços traz complexidades e desafios que devem ser cuidadosamente geridos.
- Nos próximos vídeos, serão explorados os efeitos colaterais dessa arquitetura e como trabalhar com eles de maneira eficiente.

### Próximos Passos
- Acompanhar os próximos conteúdos para aprofundar conhecimentos sobre:
  - Efeitos colaterais da arquitetura baseada em microsserviços.
  - Estratégias para otimização e eficiência na comunicação entre serviços.



---

## modulo_10_11576.mp4

# Resumo da Palestra sobre API Gateway e Micro-serviços

## Introdução
- O tema central é o uso de **API Gateway** em uma arquitetura de **micro-serviços** dentro de uma rede maior.
- A importância da utilização de API Gateway para facilitar a comunicação entre micro-serviços.

## Comunicação entre Micro-serviços
- **Não necessidade de conhecimento** sobre os micro-serviços utilizados:
  - As equipes podem comunicar-se através do API Gateway sem saber qual micro-serviço específico está sendo chamado.
  - Utilização de um **endpoint** fixo, que pode ser mantido mesmo com mudanças nos micro-serviços.

## Vantagens do API Gateway
- **Transparência para os usuários**:
  - Mudanças no micro-serviço (como troca de programação ou endpoint) não impactam os consumidores.
- **Flexibilidade**:
  - Possibilidade de refatorar, reconstruir ou trocar a linguagem de programação sem alterar o endpoint.
  
### Exemplo Prático
- Um micro-serviço que emite uma ordem de cobrança:
  - Ele chama um endpoint como `/bill` sem saber qual micro-serviço está por trás dele.
  - Mudanças nesse micro-serviço não afetam a chamada, pois continua utilizando o mesmo endpoint.

## Recursos do API Gateway
- **Recursos adicionais** que podem ser configurados:
  - Políticas de **retry**.
  - Configurações de **segurança**.
  - **Rate limiting**.
- O API Gateway gerencia esses aspectos, permitindo que os micro-serviços se concentrem em suas funções principais.

## Importância do Stateless
- **API Gateway deve ser stateless**:
  - Isso permite que o gateway seja reiniciado a qualquer momento, sem perda de funcionalidade.
  - Facilita a criação de novos contextos, bastando subir uma nova API Gateway.
  
### Exemplos de API Gateways OpenSource
- **Kong**: Permite operação stateless.
- **CrackND**: Outra solução que pode ser utilizada.
- Importância de evitar dependências de bancos de dados para melhor desempenho.

## Preparação da Equipe
- **Criação de uma Network Policy**:
  - Proibir chamadas diretas entre micro-serviços de contextos diferentes.
  - Prevenir que desenvolvedores façam chamadas diretas, garantindo a integridade da arquitetura.

## Conclusão
- A implementação de uma topologia utilizando API Gateway é uma mudança significativa na arquitetura de micro-serviços.
- A comunicação eficiente e o gerenciamento centralizado através do API Gateway podem otimizar o desenvolvimento e a manutenção de sistemas. 

## Considerações Finais
- A estratégia de utilizar uma API Gateway deve ser bem definida e implementada para garantir o sucesso na arquitetura de micro-serviços.
- Reforçar a necessidade de treinar a equipe para seguir as diretrizes estabelecidas.

**Agradecimentos e Encerramento**
- Agradecimento ao público e convite para o próximo vídeo.



---

## modulo_10_11577.mp4

# Resumo da Aula sobre API Gateway e Micro-serviços

## Introdução
No vídeo anterior, discutimos sobre a implementação de um *API Gateway* na frente de um conjunto de micro-serviços dentro de uma rede. Este conceito é fundamental para a comunicação eficiente entre diferentes serviços.

## Estrutura da Rede
- O *API Gateway* atua como um ponto de entrada para os micro-serviços.
- Os micro-serviços estão inseridos em uma rede maior, facilitando a comunicação e a integração entre eles.

## Vantagens do API Gateway
1. **Abstração de Micro-serviços**: 
   - As equipes que desenvolvem os micro-serviços não precisam saber quais serviços específicos estão sendo chamados.
   - A comunicação é feita através de um único endpoint.

2. **Flexibilidade**:
   - Mudanças em um micro-serviço (como reescrever em uma nova linguagem ou reformular) não afetam o endpoint utilizado pelos consumidores.
   - O endpoint permanece o mesmo, garantindo uma integração transparente.

3. **Exemplo Prático**:
   - Um micro-serviço que emite ordens de cobrança (ex: `/bill`) pode ser alterado sem que outros serviços saibam das mudanças internas.

4. **Recursos Adicionais**:
   - O *API Gateway* pode implementar:
     - Políticas de *retry*.
     - Segurança (auth, rate limiting).
   - Esses recursos são configurados no *API Gateway*, aliviando os micro-serviços dessas preocupações.

## Importância da Statelessness
- **Definição de Stateless**: O *API Gateway* deve ser projetado para não manter estado entre as requisições.
- **Benefícios**:
  - Permite que a API Gateway seja reiniciada a qualquer momento sem perda de funcionalidade.
  - Facilita a criação de novos contextos com novas instâncias do *API Gateway*.
- **Exemplos de API Gateways Open Source**:
  - Kong
  - KrakenD

## Práticas Recomendadas
- **Evitar Chamadas Diretas**:
  - É essencial preparar a equipe para não realizar chamadas diretas entre micro-serviços de contextos diferentes.
  - Implementar uma *Network Policy* para restringir essas chamadas diretas.
  
- **Configuração Declarativa**:
  - Trabalhar com configurações declarativas para facilitar a implementação e a manutenção do *API Gateway*.

## Conclusão
- A adoção de um *API Gateway* transforma a arquitetura baseada em micro-serviços, proporcionando maior controle e flexibilidade.
- É crucial evitar chamadas diretas entre micro-serviços para preservar a integridade da estratégia de *API Gateway*.

---

## Dicas Finais
- Sempre **mantenha o *API Gateway* stateless** para garantir escalabilidade e manutenção fácil.
- Crie **políticas de rede** para evitar que desenvolvedores eludam a arquitetura planejada.
- Considere o uso de ferramentas como Kong e KrakenD para implementar soluções eficazes.

Um grande abraço e até o próximo vídeo!



---

## modulo_10_11578.mp4

# Resumo da Aula sobre API Gateway e Microserviços

## Introdução
- Discussão sobre o uso de **API Gateway** em uma rede de micro-serviços.
- Importância de entender como esse sistema se integra em uma rede maior.

## Vantagens do Uso de API Gateway

### Comunicação entre Micro-serviços
- **Times de desenvolvimento** não precisam saber com qual micro-serviço estão se comunicando.
- A comunicação é feita através de um **endpoint único** na API Gateway.
- Mudanças em micro-serviços (linguagem de programação, lógica interna, etc.) são feitas de forma transparente para os usuários.

### Exemplos Práticos
- Um micro-serviço que emite uma ordem de cobrança acessa um endpoint específico (`/bill`).
- Se o sistema mudar, o endpoint permanece o mesmo, evitando que outros serviços precisem ser atualizados.

### Recursos e Benefícios
- API Gateway oferece:
  - Políticas de **retry**.
  - Segurança adicional.
  - **Rate limiting**.
- Redução da complexidade ao centralizar chamadas na API Gateway.

## Importância da Arquitetura Stateless

### O que significa Stateless?
- API Gateways devem ser **stateless** para facilitar escalabilidade e manutenção.
- Permite reiniciar a API Gateway sem impactos significativos, facilitando a criação de novos contextos.

### Exemplos de API Gateways Open Source
- **Kong**: Permite operar de forma stateless.
- **Crack ND**: Outra opção viável.

## Implementação e Considerações

### Políticas de Rede
- Implementar uma **Network Policy** para proibir chamadas diretas entre micro-serviços de diferentes contextos.
- Evitar que desenvolvedores façam chamadas diretas que possam comprometer a estratégia de uso da API Gateway.

## Conclusão
- A utilização de API Gateways transforma significativamente a arquitetura de micro-serviços.
- Mantém a estrutura organizada e facilita a manutenção e escalabilidade.

## Dicas Finais
- **Prepare sua equipe**: Eduque os times sobre a importância da comunicação via API Gateway.
- **Evite chamadas diretas**: Implemente políticas que restrinjam esse tipo de interação.

### Agradecimentos
- Agradecimento ao público e convite para o próximo vídeo.



---

## modulo_10_11579.mp4

# Resumo da Aula sobre API Gateway e Micro-serviços

Nesta aula, o palestrante discutiu a importância e os benefícios do uso de *API Gateway* frente a um conjunto de *micro-serviços* em uma rede. A seguir, estão os principais pontos abordados.

## Introdução ao API Gateway

- O API Gateway atua como um ponto de entrada para os micro-serviços dentro de uma rede maior.
- As equipes que desenvolvem micro-serviços não precisam saber com qual micro-serviço estão se comunicando.

## Vantagens do Uso do API Gateway

1. **Transparência para os Usuários**
   - Os desenvolvedores podem mudar, refazer ou trocar a linguagem de programação dos micro-serviços sem alterar o endpoint.
   - O endpoint permanece o mesmo para quem utiliza o micro-serviço, proporcionando uma camada de abstração.

2. **Facilidade de Comunicação**
   - Um micro-serviço pode, por exemplo, emitir uma ordem de cobrança chamando um endpoint específico (ex: `/cobrança`).
   - Mudanças na implementação do micro-serviço não afetam a chamada ao endpoint.

3. **Recursos e Funcionalidades**
   - O API Gateway pode gerenciar:
     - **Políticas de Retry**: Tentativas de reenvio em caso de falhas.
     - **Segurança**: Implementação de autenticação e autorização.
     - **Rate Limiting**: Controle do número de requisições em um determinado intervalo de tempo.

## Práticas Recomendadas

- **API Gateway Stateless**
  - É recomendado que as APIs Gateways sejam *stateless* (sem estado).
  - Vantagens:
    - Facilidade para reiniciar e escalar a API Gateway.
    - Redução de dependências com banco de dados, melhorando a performance.
  
- **Exemplos de API Gateways OpenSource**
  - **Kong**: Boa opção para implementar API Gateway stateless.
  - **CrackND**: Outra solução para trabalhar com APIs Gateways.

## Políticas de Rede

- **Evitar Chamadas Diretas**
  - É essencial criar uma *Network Policy* que proíba chamadas diretas entre micro-serviços de contextos diferentes.
  - Isso garante a integridade da arquitetura baseada em API Gateway e evita que desenvolvedores façam chamadas diretas que poderiam comprometer a estratégia.

## Conclusão

- O uso de API Gateways e a estruturação correta das comunicações entre micro-serviços representam uma mudança significativa na forma como as aplicações são desenvolvidas e mantidas.
- Implementar as recomendações discutidas pode levar a uma arquitetura mais robusta, escalável e fácil de gerenciar.

## Agradecimentos

- O palestrante finaliza com um agradecimento e convite para o próximo vídeo.

---

**Dicas para Estudo:**
- Revise os conceitos de *micro-serviços* e *API Gateway*.
- Pratique a configuração de um API Gateway usando um dos exemplos mencionados.
- Explore a implementação de *Network Policies* para reforçar a segurança e a integridade da comunicação entre micro-serviços.



---

## modulo_10_11580.mp4

# Estudo sobre Autenticação com JWT

## Introdução
No vídeo anterior, discutimos sobre autenticação e o funcionamento do servidor de autenticação na geração de tokens JWT (JSON Web Token). Neste estudo, abordaremos os problemas relacionados à expiração de tokens e como isso impacta a segurança da aplicação.

## Funcionamento do JWT
- O servidor de autenticação gera um *JWT*.
- A API Gateway valida o *JWT* utilizando uma chave pública.
- Se o token é validado, as requisições são encaminhadas para os microserviços.

## Problema da Expiração do Token
### Cenário
- O servidor de identidade gera um token com um tempo de expiração (exemplo: 1 hora).
- O token é utilizado durante um minuto, mas o login do usuário é invalidado nesse período.

### Consequências
- A API Gateway não verifica constantemente o servidor de autenticação.
- Mesmo que o login seja cancelado, o usuário ainda poderá acessar a aplicação até que o token expire.

## Estratégias de Verificação
- **Redução do Tempo de Expiração**: Diminuir o tempo de expiração do token para aumentar a segurança.
  - Exemplo: Alterar a expiração de 1 hora para 5 minutos.
  - Após 5 minutos, o token se tornará inválido e o usuário precisará de um *refresh token*.

### Refresh Token
- O *refresh token* permite que o usuário solicite um novo token após a expiração.
- O usuário deve fazer uma nova solicitação ao serviço de autenticação.

## Considerações sobre Expiração de Tokens
1. **Maior Tempo de Expiração**:
   - **Vantagens**:
     - Menor carga no servidor de autenticação.
   - **Desvantagens**:
     - Maior risco de acesso não autorizado durante a validade do token.
  
2. **Menor Tempo de Expiração**:
   - **Vantagens**:
     - Maior controle sobre o acesso do usuário.
   - **Desvantagens**:
     - Aumento da carga no servidor de autenticação devido a mais solicitações para novos tokens.

## Conclusão
- A escolha do tempo de expiração do token e a utilização de *refresh tokens* são fundamentais para equilibrar segurança e performance da aplicação.
- É necessário avaliar as necessidades específicas da aplicação para escolher a estratégia mais adequada.

## Próximos Passos
- No próximo vídeo, discutiremos mais sobre a validação de tokens e outras considerações relacionadas à segurança na autenticação.



---

## modulo_10_11581.mp4

# Resumo da Aula: Autenticação e Validação de Tokens JWT

## Introdução
Na aula anterior, discutimos *autenticação* e o papel do *servidor de autenticação* na geração de *JSON Web Tokens (JWT)*. A API Gateway é responsável por validar esses tokens para permitir o acesso aos *microserviços*.

## Validação do JWT
- A API Gateway valida o JWT usando uma **chave pública**.
- Se o token é validado com sucesso, as requisições são enviadas para os microserviços.

## Problema da Expiração do Token
- O servidor de autenticação gera um token com um tempo de expiração (ex: 1 hora).
- Se o usuário precisar ser *invalidado* após gerar o token:
  - Durante a validade do token, a API Gateway continuará validando e permitindo o acesso do usuário.

### Consequências
- **Problema Principal**: O usuário pode acessar o sistema mesmo após ter sua autenticação cancelada, até que o token expire.
- Isso levanta a necessidade de estratégias de verificação para a expiração dos tokens.

## Estratégias de Expiração
1. **Redução do Tempo de Expiração**:
   - Exemplo: reduzir a expiração de 1 hora para 5 minutos.
   - Durante esses 5 minutos, mesmo que a autenticação seja cancelada, o usuário ainda terá acesso.
   - Após 5 minutos, o token se torna inválido.
   
2. **Uso de Refresh Tokens**:
   - Após a expiração do token, o usuário deve solicitar um novo token (refresh token) para continuar acessando a aplicação.
   - Isso requer que o usuário faça uma nova autenticação no servidor.

## Considerações Finais
- **Carga no Servidor**:
  - Quanto maior o tempo de expiração do token, menor a carga no servidor de autenticação.
  - Quanto menor o tempo de expiração, maior a carga no servidor, mas melhor controle sobre o acesso.

## Conclusão
- É crucial equilibrar o tempo de expiração dos tokens para garantir segurança e eficiência no uso do servidor de autenticação.
- O próximo vídeo abordará outros casos relacionados à validação de tokens.

## Próximos Passos
- Estudar os diferentes casos de validação de tokens que serão discutidos na próxima aula.



---

## modulo_10_11596.mp4

# Resumo da Aula sobre Tracing e Correlation ID

## Introdução
- A aula aborda a importância do *tracing* para identificar problemas em micro-serviços.
- O *tracing* é um dos três pilares da *observabilidade*, que inclui também *logs* e *métricas*.

## Pilar da Observabilidade
1. **Logs**
   - Registra o que aconteceu no sistema.
2. **Métricas**
   - Mostra o estado atual do sistema, como:
     - Número de acessos
     - Requisições
     - Uso de CPU
     - Compras
3. **Tracing**
   - Rastreia uma requisição de ponta a ponta, permitindo identificar problemas.

## O que é Correlation ID?
- O *Correlation ID* é um identificador único que permite rastrear requisições entre diferentes micro-serviços.
- Cada requisição recebe um ID, que é passado adiante em cada chamada subsequente.

### Importância do Correlation ID
- Facilita a identificação de problemas em uma sequência de requisições.
- Permite a correlação de dados entre micro-serviços.

## Implementação do Correlation ID
1. **Geração do Correlation ID**
   - Se não houver um *Correlation ID* ao receber uma requisição, gera-se um novo.
   
2. **Envio do Correlation ID**
   - Ao enviar uma requisição para outro micro-serviço, o *Correlation ID* deve ser incluído.
   - O micro-serviço receptor deve verificar e enviar o mesmo *Correlation ID* em suas requisições subsequentes.

3. **Requisição Intencional**
   - A implementação do *Correlation ID* deve ser feita de forma intencional:
     - Extração do ID de cada requisição.
     - Reenvio do ID em cada nova requisição.

## Ferramentas e Bibliotecas
- Existem diversas bibliotecas e técnicas para facilitar a implementação do *Correlation ID*.
- É comum criar *middleware* para evitar repetição de código.

## Próxima Aula
- O próximo vídeo abordará o Open Telemetry (OTEL), uma ferramenta que auxilia na implementação de *tracing* e *Correlation ID*.

## Conclusão
- A prática de identificação e rastreamento de requisições em micro-serviços é crucial para a manutenção e solução de problemas em sistemas complexos. A implementação de *Correlation ID* é um passo fundamental nesse processo.



---

## modulo_10_11597.mp4

# Estudo sobre Observabilidade e Tracing em Micro-serviços

## Introdução
No vídeo anterior, foi discutido um problema comum relacionado à dificuldade de identificar problemas em micro-serviços quando não se tem acesso claro às informações. Uma solução importante para minimizar esses problemas é o uso de *Tracing*.

## Observabilidade
A *observabilidade* é uma prática composta por três pilares fundamentais:
1. **Logs**: Capturam o que aconteceu no sistema.
2. **Métricas**: Mostram o estado atual do sistema, como:
   - Número de acessos
   - Quantidade de requisições
   - Uso de CPU
   - Vendas e outras estatísticas relevantes
3. **Tracing**: Rastreia o que acontece de forma end-to-end em uma requisição.

## O que é Tracing?
- O *Tracing* permite rastrear requisições que se estendem por diversos micro-serviços.
- Cada requisição recebe um **ID**, conhecido como *Correlation ID*, que é usado para identificar e correlacionar as requisições entre os serviços.

## Correlation ID
- **Definição**: É um identificador único associado a uma requisição que permite rastrear o seu caminho através de múltiplos micro-serviços.
- **Importância**:
  - Facilita o rastreamento de requisições em caso de problemas.
  - Permite a identificação de quais micro-serviços foram atingidos por uma requisição específica.

### Implementação do Correlation ID
1. **Geração**: Ao receber a primeira requisição sem um Correlation ID, deve-se gerar um novo ID.
2. **Transmissão**: Este Correlation ID deve ser enviado em todas as requisições subsequentes para outros micro-serviços.
3. **Verificação**: Cada micro-serviço que recebe uma requisição deve verificar se há um Correlation ID. Se sim, deve reencaminhá-lo nas requisições que realizar.
4. **Extração e Reenvio**: O Correlation ID deve ser extraído de cada requisição e enviado intencionalmente.

## Ferramentas e Bibliotecas
- Existem várias bibliotecas e técnicas para facilitar a implementação do Correlation ID.
- É comum criar *middleware* para evitar a repetição de código na aplicação.

## Próximos Passos
- No próximo vídeo, será abordado o *Open Telemetry* (OTEL), um projeto que ajuda na implementação do *Tracing* e do *Correlation ID*.

## Conclusão
A implementação do *Tracing* e do *Correlation ID* é crucial para a observabilidade em sistemas de micro-serviços, permitindo um rastreamento eficaz e uma resolução de problemas mais ágil.



---

## modulo_10_11598.mp4

# Estudo sobre Autenticação e JWT

## Introdução
No vídeo anterior, discutimos o processo de autenticação utilizando JWT (JSON Web Tokens) e como a API Gateway valida esses tokens antes de encaminhar as requisições para os microserviços.

## Validação de JWT pela API Gateway
- A API Gateway valida o JWT utilizando uma **chave pública**.
- Se o token for validado, isso indica que ele foi gerado pelo servidor de identidade.

## Problema da Expiração do Token
- **Expiração do Token**: O servidor de identidade gera um token com um período de validade.
  - Exemplo: Token com expiração de **1 hora**.
- **Consequência da Expiração**:
  - Se um usuário for desconectado (login cancelado) durante a validade do token, a API Gateway continuará a aceitá-lo por até uma hora.

### Cenário de Problemas
1. Token gerado com expiração de 1 hora.
2. O usuário é desconectado após 1 minuto.
3. A API Gateway ainda aceita o token por mais 59 minutos.
4. **Problema**: Acesso não autorizado ao sistema, mesmo após o cancelamento do login.

## Estratégias de Verificação do Tempo de Expiração
- É necessário definir **estratégias de expiração** para os tokens de forma a balancear segurança e carga no servidor.
  - **Exemplo de Estratégia**:
    - Reduzir a expiração para **5 minutos**.
      - Isso significa que o usuário terá acesso por 5 minutos, mesmo que o login seja cancelado.
      - Após 5 minutos, o token se torna inválido e o usuário deve solicitar um **refresh token**.

### Refresh Token
- O refresh token permite que o usuário obtenha um novo token após a expiração do anterior.
- O usuário deve **interagir com o servidor de autenticação** para obter um novo token.

## Considerações Finais
- **Trade-off** entre tempo de expiração e carga no servidor:
  - **Maior tempo de expiração**:
    - Menor carga no servidor de autenticação.
    - Maior risco de acesso não autorizado.
  - **Menor tempo de expiração**:
    - Maior controle sobre o acesso.
    - Maior carga no servidor de autenticação.

## Próximos Passos
- O próximo vídeo abordará casos adicionais relacionados à validação dos tokens e estratégias mais avançadas.

## Dicas para Estudo
- Reforce os conceitos de **JWT** e **refresh tokens**.
- Pratique cenários onde a expiração do token impacta a segurança da aplicação.
- Estude a implementação de verificações de autenticação em sistemas de microserviços.



---

## modulo_10_11599.mp4

# Resumo da Aula sobre Autenticação e JWT

## Introdução
- Na aula anterior, discutimos sobre **autenticação** e o papel do **servidor de autenticação** na geração de **JWT (JSON Web Token)**.
- A **API Gateway** é responsável por validar o JWT antes de encaminhar as requisições para os microserviços.

## Funcionamento do JWT
- O servidor de autenticação gera um JWT que contém:
  - Uma **chave pública** para validação.
  - Um tempo de **expiração** do token.

## Problemas Relacionados à Expiração do Token
- Se um token é gerado com um tempo de expiração (exemplo: 1 hora):
  - Durante o período de validade, mesmo que o acesso do usuário seja **invalidado**, a API Gateway ainda permitirá o acesso.
  - Isso acontece porque a API Gateway não verifica constantemente o servidor de autenticação.

### Exemplificação do Problema
1. **Geração do Token**:
   - Token válido por 1 hora.
2. **Uso do Token**:
   - O usuário utiliza o token por 1 minuto.
3. **Invalidação do Acesso**:
   - Após 1 minuto, o acesso do usuário é cancelado, mas ainda pode acessar por mais 59 minutos.

## Estratégias de Verificação
- Para mitigar o problema de invalidação, é importante considerar o **tempo de expiração** do token:
  - **Exemplo**: Reduzindo o tempo de expiração para **5 minutos**.
    - O usuário terá acesso por até 5 minutos, mesmo que o login seja cancelado.
    - Após 5 minutos, o token se torna inválido, e o usuário deve solicitar um **refresh token**.

### Refresh Token
- O **refresh token** permite que o usuário solicite um novo token após a expiração do anterior.
- É necessário que o usuário faça uma nova solicitação ao servidor de autenticação para obter um novo token.

## Considerações Finais
- **Relação entre Tempo de Expiração e Carga no Servidor**:
  - **Maior Tempo de Expiração**:
    - Menor controle sobre o acesso do usuário.
    - Menor carga no servidor de autenticação.
  - **Menor Tempo de Expiração**:
    - Maior controle sobre o acesso do usuário.
    - Maior carga no servidor de autenticação.

- É essencial equilibrar o tempo de expiração dos tokens com a carga no servidor e o controle de acesso.

## Próximos Passos
- Na próxima aula, discutiremos mais sobre **validação** e outros casos relacionados a este tema.



---

## modulo_10_11600.mp4

# Resumo da Aula sobre Observabilidade e Tracing

## Introdução
No vídeo anterior, discutiu-se a importância de ter um acesso claro para identificar problemas em micro-serviços. Uma das maneiras de facilitar essa identificação é através do **Tracing**.

## Observabilidade
- **Observabilidade** é uma prática que possui três pilares fundamentais:
  1. **Logs**: Registra o que aconteceu no sistema.
  2. **Métricas**: Mostra o que está acontecendo no sistema em um dado momento (exemplo: número de acessos, requisições, uso de CPU, etc.).
  3. **Tracing**: Permite rastrear a trajetória de uma requisição de ponta a ponta.

### O que é Tracing?
- O **Tracing** é essencial para entender o fluxo de uma requisição através de vários micro-serviços.
- Para implementar o tracing, cada requisição recebe um **ID** específico.

## Correlation ID
- O **Correlation ID** é um identificador único que permite rastrear requisições entre os micro-serviços.
- Importância do Correlation ID:
  - Facilita a identificação de problemas.
  - Permite que, ao saber o ID de uma requisição, possamos rastreá-la em diferentes micro-serviços.

### Como Implementar o Correlation ID
1. **Identificação da Requisição**:
   - Sempre que uma nova requisição for recebida, deve-se verificar se já existe um Correlation ID.
   - Se não existir, um novo Correlation ID deve ser gerado.
   
2. **Envio do Correlation ID**:
   - Ao enviar uma requisição para outro micro-serviço, o Correlation ID deve ser incluído.
   - O micro-serviço receptor deve verificar se recebeu o Correlation ID e, se sim, enviá-lo nas próximas requisições.

### Importância da Implementação Intencional
- A implementação do Correlation ID deve ser feita de forma **intencional**:
  - Extração e reenvio do Correlation ID são essenciais para o rastreamento eficaz das requisições.
  
## Ferramentas e Bibliotecas
- Existem várias bibliotecas e técnicas disponíveis para facilitar a implementação do Correlation ID.
- Recomenda-se a criação de **middleware** para evitar a repetição de código.

## Próximos Passos
- No próximo vídeo, o foco será em **OTEL (Open Telemetry)**, uma ferramenta que ajuda na implementação do tracing e na gestão dos Correlation IDs.

## Conclusão
A implementação do **Tracing** e do **Correlation ID** são passos cruciais para garantir a observabilidade em sistemas de micro-serviços, permitindo assim uma identificação mais ágil e eficaz de problemas.



---

## modulo_10_11601.mp4

# Resumo da Palestra sobre Observabilidade e Tracing

## Introdução
- Importância da *observabilidade* em micro-serviços.
- Necessidade de identificar problemas de forma clara e acessível.

## Os Três Pilares da Observabilidade
1. **Logs**
   - Captura de eventos que ocorreram no sistema.
2. **Métricas**
   - Informações em tempo real sobre o sistema, como:
     - Número de acessos.
     - Número de requisições.
     - Uso de CPU.
     - Transações (ex: compras).
3. **Tracing**
   - Rastreamento de requisições de ponta a ponta.
   - Permite entender como uma requisição se estende entre diferentes micro-serviços.

## Correlation ID
- O que é?
  - Um *ID* único atribuído a cada requisição.
  - Facilita a correlação entre diferentes micro-serviços.
  
- **Como funciona?**
  - Quando um usuário envia uma requisição, um ID é gerado.
  - Esse ID é transmitido entre os micro-serviços.
  - Exemplo:
    - Requisição 1: ID = 1
    - Requisição 2: ID = 1
    - Requisição 3: ID = 1
  - Com o *Correlation ID*, é mais fácil rastrear onde ocorreu um problema.

## Implementação do Correlation ID
- **Passos para Implementação:**
  1. **Verificação do Correlation ID:**
     - Se a requisição não possui um Correlation ID, um novo deve ser gerado.
  2. **Transmissão do Correlation ID:**
     - Ao enviar uma requisição para outro micro-serviço, incluir o Correlation ID.
  3. **Extração e Reenvio:**
     - O micro-serviço receptor deve extrair o Correlation ID e reenviá-lo em suas requisições subsequentes.

- **Importância da Implementação Intencional:**
  - A extração e o envio do Correlation ID devem ser feitos de forma intencional e consistente.
  - Evitar problemas de rastreamento.

## Ferramentas e Bibliotecas
- Existem várias bibliotecas e técnicas disponíveis para implementar o Correlation ID.
- Sugestão de uso de *middleware* para evitar repetição de código.

## Próximo Tópico
- No próximo vídeo, será discutido o *Open Telemetry (OTEL)*, uma ferramenta que auxilia na implementação de tracing e observabilidade.

## Conclusão
- O uso do Correlation ID é crucial para melhorar a capacidade de identificar e resolver problemas em sistemas de micro-serviços.
- Implementação sistemática e intencional do Correlation ID é fundamental para o sucesso na observabilidade.



---

## modulo_10_11602.mp4

# Estudo sobre Microserviços e Tracing

## Introdução
Neste vídeo, o apresentador fala sobre o desempenho dos microserviços e como utilizar ferramentas de tracing, como *Jaeger* e *Zipkin*, para monitorar e entender as interações entre eles.

## Desempenho dos Microserviços
- O tempo total de resposta dos microserviços é de aproximadamente **5 segundos**.
  - Microserviço 1: **1 segundo**
  - Microserviço 2: **2 segundos**
  - Microserviço 3: **2 segundos**
  
## Ferramentas de Tracing
### Jaeger
- Utilizado para coletar e visualizar traces de microserviços.
- Permite acesso a detalhes sobre chamadas entre os serviços.
- O apresentador acessa o Jaeger através do endereço `localhost:22.16`.

### Zipkin
- Outra ferramenta que também fornece funcionalidades de tracing.
- O apresentador acessa o Zipkin através do endereço `localhost:2.14:94`.

## Usando o Zipkin
1. **Buscar Traces**
   - O usuário pode buscar pelo *service name* (ex: microservice demo).
   - Exibe requisições feitas, mostrando detalhes como:
     - Chamadas entre microserviços.
     - **SPAN ID** e **parent ID**.
     - Nome da biblioteca utilizada e **SPAN Kind**.

2. **Interpretação dos Dados**
   - O usuário pode expandir os detalhes de cada microserviço.
   - Visualiza como os microserviços se inter-relacionam:
     - Microserviço 1 chama o Microserviço 2.
     - Microserviço 2 chama o Microserviço 3.
   - **Durations** e tempos de resposta são apresentados, permitindo identificar onde ocorrem atrasos.

## Usando o Jaeger
- Semelhante ao Zipkin, permite visualizar e filtrar informações sobre os microserviços.
- O usuário pode aplicar filtros e tags para encontrar traces específicos.

## Análise de Erros
- Ambas as ferramentas ajudam a identificar problemas:
  - Quando um microserviço falha, o tracing mostra onde ocorreu a falha.
  - O usuário pode ver as interações e identificar qual microserviço causou o erro.

## Conclusão
- O uso de ferramentas de tracing como Jaeger e Zipkin é fundamental para entender melhor o funcionamento e a performance dos microserviços.
- No próximo vídeo, o apresentador vai demonstrar um pouco do código utilizado para implementar os microserviços, reforçando a compreensão teórica com prática.

## Próximos Passos
- Assistir ao próximo vídeo para ver a implementação do código.
- Praticar o uso de Jaeger e Zipkin em seus próprios projetos de microserviços.



---

## modulo_10_11603.mp4

# Notas de Estudo sobre Microserviços e Tracing

## Introdução
Nesta aula, foi discutido o funcionamento de microserviços e a importância do tracing para monitorar e diagnosticar problemas entre eles. Utilizou-se ferramentas como **Zipkin** e **Jaeger** para visualizar as requisições e o desempenho dos microserviços.

## Principais Conceitos

### Tempo de Resposta dos Microserviços
- O tempo total de resposta foi de 5 segundos, composto por:
  - **Microserviço 1:** 1 segundo
  - **Microserviço 2:** 2 segundos
  - **Microserviço 3:** 2 segundos

### Ferramentas de Tracing
- **Jaeger** e **Zipkin** são ferramentas de tracing que permitem monitorar as chamadas entre microserviços.
- Ambas as ferramentas ajudam a coletar e analisar os *traces* das requisições.

### Acessando o Zipkin
1. Acesse o Zipkin através do endereço `localhost:9411`.
2. Utilize a opção "find a trace" para buscar pelo nome do serviço (exemplo: **microservice demo**).
3. Resultados incluem:
   - Visualização de requisições passadas.
   - Detalhamento de chamadas entre microserviços (ex: Microserviço 1 → Microserviço 2 → Microserviço 3).
   - Informações como *SPAN ID* e *Parent ID*.

### Entendendo SPAN
- Um **SPAN** é um trecho de código que representa uma operação executada e possui um ponto de início e um de fim.
- Exemplo: Um SPAN que levou 5 segundos para ser resolvido devido a dependências de outros microserviços.

## Acessando o Jaeger
- Acesse o Jaeger através do endereço `localhost:16686`.
- Selecione o serviço desejado e aplique filtros para refinar a busca.
- O Jaeger também fornece informações similares ao Zipkin, como:
  - Número de SPANs executados.
  - Detalhamento de chamadas entre microserviços.
  - Identificação de erros e problemas ocorridos.

## Diagnóstico de Problemas
- Ambas as ferramentas são úteis para identificar a origem de erros nas requisições.
- A visualização clara das dependências entre microserviços ajuda a entender onde as falhas ocorrem.

## Conclusão
- O uso de ferramentas de tracing como Jaeger e Zipkin é essencial para monitorar o desempenho e solucionar problemas em arquiteturas de microserviços.
- Na próxima aula, será apresentado um exemplo de código para demonstrar a implementação dos microserviços discutidos.

## Próximos Passos
- Assistir ao próximo vídeo para aprender sobre a implementação prática dos microserviços.
- Explorar mais sobre ferramentas de tracing e suas aplicações em cenários do mundo real.



---

## modulo_10_11604.mp4

# Estudo sobre Microserviços e Tracing

## Introdução
No vídeo anterior, foram apresentados microserviços e como eles se comunicam entre si, levando a um tempo total de resposta de aproximadamente 5 segundos.

## Principais Microserviços e Tempos
- **Microserviço 1:** 1 segundo
- **Microserviço 2:** 2 segundos
- **Microserviço 3:** 2 segundos

## Ferramentas de Tracing
### Jaeger
- Ferramenta utilizada para visualizar *traces* de microserviços.
  
### Zipkin
- Outra ferramenta que também permite o *tracing* de microserviços.

### Comparação entre Jaeger e Zipkin
- Ambas as ferramentas oferecem funcionalidades semelhantes para análise de *traces*.
- O acesso a ambas pode ser feito via `localhost` com portas específicas.

## Demonstração de Uso do Zipkin
1. Acesse o Zipkin em `localhost:9411`.
2. Utilize a funcionalidade "Find a Trace".
3. Insira o **service name** como "microservice demo".
4. Execute a busca e observe os resultados:
   - Exibição de requisições anteriores (ex: 7 e 8 minutos atrás).
   - Visualização das chamadas entre microserviços:
     - Microserviço 1 chama o Microserviço 2
     - Microserviço 2 chama o Microserviço 3

### Detalhes de Traces
- **SPAN ID:** Identificação única do trecho de código executado.
- **Parent ID:** Indica o microserviço que fez a chamada (pai).
- **SPAN Kind:** Tipo de operação realizada.

### Análise de Duração
- O tempo total de 5 segundos é resultado das dependências entre os microserviços.

## Demonstração de Uso do Jaeger
1. Acesse o Jaeger em `localhost:16686`.
2. Selecione o microserviço que deseja analisar.
3. Execute a busca por *traces*.
4. Visualização de múltiplos SPANs, mostrando a fluência das chamadas entre microserviços.

### Identificação de Erros
- Quando algum microserviço apresenta erro, é possível visualizar:
  - A sequência de chamadas realizadas.
  - O microserviço que falhou e a descrição do erro.

## Conclusão
- O uso de ferramentas de *tracing* como Jaeger e Zipkin é fundamental para entender e diagnosticar problemas em microserviços.
- Com a visualização dos *traces*, é possível identificar rapidamente a origem de falhas e otimizar a comunicação entre serviços.

## Próximos Passos
- No próximo vídeo, será apresentada uma visão geral do código que foi utilizado para desenvolver os microserviços, proporcionando um entendimento mais profundo sobre sua implementação.



---

## modulo_10_11605.mp4

# Estudo sobre Microserviços e Tracing

## Introdução
No vídeo anterior, foi discutido o funcionamento de microserviços, mostrando como eles se comunicam e o tempo que cada um leva para processar requisições.

## Tempo de Execução dos Microserviços
- **Microserviços envolvidos:**
  - Microserviço 1: 1 segundo
  - Microserviço 2: 2 segundos
  - Microserviço 3: 2 segundos
- **Tempo total:** 5 segundos para a chamada completa.

## Ferramentas de Tracing
Duas ferramentas principais foram mencionadas para rastreamento de microserviços:

1. **Jaeger**
   - Usado para coletar e visualizar traces.
2. **Zipkin**
   - Também utilizado para rastreamento, similar ao Jaeger.

### Acessando o Zipkin
- Endereço: `localhost:9411`
- Para encontrar um trace:
  1. Acesse a opção "find a trace".
  2. Insira o *service name* (exemplo: `microservice demo`).
  3. Execute a consulta.

### Resultados no Zipkin
- O Zipkin mostrou duas requisições feitas 7 e 8 minutos atrás.
- Visualização das chamadas:
  - Microserviço 1 chama o Microserviço 2.
  - Microserviço 2 chama o Microserviço 3.
- Informações exibidas:
  - Nome do serviço.
  - *SPAN ID* e *parent ID* (identifica a hierarquia das chamadas).

## Entendendo SPAN
- **Definição:** Um *SPAN* é um trecho de código executado com um ponto de início e um fim.
- **Exemplo de duração:** Um *SPAN* pode ter durado 5 segundos, dependendo de outros serviços.

## Acessando o Jaeger
- Endereço: `localhost:16686`
- Funcionalidades:
  - Seleção do serviço desejado para visualização.
  - Filtragem de informações através de tags e outros parâmetros.
- Resultados semelhantes ao Zipkin:
  - Mostra SPANs e a relação entre os microserviços.

## Diagnóstico de Erros
- O uso de ferramentas de tracing ajuda a identificar problemas:
  - Exibe a sequência de chamadas entre os microserviços.
  - Indica onde ocorrem falhas e quais serviços estão envolvidos.
  
## Conclusão
- O tracing é essencial para monitorar e entender o comportamento de microserviços.
- No próximo vídeo, será apresentado um código exemplo para demonstrar a implementação dos microserviços discutidos.

## Próximos Passos
- Assistir ao próximo vídeo para ver a implementação prática e o código relacionado aos microserviços.



---

## modulo_10_11606.mp4

# Estudo sobre Comunicação Assíncrona

## Introdução
Neste vídeo, o palestrante discute os riscos do uso indiscriminado de REST em sistemas e apresenta a *comunicação assíncrona* como uma solução mais robusta.

## Riscos do Uso de REST
- O uso excessivo de REST pode levar à:
  - **Perda de informação**
  - **Latência** em sistemas, mesmo que estejam online, mas lentos
- A comunicação assíncrona surge como uma alternativa para mitigar esses riscos.

## O que é Comunicação Assíncrona?
- **Definição**: Sistemas não se comunicam diretamente e as interações ocorrem em momentos diferentes.
- **Desacoplamento**: Um sistema não depende diretamente do outro, o que aumenta a flexibilidade e a resiliência.

## Exemplo Prático: Sistema de E-commerce
- Cenário: Um sistema de e-commerce que realiza várias ações após uma compra aprovada.
  - **Ações Necessárias**:
    - Baixar estoque
    - Emitir nota fiscal
    - Enviar para separação no centro de distribuição
- **Solução**: Em vez de enviar informações diretamente para cada sistema, a informação é enviada para um *tópico* (um canal de comunicação).
  - **Benefícios**:
    - Mensagens não são perdidas, mesmo que um sistema esteja fora do ar.
    - Sistemas podem processar mensagens quando voltam a estar disponíveis.

## Comparação: Comunicação Assíncrona vs. Comunicação Sincrona
- **Comunicação Sincrona**:
  - Exemplo: Ligação telefônica
    - Mensagens enviadas em tempo real.
    - Se houver problemas, a mensagem pode não ser entendida.
- **Comunicação Assíncrona**:
  - Exemplo: Envio de cartas pelos correios
    - Mensagem não é recebida imediatamente, mas pode ser lida posteriormente.
    - Mais segura em termos de resiliência.

## Vantagens da Comunicação Assíncrona
- **Segurança**: A comunicação assíncrona é mais confiável em relação à resiliência.
- **Escalabilidade**: Permite que um sistema se comunique com múltiplos outros sistemas ao mesmo tempo.
- **Menos Acoplamento**: Reduz a dependência entre sistemas, facilitando manutenções e atualizações.

## Conclusão
- A compreensão da comunicação assíncrona é fundamental para melhorar a eficiência e a robustez dos sistemas.
- O palestrante promete explorar mais sobre comunicação assíncrona em vídeos futuros.

## Próximos Passos
- Acompanhar os próximos vídeos para entender mais sobre a comunicação assíncrona e suas aplicações práticas.



---

## modulo_10_11607.mp4

# Comunicação Assíncrona em Sistemas

## Introdução
No vídeo anterior, discutimos os perigos do uso excessivo de REST para comunicação entre sistemas. Este vídeo foca na importância da comunicação assíncrona e como ela pode melhorar a eficiência e a resiliência dos sistemas.

## Riscos do Uso de REST
- **Perda de Informação**: O uso inadequado de REST pode levar à perda de dados.
- **Latência**: Mesmo sistemas operacionais podem apresentar lentidão, causando problemas de performance.

## O Que É Comunicação Assíncrona?
- **Definição**: Sistemas se comunicam de maneira que não precisam estar ativos ao mesmo tempo; as interações ocorrem em momentos diferentes.
- **Desacoplamento**: Um sistema não depende diretamente de outro para operar.

## Exemplos Práticos
### Cenário de E-commerce
- **Sistema 1**: Sistema de e-commerce que precisa comunicar eventos como "compra aprovada".
- **Sistemas Interessados**:
  1. **Baixar Estoque**
  2. **Emitir Nota Fiscal**
  3. **Enviar para Separação no Centro de Distribuição**
- **Solução**: Em vez de enviar mensagens diretamente para cada sistema, o Sistema 1 envia informações para um **tópico**.
  - **Tópico**: Local onde mensagens são enviadas e recebidas.
  - **Resiliência**: Se um sistema estiver fora do ar, a mensagem não é perdida e pode ser lida posteriormente.

### Comparativo: Ligações vs. Correios
- **Ligação Telefônica**:
  - Comunicação em tempo real.
  - Problemas de comunicação podem resultar em perda de informação.
- **Carta**:
  - Mensagem não é recebida imediatamente.
  - O destinatário pode ler a mensagem mais tarde, garantindo que a informação não se perca.

## Vantagens da Comunicação Assíncrona
- **Segurança**: Maior resiliência em relação à perda de dados.
- **Escalabilidade**: Permite que sistemas se comuniquem com múltiplos outros sistemas simultaneamente, sem forte acoplamento.

## Conclusão
Entender a comunicação assíncrona é crucial para melhorar a eficiência e a resiliência dos sistemas modernos. No próximo vídeo, serão discutidos mais pontos importantes sobre esse tema.

---

### Dicas de Estudo
- **Revise os conceitos de comunicação assíncrona e desacoplamento**.
- **Pratique exemplos** de cenários onde a comunicação assíncrona pode ser aplicada.
- **Compare e contraste** os métodos de comunicação síncrona e assíncrona para entender melhor suas vantagens e desvantagens.



---

## modulo_10_11657.mp4

## Estudo sobre Comunicação Assíncrona

### Introdução
- A comunicação em sistemas é um tema crucial no desenvolvimento de software.
- O uso indiscriminado de REST pode levar à perda de informações e a problemas de latência.

### Perigos do Uso de REST
- **Perda de Informação**: Há um risco significativo de que informações sejam perdidas em chamadas REST.
- **Latência**: Sistemas lentos, mesmo que estejam operacionais, podem afetar o desempenho geral.

### O que é Comunicação Assíncrona?
- **Definição**: Comunicação onde os sistemas não precisam interagir diretamente em tempo real.
- **Desacoplamento**: Sistemas operam de forma independente, permitindo maior flexibilidade.

### Exemplo Prático: Sistema de E-commerce
- **Cenário**: Um sistema de e-commerce que precisa se comunicar com vários outros sistemas após uma compra aprovada.
  - **Sistemas envolvidos**:
    - Sistema de estoque
    - Emissão de nota fiscal
    - Centro de distribuição
- **Problema**: Se o sistema 1 tiver que enviar informações para cada um dos outros sistemas, isso pode ser arriscado.

### Solução com Tópicos
- **Tópico**: Um local para enviar e receber mensagens.
  - As mensagens ficam armazenadas no tópico até que os sistemas estejam prontos para processá-las.
- **Vantagens**:
  - Se um sistema estiver fora do ar, a mensagem não é perdida; aguarda no tópico.
  - Quando o sistema volta, ele pode ler as mensagens acumuladas.

### Comparação: Correios vs. Ligação Telefônica
- **Ligação Telefônica**: Comunicação em tempo real, onde falhas de comunicação podem levar à perda de informações.
- **Correios**: Mensagens são entregues posteriormente, permitindo que o destinatário leia a mensagem quando estiver disponível.

### Benefícios da Comunicação Assíncrona
- **Segurança**: A comunicação assíncrona é mais resiliente a falhas.
- **Eficiência**: Permite que um sistema se comunique com múltiplos sistemas simultaneamente, sem forte acoplamento.

### Conclusão
- É fundamental entender como a comunicação assíncrona funciona para melhorar o desenvolvimento e a manutenção de sistemas.
- A prática de comunicação assíncrona pode fazer uma diferença significativa no dia a dia de desenvolvedores.

### Próximos Passos
- Em vídeos futuros, mais exemplos e detalhes sobre comunicação assíncrona serão abordados.



---

## modulo_10_11658.mp4

# Comunicação Assíncrona em Sistemas

## Introdução
No vídeo anterior, foi discutido os perigos do uso excessivo de REST para comunicação entre sistemas. A abordagem tradicional pode resultar em perda de informações e latência. 

## Problemas do Uso de REST
- **Perda de Informação**: Risco elevado quando sistemas estão acoplados.
- **Latência**: Mesmo sistemas em funcionamento podem ter desempenho lento, resultando em baixa eficiência.

## O que é Comunicação Assíncrona?
- A comunicação assíncrona permite que sistemas se comuniquem sem depender de respostas imediatas.
- Os sistemas ficam **desacoplados**, ou seja, um não precisa esperar pelo outro para continuar sua operação.

### Vantagens
- **Resiliência**: Mensagens não são perdidas mesmo que um sistema esteja fora do ar.
- **Escalabilidade**: Vários sistemas podem se comunicar simultaneamente sem interferir uns nos outros.

## Exemplo Prático: E-commerce
1. **Sistema 1**: Gerencia a aprovação da compra.
2. **Sistema 2**: Baixa o estoque.
3. **Sistema 3**: Emissão de nota fiscal.
4. **Sistema 4**: Envio para separação no centro de distribuição.

### Problema Sem Comunicação Assíncrona
- O Sistema 1 precisaria enviar informações para todos os sistemas diretamente, o que é arriscado e complexo.

### Solução com Tópicos
- **Tópicos**: Um canal onde mensagens são enviadas e recebidas.
  - Se um sistema estiver fora do ar, a mensagem ficará armazenada no tópico.
  - Quando o sistema voltar, ele poderá acessar essa mensagem.

## Comparação: Correios vs. Ligação Telefônica
- **Ligação Telefônica**: Comunicação em tempo real; falhas podem resultar em mensagens incompletas.
- **Carta pelos Correios**: Mensagem não é recebida imediatamente, mas é entregue eventualmente. 

## Conclusão
- A comunicação assíncrona é **fundamental** para garantir a segurança e eficiência na troca de informações entre sistemas.
- Essa abordagem pode trazer uma diferença significativa no cotidiano do desenvolvimento de sistemas.

## Próximos Passos
- Continuar a discussão sobre comunicação assíncrona em vídeos futuros.



---

## modulo_10_11659.mp4

# Resumo da Arquitetura Baseada em Eventos (Event Driven Architecture - EDA)

## Introdução
- **Tema**: Importância da Arquitetura Baseada em Eventos.
- **Definição**: Event Driven Architecture (EDA) é uma arquitetura que permite o trabalho baseado em eventos.

## O que são Eventos?
- **Definição de Evento**: Um evento é algo que já aconteceu no sistema.
  - *Importante*: Não existem eventos futuros, apenas eventos passados.
  
### Exemplos de Eventos
- Compra aprovada.
- A porta do carro abriu.
- O site foi acessado.
- Cliente cadastrado.
- Dados alterados.
- E-mail enviado.

## Funcionamento da EDA
- Eventos ocorrem frequentemente nos sistemas.
- É fundamental entender os eventos para determinar a comunicação entre:
  - Sistemas que produzem eventos.
  - Sistemas que leem eventos.

## Tipos de Eventos
- Existem diferentes tipos de eventos que influenciam a estratégia de comunicação.
- **Próximo Passo**: No próximo vídeo, serão discutidos os tipos de eventos e quando utilizá-los.

## Conclusão
- A EDA é uma abordagem essencial para sistemas modernos.
- Compreender os eventos e suas classificações é crucial para a implementação eficaz da arquitetura.

### O que esperar no próximo vídeo
- Tipos de eventos.
- Quando e como produzir eventos.

---

## Dicas para Estudo
- **Revisar exemplos de eventos**: Tente criar seus próprios exemplos para melhor compreensão.
- **Refletir sobre a comunicação entre sistemas**: Como os sistemas interagem quando eventos são gerados?
- **Preparar perguntas**: Quais dúvidas você tem sobre a produção e utilização de eventos?



---

## modulo_10_11660.mp4

# Arquitetura Orientada a Eventos (Event Driven Architecture - EDA)

## Introdução
A Arquitetura Orientada a Eventos, ou EDA, é uma abordagem crucial para o desenvolvimento de sistemas que são baseados em eventos. Este modelo permite que os sistemas respondam rapidamente a mudanças e interações.

## O que são Eventos?
- **Definição de Evento**: Um evento é algo que já ocorreu no sistema. É importante notar que eventos são sempre registros do passado.
- **Exemplos de Eventos**:
  - Compra aprovada
  - A porta do carro abriu
  - O site foi acessado
  - Cliente cadastrado
  - Dados alterados
  - E-mail enviado

## Importância dos Eventos
- Eventos são dados que refletem ações que já aconteceram.
- Nos sistemas modernos, muitos eventos ocorrem continuamente, criando um fluxo constante de informações.

## Tipos de Eventos
- É fundamental entender os diferentes tipos de eventos que podem ocorrer nos sistemas, pois isso afetará a **estratégia de comunicação** entre:
  - Sistemas que produzem os eventos.
  - Sistemas que consomem ou leem esses eventos.

## Próximos Passos
- Nos vídeos seguintes, será discutido:
  - Os **tipos de eventos**.
  - Quando e como utilizar cada tipo de evento.
- A intenção é esclarecer dúvidas comuns sobre a produção e uso de eventos nos sistemas.

## Conclusão
A Arquitetura Orientada a Eventos é uma ferramenta poderosa para o desenvolvimento de sistemas responsivos e dinâmicos. Compreender a natureza dos eventos e suas aplicações é essencial para construir sistemas eficazes.

---

**Notas Importantes**:
- Lembre-se que eventos são sempre uma representação do que já ocorreu.
- A escolha do tipo de evento pode impactar diretamente a performance e a comunicação dos sistemas envolvidos.

Prepare-se para o próximo vídeo, onde exploraremos mais sobre os diferentes tipos de eventos e suas utilizações!



---

## modulo_10_11661.mp4

# Arquitetura Orientada a Eventos (Event Driven Architecture - EDA)

## Introdução
- A Arquitetura Orientada a Eventos é uma abordagem fundamental para o desenvolvimento de sistemas que se baseiam em eventos.
- O conceito central é que os sistemas operam e se comunicam em função de eventos que ocorrem.

## O que é um Evento?
- **Definição:** Um *evento* é algo que aconteceu no sistema.
  - *Importante:* Um evento sempre se refere a algo que já ocorreu no passado.
  
### Exemplos de Eventos
- Compra aprovada
- Porta do carro aberta
- Acesso ao site
- Cliente cadastrado
- Dados alterados
- E-mail enviado

## Tipos de Eventos
- É fundamental entender que existem diferentes tipos de eventos nos sistemas.
- Cada tipo de evento pode influenciar a estratégia de comunicação entre os sistemas que produzem os eventos e os que os consomem.

### Importância dos Tipos de Eventos
- A escolha do tipo de evento impacta:
  - Como os eventos são produzidos
  - Quando e como são utilizados
- Será abordado no próximo vídeo quais são os tipos de eventos e suas aplicações.

## Conclusão
- A compreensão da Arquitetura Orientada a Eventos e dos tipos de eventos é crucial para o desenvolvimento eficaz de sistemas baseados em eventos.
- O próximo passo é aprofundar no conhecimento sobre como produzir e utilizar esses eventos de forma adequada.

## Próximos Passos
- Assistir ao próximo vídeo para entender melhor:
  - Os diferentes tipos de eventos
  - Quando e como utilizá-los na prática

### Dicas para Estudo
- Reflita sobre exemplos de eventos que você já encontrou em sistemas que utilizou.
- Tente identificar o tipo de evento e sua relevância no fluxo de informações de um sistema.



---

## modulo_10_11662.mp4

# Estudo sobre Event Driven Architecture (EDA)

## Introdução à Arquitetura Baseada em Eventos

- A **Event Driven Architecture (EDA)** é uma forma importante de trabalhar com sistemas que se baseiam em eventos.
- A arquitetura é centrada na ideia de que os sistemas reagem a eventos que já ocorreram.

## O que são Eventos?

- Um evento é definido como algo que **já aconteceu** no sistema.
- Eventos são sempre relacionados ao passado; não existem eventos futuros.
  
### Exemplos de Eventos:

- **Compra aprovada**
- **A porta do carro foi aberta**
- **O site foi acessado**
- **Cliente cadastrado**
- **Dados alterados**
- **E-mail enviado**

## Importância dos Eventos

- Em sistemas complexos, muitos eventos ocorrem continuamente.
- Esses eventos são essenciais para a comunicação entre diferentes partes do sistema.

## Tipos de Eventos

- É crucial entender os diferentes tipos de eventos em um sistema, pois isso afetará a estratégia de comunicação entre:
  - Sistemas que **produzem eventos**
  - Sistemas que **leem eventos**

### Próximos Passos

- No próximo vídeo, será discutido:
  - Os diferentes tipos de eventos
  - Quando e como utilizar cada tipo de evento
  - Dúvidas comuns sobre a produção de eventos

## Conclusão

- A compreensão dos eventos e da Event Driven Architecture é fundamental para o desenvolvimento de sistemas modernos e eficientes.
- Preparar-se para o próximo conteúdo ajudará a esclarecer as diferentes estratégias de eventos e sua aplicação prática.



---

## modulo_10_11663.mp4

# Esquema Evolutivo em Sistemas de Mensagem

## Introdução
O esquema evolutivo é um conceito fundamental na comunicação entre sistemas, especialmente em arquiteturas de microserviços. Este conceito visa garantir que as mudanças nos formatos de mensagens não causem falhas nos sistemas que consomem essas mensagens.

## Importância
- O esquema de mensagem é crucial para a comunicação entre publicadores e consumidores.
- Mudanças inesperadas no formato da mensagem podem causar **caos** na aplicação.

## Estrutura da Mensagem
- Exemplo de mensagem:
  - `order ID: 1`
  - `status: aprovado`
  - `product ID: 1`
- A importância de um formato consistente:
  - Se um sistema alterar o nome de um campo (ex: de `product_id` para `product ID`), o sistema consumidor pode não reconhecer a mensagem, resultando em erros.

## Necessidade de Compatibilidade
- Com múltiplos microserviços consumindo mensagens de um único publicador, a mudança no formato da mensagem pode causar falhas em todos os serviços consumidores.
- É essencial ter um padrão claro para o envio e recebimento de mensagens.

## Tipos de Compatibilidade de Esquema
Para manter a compatibilidade ao longo do tempo, existem três tipos básicos de evolução de esquema:

### 1. Compatibilidade para Frente (*Forward Compatibility*)
- **Definição**: Dados são produzidos com um novo esquema, mas ainda podem ser lidos pelo esquema antigo.
- **Exemplo**:
  - Sistema 1 muda o formato de envio, mas o sistema 2 ainda consegue ler as mensagens sem problemas.

### 2. Compatibilidade para Trás (*Backward Compatibility*)
- **Definição**: Dados produzidos com o esquema antigo podem ser lidos como se fossem do novo esquema.
- **Exemplo**:
  - Um consumidor pode implementar uma nova funcionalidade antes que o produtor envie o novo campo em suas mensagens.
  - Caso um campo novo (ex: `bônus`) seja introduzido, o consumidor pode se preparar para lê-lo antes que o produtor comece a enviá-lo.

### 3. Compatibilidade Total (*Full Compatibility*)
- **Definição**: Combina compatibilidade para frente e para trás, permitindo que esquemas antigos sejam processados e novas mudanças sejam previstas.
- **Desafios**:
  - Requer planejamento cuidadoso e pode não ser sempre necessário.

## Conclusão
O esquema evolutivo é essencial para garantir a **resiliência** dos sistemas que dependem de mensagens. As três formas de manter a compatibilidade são fundamentais para a evolução dos sistemas e para prevenir falhas decorrentes de mudanças no formato das mensagens.



---

## modulo_10_11664.mp4

# Esquema Evolutivo

## Importância do Esquema Evolutivo
- O esquema evolutivo é *extremamente importante* em sistemas que utilizam mensagens entre publicadores e consumidores.
- Mudanças no formato das mensagens podem causar *caos* nas aplicações.

## Problemas com Mudanças de Formato
- Exemplo de mensagem:
  - `order ID: 1`
  - `status: aprovado`
  - `product ID: 1`
- Se o formato da mensagem mudar (ex.: de `product_id` para `product ID`), o sistema consumidor pode não reconhecer a mensagem, resultando em erros.

## Necessidade de Compatibilidade
- À medida que os sistemas evoluem, o formato das mensagens pode mudar.
- Se um microserviço altera o formato da mensagem, todos os microserviços que consomem essa mensagem podem quebrar.
- É essencial estabelecer um padrão de envio e recebimento das mensagens para evitar problemas.

## Tipos de Compatibilidade
### 1. Forward Compatibility
- **Definição**: Dados são produzidos com um novo esquema, mas ainda são compatíveis com o esquema antigo.
- **Exemplo**: O sistema 1 muda o padrão de envio, mas o sistema 2 ainda consegue ler as informações antigas sem alteração de código.

### 2. Backward Compatibility
- **Definição**: Dados produzidos no esquema antigo podem ser lidos como um novo esquema.
- **Exemplo**: Um consumidor pode se preparar para receber novos dados (como um campo "bônus") antes que o produtor comece a enviar essas informações.
  - O consumidor pode implementar a nova feature antecipadamente, mesmo que o produtor ainda não a tenha enviado.

### 3. Full Compatibility
- **Definição**: Combinação das duas anteriores; possibilita a leitura de esquemas antigos e a previsão de novas mudanças.
- **Características**:
  - Requer um planejamento cuidadoso.
  - Nem sempre é necessário, pois pode demandar muitos recursos.

## Conclusão
- O esquema evolutivo é crucial para a integração e funcionamento eficiente de sistemas que se comunicam via mensagens.
- A implementação de técnicas de compatibilidade é fundamental para evitar que mudanças disruptivas causem falhas em sistemas interconectados.



---

## modulo_10_11665.mp4

# Esquema Evolutivo

## Introdução
O esquema evolutivo é um conceito crucial para a comunicação entre sistemas, especialmente em sistemas que utilizam publicadores e consumidores de mensagens. Este tópico aborda como manter a compatibilidade de mensagens durante as mudanças de esquema.

## Importância do Esquema de Mensagem
- **Publicador e Consumidor**: O publicador envia mensagens em um formato específico que o consumidor deve entender.
- **Mudanças no Esquema**: Alterações inesperadas no formato das mensagens podem causar falhas na leitura dos dados, levando a problemas em aplicações.

## Exemplo de Problema
- Se um sistema que publica mensagens muda o formato de `product_id` para `product_id` (sem o underline), o sistema consumidor não conseguirá ler a mensagem, resultando em falhas.

## Necessidade de Compatibilidade
- Com múltiplos microserviços interagindo, uma mudança no formato de mensagem pode impactar todos os serviços consumidores.
- É essencial definir e reforçar o padrão de envio e recebimento das mensagens.

## Tipos de Compatibilidade

### 1. Forward Compatibility
- **Definição**: Dados são produzidos com um novo esquema, mantendo a compatibilidade de leitura com o esquema antigo.
- **Funcionamento**:
  - O sistema 1 muda o padrão de informação, mas o sistema 2 ainda consegue ler as mensagens sem alteração de código.
  - O sistema 1 pode enviar novos dados sem quebrar a funcionalidade do sistema 2.

### 2. Backward Compatibility
- **Definição**: Dados produzidos no esquema antigo podem ser lidos como se fossem do novo esquema.
- **Funcionamento**:
  - Um consumidor pode se preparar para uma nova feature com antecedência, mesmo que o produtor ainda não esteja enviando os dados nesse novo formato.
  - Exemplo: Introdução de um campo `bônus` que o consumidor pode implementar antes do produtor enviar esse novo dado.

### 3. Full Compatibility
- **Definição**: Combina os conceitos de forward e backward compatibility.
- **Funcionamento**:
  - Permite que esquemas antigos sejam processados enquanto se prevê novas mudanças.
  - Requer planejamento cuidadoso, mas nem sempre é necessário devido à complexidade e ao esforço envolvido.

## Conclusão
- Existem três formas principais de garantir a evolução do esquema:
  - **Forward Compatibility**
  - **Backward Compatibility**
  - **Full Compatibility**
- A escolha do método de compatibilidade depende das necessidades do sistema e do nível de planejamento disponível.

## Considerações Finais
A manutenção da compatibilidade entre esquemas é fundamental para a operação contínua de sistemas interconectados, e a escolha da abordagem apropriada pode evitar que mudanças simples causem grandes problemas em um ecossistema de microserviços.



---

## modulo_10_11666.mp4

# Esquema Evolutivo em Sistemas

**Introdução**
- A palestra aborda a importância do *esquema evolutivo* em sistemas que utilizam *publicadores* e *consumidores* de mensagens.
- O foco está na comunicação entre sistemas e a necessidade de manter a compatibilidade ao longo do tempo.

## Importância do Esquema da Mensagem
- Um *esquema de mensagem* define o formato dos dados que um sistema publica e que outro sistema consome.
- Exemplo de mensagem:
  - `order ID: 1`
  - `status: aprovado`
  - `product ID: 1`

### Problemas de Incompatibilidade
- Mudanças inesperadas no formato das mensagens podem causar falhas:
  - Exemplo: Alteração de `product_id` para `product ID` sem o underline pode quebrar a leitura.

## Necessidade de Compatibilidade
- À medida que os sistemas evoluem, os formatos de mensagem também mudam.
- Sistemas dependentes devem ser capazes de lidar com essas mudanças sem falhas.

## Tipos de Compatibilidade
### 1. Forward Compatibility
- **Definição**: Dados são produzidos com um novo esquema mas ainda são compatíveis com o esquema antigo.
- **Funcionamento**:
  - O sistema que publica pode mudar o formato sem afetar o sistema que consome.
  - O consumidor continua a funcionar normalmente enquanto novos dados são introduzidos.

### 2. Backward Compatibility
- **Definição**: Dados produzidos em um esquema antigo podem ser lidos como se fossem de um novo esquema.
- **Funcionamento**:
  - O consumidor pode implementar novas funcionalidades antes que o produtor envie os dados correspondentes.
  - Exemplo: Um novo campo chamado `bônus` é adicionado, e o consumidor pode se preparar para utilizá-lo antes que o produtor comece a enviá-lo.

### 3. Full Compatibility
- **Definição**: Combinação das duas compatibilidades anteriores.
- **Funcionamento**:
  - Permite que esquemas antigos sejam processados enquanto se antecipa mudanças futuras.
  - É um método complexo que requer planejamento cuidadoso, mas nem sempre é necessário.

## Conclusão
- Compreender e implementar um *esquema evolutivo* é crucial para o sucesso de sistemas que dependem de comunicação entre microserviços.
- As três formas de compatibilidade (forward, backward e full) oferecem diferentes estratégias para manter a integridade e funcionalidade dos sistemas durante as mudanças. 

**Observação Final**
- O *esquema evolutivo* é uma ferramenta essencial para evitar o caos nas aplicações e garantir a continuidade do serviço.



---

## modulo_10_11667.mp4

# Resumo da Aula sobre CQRS e Banco de Dados

## Introdução ao CQRS
- **CQRS** (Command Query Responsibility Segregation) é um padrão de arquitetura que divide o sistema em duas partes:
  - **Comando**: Responsável pelas regras de negócio.
  - **Consulta**: Responsável pela leitura de dados, que não necessariamente contém regras de negócio.

## Estrutura de Banco de Dados
- No CQRS, é possível trabalhar de duas maneiras em relação ao banco de dados:
  - **Um único banco de dados** para comandos e consultas.
  - **Dois bancos de dados**:
    - Um para operações de *escrita*.
    - Um para operações de *leitura*.

## Motivos para Usar Dois Bancos de Dados
1. **Performance**:
   - Um banco de dados intensivo em *escrita* pode ser sobrecarregado com *leituras*, resultando em baixa performance.
   - Um banco de dados intensivo em *leitura* pode ter baixa *escrita*, ou vice-versa.

2. **Estrutura de Dados**:
   - Dados podem ser armazenados de forma estruturada em um banco de dados relacional para garantir consistência e transações.
   - Consultas complexas podem exigir estruturas de dados otimizadas para facilitar a leitura.

3. **Complexidade de Consultas**:
   - Consultas complexas podem ser difíceis de otimizar em um único banco de dados. Separar os dados pode facilitar a criação de relatórios e consultas.
   - É possível utilizar diferentes tipos de bancos de dados (orientados a documentos, colunar, gráfico) para atender a necessidades específicas.

## Vantagens da Separação de Bancos de Dados
- **Velocidade**:
  - A separação permite que as operações de *escrita* e *leitura* sejam realizadas de forma mais rápida.
  
- **Simplicidade**:
  - Estruturas diferentes para leitura e escrita podem aumentar a simplicidade e a eficiência das operações.

## Consistência Eventual
- Um dos desafios de usar dois bancos de dados é a *consistência eventual*:
  - Os dados gravados em um banco de dados podem não estar imediatamente atualizados no outro.
  - É importante entender se o sistema pode tolerar essa inconsistência.
  
- **Decisão sobre a Estrutura**:
  - Se o sistema não pode estar inconsistente, deve-se optar por um único banco de dados.
  - Se a inconsistência é aceitável, a separação pode ser vantajosa.

## Conclusão
- A escolha entre um ou dois bancos de dados deve ser baseada nas necessidades específicas do sistema.
- Entender as **vantagens** e **desvantagens** de cada abordagem é crucial para uma implementação eficiente.

**Espero que você tenha compreendido as diferenças entre trabalhar com um ou dois bancos de dados no contexto do CQRS!**



---

## modulo_10_11668.mp4

# Estudo sobre CQRS e Estrutura de Banco de Dados

## Introdução
No vídeo anterior, foi discutido o conceito de CQRS (Command Query Responsibility Segregation), que divide o sistema em duas partes: uma para comandos (escrita) e outra para consultas (leitura).

## Principais Conceitos de CQRS
- **Divisão do sistema**: 
  - **Parte de Comandos**: Onde estão as regras de negócio.
  - **Parte de Consultas**: Não necessariamente possui regras de negócio.

## Modelos de Banco de Dados em CQRS
- **Banco de dados único**: Comandos e consultas acessam o mesmo banco de dados.
- **Dois bancos de dados**: 
  - Um banco para escrita (comandos).
  - Um banco para leitura (consultas).
  
### Vantagens de Usar Dois Bancos de Dados
1. **Desempenho**:
   - Evitar sobrecarga em um banco de dados intensivo em escrita ao lidar com leituras.
   - Separar operações intensivas em leitura e escrita pode melhorar a performance.

2. **Isolamento e Consistência**:
   - Necessidade de isolamento e transações durante a gravação.
   - Utilização de bancos de dados relacionais para dados estruturados.

3. **Facilidade nas Consultas**:
   - Estruturas de dados otimizadas para leitura podem simplificar consultas complexas.
   - Possibilidade de usar diferentes tipos de bancos de dados (ex: orientados a documentos, colunar, gráfico).

## Considerações sobre Consistência
- **Consistência Eventual**:
  - Ao usar dois bancos de dados, pode haver um atraso na sincronização de dados.
  - É importante entender que os dados podem não estar atualizados ao mesmo tempo.
  - Para sistemas que não podem estar inconsistentes, a utilização de um único banco de dados é recomendada.

## Conclusão
- A separação entre leitura e escrita através do CQRS pode trazer benefícios significativos, especialmente em sistemas com consultas complexas.
- A escolha entre um ou dois bancos de dados deve considerar a necessidade de desempenho, simplicidade nas consultas e consistência dos dados.

## Dicas para Implementação
- Avalie a complexidade das consultas que seu sistema precisa realizar.
- Considere as operações de leitura e escrita e como elas impactam na performance do sistema.
- Lembre-se de que consistência é fundamental para certos tipos de aplicações e deve ser priorizada.

---

Com isso, você terá uma visão clara sobre CQRS e como a estrutura de banco de dados pode impactar a eficiência e a eficácia do seu sistema.



---

## modulo_10_11669.mp4

# Resumo da Aula sobre CQRS e Banco de Dados

## Introdução ao CQRS
- **CQRS** (Command Query Responsibility Segregation) é um padrão arquitetural que separa as operações de leitura e escrita de um sistema.
- **Divisão em duas partes**:
  - **Comandos**: Parte responsável pelas regras de negócio.
  - **Consultas**: Parte responsável pela leitura de dados, que não necessariamente contém regras de negócio.

## Estrutura do Banco de Dados
- O sistema pode operar com um único banco de dados para leitura e escrita ou com **dois bancos de dados**:
  - **Banco de Dados para Escrita**: Focado em operações de comando.
  - **Banco de Dados para Consulta**: Focado em operações de leitura.

### Motivos para Utilizar Dois Bancos de Dados
1. **Performance**:
   - Evitar sobrecarga no banco de dados de escrita com operações de leitura.
   - Possuir um banco intensivo em leitura e outro em escrita.
   
2. **Isolamento e Estrutura**:
   - Necessidade de transações e isolamento ao gravar dados.
   - Utilização de um banco de dados relacional para garantir estrutura e consistência na escrita.

## Complexidade nas Consultas
- **Consultas complexas** podem exigir SQL otimizado e extensivo.
- Para facilitar as consultas:
  - Estruturar os dados de forma que a leitura seja mais simples e rápida.
  - Possibilidade de ter cópias dos dados em diferentes formatos (ex.: orientado a documentos, colunar, gráfico).

## Vantagens do CQRS
- Permite:
  - **Separação das camadas** de leitura e escrita.
  - Aumento da **velocidade** para gravação e leitura.
  
### Desafios do CQRS
- **Consistência Eventual**:
  - Os dados podem não estar sincronizados entre os bancos de dados.
  - É importante que o sistema tenha uma tolerância à inconsistência:
    - Se o sistema precisa estar sempre consistente, deve-se usar um único banco de dados.

## Considerações Finais
- Avaliar a necessidade de separar os bancos de dados em função das complexidades das queries.
- **Escolha do banco de dados** deve ser baseada nas operações predominantes:
  - **Escrita**: Priorizar consistência e estrutura.
  - **Leitura**: Priorizar simplicidade e performance.

## Conclusão
- A separação de comandos e consultas através do padrão CQRS é uma abordagem poderosa, mas deve ser utilizada com cuidado, considerando a necessidade de consistência dos dados no sistema.



---

## modulo_10_11670.mp4

# Resumo do Vídeo sobre CQRS

## Introdução ao CQRS
- **CQRS** (Command Query Responsibility Segregation) é um padrão arquitetural que divide o sistema em duas partes:
  - **Comandos**: Responsáveis por executar regras de negócio.
  - **Consultas**: Responsáveis por ler dados, sem necessariamente aplicar regras de negócio.

## Estrutura dos Bancos de Dados
- O padrão CQRS permite o uso de um ou dois bancos de dados:
  - **Um banco de dados**:
    - Tanto para comandos quanto para consultas.
  - **Dois bancos de dados**:
    - Um para escrita (comandos) e outro para leitura (consultas).
    - Os bancos de dados podem ser *sincronizados*.

### Vantagens de Usar Dois Bancos de Dados
1. **Performance**:
   - Separar bancos evita sobrecarga: 
     - Um banco intensivo em escrita não é sobrecarregado com leitura.
     - Um banco intensivo em leitura não é sobrecarregado com escrita.
  
2. **Estrutura e Consistência**:
   - Dados podem ser armazenados em um banco relacional para garantir estrutura e consistência.
   - Consultas podem ser feitas em uma cópia otimizada dos dados, facilitando o acesso e a performance.

## Consultas Complexas
- A separação dos bancos de dados é especialmente útil quando:
  - Há necessidade de *queries complexas*.
  - Relatórios exigem consultas grandes e otimizadas.

### Tipos de Bancos de Dados
- Diferentes tipos de bancos podem ser utilizados para leitura:
  - Banco de dados orientado a documentos.
  - Banco de dados colunar.
  - Banco de dados gráfico.

## Desafios da Sincronização
- **Consistência Eventual**:
  - A separação pode levar a uma inconsistente eventual:
    - Os dados podem não estar atualizados entre os bancos de dados.
    - O tempo de sincronização pode variar (mesmo que em milissegundos).
  
- **Considerações**:
  - Se o sistema pode tolerar inconsistências, a separação é viável.
  - Se a consistência é crítica, é preferível usar um único banco de dados.

## Conclusão
- A decisão entre usar um ou dois bancos de dados deve ser baseada em:
  - Necessidades de performance.
  - Complexidade das consultas.
  - Tolerância a inconsistências.

Espero que este resumo tenha ajudado a entender as nuances do CQRS e a importância da escolha entre um ou dois bancos de dados em seu sistema!



---

## modulo_10_11671.mp4

# Resumo da Aula sobre CQRS e CQS

## Introdução ao CQRS
- **CQRS (Command Query Responsibility Segregation)**: Padrão arquitetural que separa as operações de leitura e escrita em um sistema.
- **DualWrite**: Técnica que permite que um sistema grave dados em dois bancos de dados simultaneamente.

## Estrutura do Sistema
### Camada de Comando
- **Banco de Dados de Escrita**: Utiliza um banco de dados relacional (SQL).
- **Banco de Dados de Leitura**: Utiliza o MongoDB.
- **Eventos**: Ao criar um produto, um evento é disparado e os dados são gravados em um banco de dados de leitura.

### Camada de Consulta
- **Objetivo**: Consultar dados, sem gravações ou regras de domínio.
- **Exemplo de Query**:
  - `findProduct`: Consulta ao banco de dados MongoDB.
  - Métodos:
    - `findAll()`: Retorna uma lista de produtos.
    - `findById(id)`: Retorna um produto específico pelo ID.

## Benefícios da Separação
- **Facilidade**: A separação das camadas facilita o desenvolvimento e a manutenção do sistema.
- **Comunicação Assíncrona**: A arquitetura é benéfica para microsserviços, onde as transações podem ser lidas independentemente das gravações.

## Desafios
- **Transações Sem Retorno**: A principal dificuldade é executar transações que não retornam dados.
- **Independência nas Leitura e Gravação**: Garantir que a leitura não dependa de gravação e vice-versa.

## Conceitos Relacionados
### CQS (Command Query Separation)
- **Definição**: Padrão que garante que comandos não retornem dados e que consultas não dependam de comandos.
- **Diferenciação**:
  - *CQRS*: Enfoque arquitetural abrangente.
  - *CQS*: Enfoque mais local e específico.

## Implementação Prática
- **Conexão com MongoDB**: Na parte de consulta, é criada uma conexão com o MongoDB para executar as queries.
- **Métodos de Especificação**:
  - A escrita pode ser feita através de um POST que retorna apenas o código HTTP, mantendo a lógica do CQRS.

## Conclusão
- **Separação de Comandos e Consultas**: É fundamental para a arquitetura do sistema.
- **Regras de Domínio**: Implementadas na camada de comandos, mas não na de consultas, permitindo consultas mais eficientes e organizadas.

## Dicas para Estudo
1. **Revisar os conceitos de CQRS e CQS**: Entender a diferença entre os dois padrões.
2. **Praticar Implementações**: Tentar implementar um exemplo simples de CQRS em um projeto.
3. **Refletir sobre Transações**: Pensar em como gerenciar transações que não retornam dados.

**Observação**: A abordagem que separa comandos e consultas ajuda a melhorar a performance e a escalabilidade do sistema.



---

## modulo_10_11672.mp4

# Resumo sobre CQRS e CQS

## Introdução
No vídeo anterior, discutimos a arquitetura CQRS (Command Query Responsibility Segregation) focando na camada de comandos e na implementação com bancos de dados relacionais e não relacionais.

## Estrutura de Dados
- **Banco de Dados de Escrita**: Utiliza SQL para gravar dados.
- **Banco de Dados de Leitura**: Utiliza MongoDB para consultas.
- **DualWrite**: Estratégia de gravar dados em dois bancos simultaneamente.

## Camadas da Arquitetura

### Camada de Comando
- **Função**: Gerenciar a criação e modificação de dados.
- **Eventos**: Quando um produto é criado, um evento é disparado.
- **Regras de Domínio**: A camada de comando contém regras de domínio e lógica de negócio.

### Camada de Consulta
- **Função**: Realizar apenas consultas sem gravações de dados.
- **Método `findProduct`**: Exemplo de uma consulta que busca produtos no MongoDB.
  - **`findAll`**: Retorna uma lista de todos os produtos.
  - **`findById`**: Retorna um produto específico pelo ID.
  
## Conceitos Importantes

### CQS (Command Query Separation)
- **Definição**: Princípio que garante que comandos não retornem dados e que consultas não dependam de comandos.
- **Diferença entre CQRS e CQS**:
  - **CQRS**: Abordagem arquitetural mais ampla.
  - **CQS**: Foco local em métodos específicos.

## Desafios na Implementação
- **Execução de Transações**: Importância de realizar transações sem retorno de dados.
- **Leitura Assíncrona**: Facilita a comunicação entre microsserviços.

## Conclusão
- A separação entre comandos e consultas simplifica a arquitetura da aplicação.
- Na camada de consulta, não é necessário implementar regras de domínio, permitindo consultas mais rápidas e eficientes.
- A implementação de CQRS proporciona um melhor desempenho com uma estrutura organizada para a consulta de dados.

## Observações Finais
- A conexão com o MongoDB é estabelecida para realizar as buscas de produtos.
- Em operações de escrita (como POST), o retorno é apenas o código HTTP, sem dados inseridos, alinhando-se ao princípio de CQRS. 

Com essa estrutura, é possível visualizar como a separação de comandos e consultas pode ser aplicada na construção de sistemas mais eficientes e escaláveis.



---

## modulo_10_11673.mp4

# Resumo sobre CQRS (Command Query Responsibility Segregation)

## Introdução
No vídeo anterior, foi discutido o conceito de CQRS, focando principalmente na camada de comandos e em como os dados são gerenciados utilizando bancos de dados distintos para escrita e leitura.

## Camada de Comando
- **Escrita de Dados:**
  - Ao criar um produto, os dados são gravados em um banco de dados relacional.
  - Após a gravação, um evento é disparado.
  - Esse evento é lido e os dados são gravados em um banco de dados de leitura (neste caso, o MongoDB).

- **DualWrite:**
  - O sistema grava em dois bancos de dados simultaneamente:
    - Banco de dados de escrita: SQL
    - Banco de dados de leitura: MongoDB

## Camada de Consulta (Query)
- **Propósito da Query:**
  - A camada de consulta serve apenas para consulta de dados, sem gravação ou regras de domínio.
  
- **Métodos de Consulta:**
  - `findProduct`: Método criado para buscar produtos no MongoDB.
    - **Estrutura do Produto:**
      - ID
      - Nome
      - Preço
  - `findAll`: Método que retorna todos os produtos em uma lista (slice).
  - `findById`: Método que retorna um produto específico baseado no ID.

## Vantagens da Separação de Camadas
- A separação entre comandos e consultas facilita a gestão e a manutenção da aplicação.
- As transações podem ser executadas sem retornar dados, permitindo uma leitura independente da gravação.

## Comunicação em Microsserviços
- A implementação de CQRS é benéfica para:
  - Comunicação assíncrona entre sistemas.
  - Melhoria na performance e na organização das consultas.

## CQS vs CQRS
- **CQS (Command Query Separation):**
  - Foca na separação de comandos e consultas em um nível mais local.
  - Garante que:
    - Escritas não retornem dados.
    - Leituras não dependam de gravações.

- **CQRS (Command Query Responsibility Segregation):**
  - Abordagem arquitetural que separa a lógica de comandos e consultas dentro da aplicação.

## Implementação com MongoDB
- Criação de uma conexão com o MongoDB para realizar consultas.
- O método POST, utilizado para escrita, retorna apenas o código HTTP, sem retornar os dados inseridos, conforme os princípios do CQRS.

## Conclusão
- A implementação de CQRS permite uma melhor organização e desempenho na aplicação.
- A camada de comandos contém regras de domínio, enquanto a camada de consultas é otimizada para performance.

---

Esses pontos são essenciais para entender como aplicar CQRS em suas aplicações e como isso pode beneficiar a arquitetura do sistema.



---

## modulo_10_11674.mp4

# Resumo da Aula sobre CQRS

## Introdução ao CQRS
- **CQRS**: Command Query Responsibility Segregation.
- O foco da aula foi na camada de **comando** e **consulta**.

## Camada de Comando
- Quando um produto é criado:
  - Dados são gravados em um **banco de dados relacional** (SQL).
  - Um **evento** é disparado.
  - O evento é lido e os dados são gravados em um **banco de leitura** (MongoDB).
- Utilização de **DualWrite**:
  - O mesmo sistema grava em dois bancos de dados simultaneamente.

### Funcionalidades da Camada de Comando
- Contém:
  - Regras de domínio.
  - Eventos.
  - Repositórios.

## Camada de Consulta
- A camada de consulta é responsável apenas por **consultas**:
  - Não realiza gravações de dados.
  - Não possui regras de domínio.
- Exemplo de Query criada: `findProduct`.
  - Utiliza o MongoDB para buscar produtos.
  - Métodos disponíveis:
    - **findAll**: Retorna uma lista de produtos.
    - **findById**: Retorna um produto específico pelo ID.

### Importância da Separação
- A separação entre comandos e consultas facilita a manutenção e o entendimento do sistema.
- Permite a execução de transações que não retornam dados.
- Lê transações independentemente de gravações.

## Comunicação e Microsserviços
- **Comunicação assíncrona** é benéfica para microsserviços.
- A gravação de dados não retorna informações, promovendo desacoplamento entre os componentes do sistema.

## CQS vs CQRS
- **CQS**: Command Query Separation.
  - Foca na separação local de comandos e consultas.
  - Garante que a escrita não retorne dados e que a leitura não dependa de escrita.
- **CQRS**: Foca na arquitetura da aplicação.
- Ambos promovem a estruturação eficiente do código.

## Conexão com o MongoDB
- Conexão estabelecida para realizar as operações de consulta.
- Exemplo de operações:
  - **GET**: Para buscar produtos.
  - **POST**: Para inserir produtos, que retorna apenas o código HTTP e não os dados inseridos.

## Conclusão
- A separação entre comandos e consultas é fundamental para a organização da aplicação.
- Na camada de comando, devem ser implementadas regras de domínio.
- Na camada de consulta, as regras não são necessárias, permitindo consultas mais eficientes e rápidas.

## Dicas para Estudo
- Revise os conceitos de **CQRS** e **CQS**.
- Pratique a implementação de comandos e consultas em um projeto de exemplo.
- Explore as vantagens de usar diferentes tipos de bancos de dados para escrita e leitura.

### Palavras-chave
- **CQRS**
- **CQS**
- **DualWrite**
- **MongoDB**
- **Comando**
- **Consulta**



---

## modulo_10_11678.mp4

# Módulo sobre Arquitetura Baseada em Microserviços

## Introdução
- **Boas-vindas**: O módulo é sobre arquitetura baseada em microserviços.
- **Expectativas**: Ajustes sobre o que será abordado durante o curso.

## Problemas Comuns em Microserviços
- Muitas arquiteturas em grandes empresas falham devido a:
  - **Falta de conceitos**: Desenvolvedores, tech leads e arquitetos não compreendem os fundamentos.
  - **Motivos errados para utilização**: Implementação sem entendimento adequado.

## Objetivos do Módulo
- **Fundamentos**: Apresentar os principais conceitos sobre microserviços.
- **Uso correto**: Quando utilizar e quando evitar a arquitetura de microserviços.
- **Minimização de riscos**: Estratégias para evitar falhas comuns.
- **Diferenças**:
  - *Coreografia* vs. *Orquestração* de microserviços.

## Estrutura do Módulo
- **Teoria vs. Prática**:
  - O módulo terá uma parte teórica importante, pois:
    - Microserviços são *pequenos sistemas* que se comunicam.
    - O desafio está em *compor* e *organizar* esses sistemas.

## Importância da Arquitetura de Microserviços
- Presença comum em grandes empresas.
- Necessidade de entender a implementação correta para evitar problemas.
- **Motivação**: Muitas empresas utilizam microserviços pelos motivos errados.

## Dicas para Implementação
- **Fundamentos a serem considerados**:
  - Compreensão dos conceitos por trás da arquitetura.
  - Estruturar a comunicação entre microserviços de maneira eficiente.
  - Avaliar se a adoção de microserviços faz sentido para a sua empresa.

## Conclusão
- O módulo é considerado um dos mais importantes do curso.
- Preparação para enfrentar obstáculos na implementação de microserviços.
- **Encerramento**: Preparar-se para aprender bastante ao longo do curso.

---

**Notas Finais**:
- Este módulo é essencial para quem deseja trabalhar com arquiteturas de microserviços.
- O entendimento teórico será crucial para a aplicação prática bem-sucedida.



---

## modulo_10_11679.mp4

# Módulo sobre Arquitetura Baseada em Micro-serviços

## Introdução
- Boas-vindas ao módulo.
- Ajuste de expectativas sobre o que será abordado.

## Importância dos Fundamentos
- Muitas arquiteturas de micro-serviços falham devido a:
  - Falta de compreensão dos conceitos fundamentais.
  - Implementação pelos motivos errados por parte dos desenvolvedores, tech leads e arquitetos.

## Objetivos do Módulo
Durante este módulo, você irá aprender sobre:

1. **Fundamentos da Arquitetura Baseada em Micro-serviços**:
   - Compreender os princípios básicos e conceitos.
  
2. **Quando Utilizar Micro-serviços**:
   - Situações apropriadas para a implementação.

3. **Quando Não Utilizar Micro-serviços**:
   - Cenários em que essa arquitetura pode não ser a melhor escolha.

4. **Funcionamento dos Micro-serviços**:
   - Como os pequenos sistemas se comunicam entre si.

5. **Minimizando Riscos**:
   - Estratégias para evitar falhas na implementação.
   - Evitar a "estrela da morte", um termo usado para descrever sistemas complexos e problemáticos.

6. **Coreografia vs. Orquestração**:
   - Diferenças entre esses dois métodos de gerenciamento de micro-serviços.

## Estrutura do Módulo
- Parte teórica é essencial para entender a composição e organização dos micro-serviços.
- Desenvolvimento de sistemas pequenos é simples, mas a complexidade está na integração e na lógica de negócios.

## Relevância no Mercado
- A arquitetura de micro-serviços é comum em grandes empresas.
- A necessidade de implementar essa arquitetura corretamente para evitar problemas recorrentes.

## Conclusão
- Este módulo é considerado um dos mais importantes do curso.
- Compreensão correta dos fundamentos é crucial para o sucesso na implementação de arquiteturas baseadas em micro-serviços.

## Dicas de Estudo
- **Revisar os conceitos básicos** sobre micro-serviços frequentemente.
- **Participar ativamente das discussões** e atividades propostas.
- **Praticar a aplicação dos conceitos** em projetos reais ou simulados.



---

## modulo_10_11680.mp4

# Módulo sobre Arquitetura Baseada em Microserviços

## Introdução
- **Bem-vindo ao módulo** sobre arquitetura baseada em microserviços.
- Importância de entender fundamentos para o sucesso na implementação.

## Expectativas do Módulo
- O foco será em conceitos e fundamentos que muitas vezes são negligenciados por desenvolvedores e arquitetos.
- **Objetivos principais**:
  - Compreender quando usar e quando não usar microserviços.
  - Aprender como os microserviços funcionam.
  - Minimizar riscos associados à arquitetura.
  - Evitar a "estrela da morte".
  - Diferenciar entre *coreografia* e *orquestração* de microserviços.

## Fundamentos da Arquitetura de Microserviços
- Microserviços são pequenos sistemas que se comunicam entre si.
- A simplicidade no desenvolvimento de sistemas pequenos.
- O desafio está na **composição** e **organização** desses sistemas.

## Importância do Módulo
- Este é um dos módulos mais importantes do curso.
- Relevância em empresas grandes que frequentemente utilizam microserviços.
- Muitas empresas adotam essa arquitetura por motivos errados.

## Dicas para Implementação de Microserviços
1. **Entenda os fundamentos**:
   - Compreensão sólida dos conceitos é crucial.
2. **Avalie a necessidade**:
   - Verifique se a arquitetura faz sentido para a sua empresa.
3. **Evite armadilhas comuns**:
   - Não caia na armadilha da "estrela da morte".
4. **Escolha entre coreografia e orquestração**:
   - Entenda as diferenças e aplicações de cada abordagem.

## Conclusão
- O módulo visa acelerar o aprendizado e evitar obstáculos na implementação de microserviços.
- Prepare-se para uma jornada rica em aprendizado sobre arquitetura baseada em microserviços.



---

## modulo_10_11764.mp4

# Resumo da Palestra sobre Desafios de Crescimento e Gestão de Estado

## Introdução
- A palestra aborda os problemas enfrentados por uma empresa em crescimento, especialmente relacionados à degradação da arquitetura de sistemas.
- Destaca a importância de manter a estabilidade e a eficiência operacional à medida que a empresa expande.

## Problemas Identificados

### Degradação da Arquitetura
- Após um crescimento acentuado, a arquitetura começou a falhar.
- Aumento nos erros e na redução da capacidade de processamento, comprometendo a estabilidade.

### Impacto nos Clientes
- Os problemas afetavam especialmente um grupo específico de clientes com alto valor comercial.
- Dificuldades em cumprir acordos comerciais devido à instabilidade do sistema.

### A Questão do Monolito
- A empresa enfrentava desafios ao tentar dividir um sistema monolítico em microserviços.
- Muitas iniciativas de refatoração não foram concluídas devido a mudanças de prioridade.

## Desenho da Arquitetura de Sistemas

### Fluxo de Transações
1. **Monolito**: Sistema central com um banco de dados grande.
2. **Serviço A**: Chamado via HTTP; validações e operações na base local.
3. **Serviço B**: Chamado via gRPC; processa eventos e atualiza a base core.
4. **Experiência do Cliente**: A transação só era concluída após a finalização do Serviço B.

### Problemas de Integração e Sincronização
- **Timeouts**: Problemas de propagação de erros entre os serviços.
- **Pooling**: Uso de *sleep pooling* resultou em bloqueio de processos, ocupando threads sem efetivamente consumir recursos.

## Desafios de Performance
- **Autoscaling**: A falha no autoscaling baseado em CPU não resolveu os problemas de capacidade durante picos de demanda.
- **Dificuldade de Identificação de Estado**: A falta de clareza sobre o estado das transações resultou em caos operacional.

## Diálogo com o CTO
- O CTO foi consultado para discutir a gestão de estado no sistema.
- **Solução Proposta**: Implementação do padrão *Saga* como uma possível solução para gerenciamento de transações.

### Desafios do Padrão Saga
- O padrão é frequentemente associado a e-commerces, mas a empresa tinha um fluxo de trabalho mais complexo.
- A expectativa dos clientes era por respostas síncronas, o que torna a adaptação do padrão um desafio.

## Conclusão
- A palestra destaca a complexidade do gerenciamento de sistemas em crescimento e a necessidade de soluções eficazes para garantir a estabilidade e a satisfação dos clientes.
- A discussão sobre o padrão *Saga* levanta questões sobre sua aplicabilidade em contextos que não sejam de e-commerce.

## Pontos para Revisão
- **Degradação da Arquitetura**: Como o crescimento acentuado impactou a infraestrutura.
- **Desafios de Integração**: Identificar problemas comuns entre microserviços.
- **Solução do Padrão Saga**: Avaliar a aplicabilidade e efetividade em diferentes cenários.

## Reflexões Finais
- A importância de uma comunicação clara e processos bem definidos durante a transição de um sistema monolítico para microserviços.
- Necessidade de adaptar soluções tradicionais às especificidades de cada negócio para garantir sucesso.



---

## modulo_10_11765.mp4

# Resumo da Palestra: Desafios de Crescimento e Gestão de Estado

## Introdução
- O crescimento da arquitetura de sistemas trouxe desafios significativos.
- A degradação da performance após um pico inicial resultou em problemas de estabilidade.

## Problemas Enfrentados
### Erros e Instabilidade
- Aumento de erros e problemas de processamento.
- Impacto maior em clientes com contratos comerciais significativos.
- Dificuldade em manter a estabilidade e cumprir acordos comerciais.

### Complexidade da Arquitetura
- Transição de um monolito para micro serviços não foi totalmente eficaz.
- A estratégia de micro serviços não foi concluída devido a mudanças de prioridade.

## Desafios Técnicos
### Comunicação entre Serviços
- Dependência forte do banco de dados core.
- Chamadas entre serviços A e B usando diferentes protocolos (HTTP e gRPC).
- Problemas de *timeout* e falta de propagação de erros.

### Sincronização e Estado
- Dificuldades na sincronização entre dados nas diversas bases.
- Contextos de chamadas que não eram propagados corretamente.
- O cliente frequentemente ficava sem informações sobre o estado da transação.

## Soluções Propostas
### Uso de Padrões
- Consideração do padrão *Saga* para gerenciamento de estados complexos.
- Desafios em aplicar conceitos de e-commerce a um sistema não e-commerce.

### Diálogo com o CTO
- Identificação das dificuldades de gestão de estado com a ajuda do CTO.
- Exploração de soluções para problemas de estado, sem se limitar aos exemplos tradicionais.

## Conclusões
- A gestão de estado é um desafio crítico em sistemas complexos.
- A transição para micro serviços precisa ser acompanhada por uma gestão adequada de estado para evitar problemas de performance e confiabilidade.
- O diálogo constante e a busca por soluções inovadoras são essenciais para resolver os problemas enfrentados.

## Pontos-Chave para Estudo
- **Crescimento de Arquitetura**: Entender as implicações do crescimento em sistemas complexos.
- **Estratégia de Micro Serviços**: Avaliar a eficácia da transição e o impacto na performance.
- **Gerenciamento de Estado**: Explorar padrões como o *Saga* e suas aplicações em sistemas não e-commerce.
- **Importância do Diálogo**: Enfatizar a comunicação entre a equipe técnica e a gestão para resolver problemas complexos.
- **Protocolos de Comunicação**: Compreender as vantagens e desvantagens de protocolos como HTTP e gRPC em sistemas distribuídos.

## Reflexões Finais
- A complexidade dos sistemas modernos exige uma abordagem cuidadosa para garantir a estabilidade e a performance.
- A flexibilidade e a capacidade de adaptação são fundamentais para resolver os desafios emergentes no desenvolvimento de software.



---

## modulo_10_11766.mp4

# Resumo da Aula sobre Desafios com CascadeDB

## Introdução
Nesta aula, discutiu-se os problemas enfrentados ao implementar o CascadeDB em um projeto utilizando microserviços e as limitações encontradas durante o processo.

## Problemas Iniciais
- **Expectativa vs. Realidade**: A equipe confiou que o CascadeDB resolveria todos os problemas, mas enfrentou dificuldades inesperadas.
- **Parceria com a Confluent**: A solução foi contratada para utilizar o CascadeDB, mas a equipe não era especialista na tecnologia.

## Limitações do CascadeDB
- **Limite de Query Tables**: O sistema permitia apenas 10 Query Tables por cluster, enquanto o design inicial incluía 30.
- **Estrutura de Microserviços**:
  - 10 microserviços criados, divididos em dois fluxos (5 em cada).
  - Cada microserviço tinha três tópicos, resultando em uma necessidade de 30 Table Views.

### Resolução de Limite
- **Chamada à Confluent**: A equipe abriu um chamado para entender o limite de 10, e foi informado que era um "soft limit", que poderia ser aumentado para 100.
- **Recomendações**: Para contornar as limitações, a Confluent sugeriu:
  - Criar mais de um cluster gráfico.
  - Limite de 10 clusters por conta.

## Estratégia de Contorno
- **Criação de um Fan-In**: 
  - Microserviço que ouve tópicos antes e escreve em um novo tópico.
  - Resultado: Redução para 3 Table Views (GSM-in, GSM-incompensate, GSM-error).
  
## Problemas de Desempenho
- **Degradação do Sistema**: Após consultas, o desempenho do CascadeDB começou a cair.
- **Tipo de Consultas**: 
  - O banco não era adequado para consultas específicas necessárias, como buscar erros em transações ou estados específicos.
  - O uso de IDs para consultas resultou em confusão pela falta de uma chave adequada na estrutura do banco.

## Rediscussão com SRE
- **Reavaliação da Base de Dados**: 
  - A equipe considerou se o CascadeDB era realmente a melhor opção para as necessidades do projeto.
  - Discussões focaram na gestão de dados transacionais para auditorias futuras e entendimento das transações.

## Motivação para QSQL
- **Necessidade de Microserviço**: A principal motivação para considerar a mudança para QSQL foi a eliminação da necessidade de criar um microserviço para ouvir tudo.

## Conclusão
A implementação do CascadeDB trouxe à tona a importância de entender as limitações tecnológicas e a necessidade de se adaptar às condições do sistema, além de reavaliar as soluções propostas para atender às demandas do projeto.

## Pontos-Chave para Estudo
- **Entender Limitações**: Conhecimento sobre limites de capacidade em bancos de dados.
- **Estratégias de Contorno**: Como implementar soluções alternativas em arquitetura de microserviços.
- **Desempenho e Consultas**: Importância de escolher a tecnologia certa para os tipos de consulta necessárias.
- **Gestão de Dados**: Necessidade de foco na gestão eficiente de dados transacionais.

**Dica de Estudo**: Revise os conceitos de microserviços e bancos de dados distribuídos para melhor compreensão das limitações e estratégias discutidas na aula.



---

## modulo_10_11767.mp4

# Resumo da Palestra sobre Desafios com CascadeDB

## Introdução
A palestra discute os desafios enfrentados ao implementar a solução CascadeDB, incluindo limitações de configuração e desempenho, além de estratégias para contornar esses problemas.

## Problemas Enfrentados
### 1. Limitação de Tabelas
- **Limite inicial**: CascadeDB permitia apenas **10 Query Tables** por cluster.
- **Desenho inicial**:
  - 10 microserviços com 3 tópicos cada, totalizando 30 Table Views.
- **Ação tomada**: 
  - Chamado à Confluent resultou em aumento do limite para **100** Table Views, mas ainda insuficiente.

### 2. Dificuldades de Consulta
- **Desempenho insatisfatório**: 
  - O CascadeDB não se mostrou adequado para consultas complexas requeridas.
  - Dificuldades em obter dados específicos, como estados de transações e erros.
- **Identificação de problemas**:
  - A estrutura do CascadeDB não permitia consultas eficientes sobre os dados.

## Estratégias de Contorno
### 1. Implementação de Fan-in
- **Criação de um microserviço**:
  - Um microserviço que ouve todos os tópicos e consolida mensagens em apenas três tópicos:
    - **GSM-in**
    - **GSM-incompensate**
    - **GSM-error**
- **Resultado**: 
  - Redução do número de Table Views para três, contornando a limitação inicial.

### 2. Redefinição da Estratégia de Dados
- **Reavaliação do uso do CascadeDB**: 
  - Discussões com a equipe SRE sobre a necessidade de um banco de dados mais adequado para consultas transacionais.
- **Motivação para mudar para QSQL**:
  - Eliminar a necessidade de um microserviço para ouvir todos os dados.

## Conclusões
- **Aprendizado**: 
  - A implementação de novas tecnologias requer uma análise cuidadosa das limitações e do desempenho, assim como um plano de contingência.
- **Próximos Passos**:
  - Continuação do rollout da solução, monitorando o desempenho e a adequação às necessidades do sistema.

## Pontos Chave para Revisão
- **Limitações do CascadeDB**: 10 vs. 100 Query Tables.
- **Desenvolvimento de soluções alternativas**: Fan-in como uma abordagem para contornar limitações.
- **Necessidade de um banco de dados mais flexível**: O caso para migrar para QSQL.

Esta estrutura fornece uma visão clara dos desafios enfrentados, das soluções implementadas e das conclusões tiradas durante o processo de desenvolvimento.



---

## modulo_10_11768.mp4

# Resumo da Aula sobre Desafios com CascadeDB

## Introdução
Nesta aula, discutimos as dificuldades enfrentadas ao trabalhar com o CascadeDB, uma solução contratada para gerenciar dados em um ambiente de microserviços. A apresentação abordou problemas inesperados e as soluções propostas pelos participantes.

## Problemas Identificados

### 1. Limitação de Query Tables
- **Limite Inicial**: O CascadeDB apresentou um limite de **10 Query Tables** por cluster.
- **Desenho Inicial**: 
  - Primeira versão tinha **10 microserviços**.
  - Cada microserviço continha **3 tópicos**, totalizando **30 Table Views**.
- **Suporte da Confluent**:
  - Após abrir um chamado, o limite foi aumentado para **100**, mas ainda assim insuficiente.
  - Discussões destacaram que o limite inicial não era um *hard limit*, mas um *soft limit*.

### 2. Degradação do Sistema
- **Consultas Ineficientes**: 
  - As consultas que precisavam ser feitas não eram adequadas para o CascadeDB.
  - Problemas ao obter informações como *status de transações* e *erros específicos*.
- **Estrutura de Dados**:
  - A estrutura de dados do CascadeDB não permitia uma identificação clara por ID, dificultando a busca.

## Estratégias Adotadas

### 1. Criação de um Fan-in
- **Solução**: Criar um microserviço que ouve tópicos e escreve em um único tópico.
- **Objetivo**: Reduzir o número de Table Views para **três** (GSM-in, GSM-incompensate, GSM-error).

### 2. Rediscussão com a SRE
- **Reavaliação da Estratégia**: 
  - Discutir a real necessidade do uso do CascadeDB.
  - Considerar a gestão de dados transacionais e a auditoria futura.

### 3. Alternativa ao CascadeDB
- **Motivação para QSQL**:
  - Evitar a criação de microserviços adicionais para ouvir todos os tópicos.
  - Focar em soluções que atendam melhor às necessidades de consultas complexas.

## Conclusão
A aula enfatizou a importância de entender as limitações de ferramentas de software e a necessidade de estratégias adaptativas em ambientes de microserviços. A comunicação com os fornecedores e a exploração de soluções alternativas são cruciais para o sucesso de implementações tecnológicas.

## Pontos Chave para Estudo
- Compreender os conceitos de *hard limit* e *soft limit* em bancos de dados.
- Analisar a arquitetura de microserviços e suas interações com soluções de armazenamento de dados.
- Avaliar a importância da estrutura de dados na eficiência de consultas e operações.
- Explorar alternativas tecnológicas que podem ser mais adequadas para necessidades específicas de negócio.

## Sugestões de Leitura
- Documentação do CascadeDB e Confluent.
- Práticas recomendadas para o design de microserviços e gestão de dados.
- Artigos sobre otimização de consultas em bancos de dados.



---

## modulo_10_11769.mp4

# Resumo da Palestra sobre Desafios com CascadeDB

## Introdução
- A palestra aborda os desafios enfrentados ao implementar o **CascadeDB** em um novo projeto.
- O foco principal é entender as limitações do sistema e como contorná-las.

## 1. Problemas Iniciais Encontrados
- A equipe confiou excessivamente que o **CascadeDB** resolveria todos os problemas.
- A parceria com a **Confluent** foi estabelecida para utilizar sua solução.

### 1.1 Limitação de Query Tables
- O **CascadeDB** tinha um limite inicial de **10 Query Tables** por cluster.
- O projeto original consistia em:
  - **10 microserviços**.
  - Cada microserviço com **3 tópicos**.
  - Totalizando **30 Table Views**.
  
### 1.2 Chamadas à Confluent
- Após abrir um chamado, a Confluent aumentou o limite para **100**, mas isso ainda não atendia às necessidades.
- A conversa com o suporte revelou que o limite era um **soft limit**, não um **hard limit**.

## 2. Testes e Descobertas
- Realizaram testes de carga, colocando **2.000 Table Views** em uma imagem Docker.
- Limitações foram observadas dentro do ecossistema da **Confluent**.

### 2.1 Estrategizando para Contornar Limitações
- Para contornar as limitações, foi criado um **fan-in**:
  - Um microserviço que ouvia todos os tópicos e escrevia em três tópicos: 
    - **GSM-in**
    - **GSM-incompensate**
    - **GSM-error**
  - Isso resultou na criação de apenas três **Table Views**.

## 3. Desempenho e Degradação
- O desempenho do sistema começou a degradar durante as consultas.
- O **CascadeDB** não era adequado para o tipo de consulta necessária.

### 3.1 Tipos de Consultas Problemáticas
- Consultas específicas não retornavam os resultados esperados:
  - Ex: "Me dá tudo que está com erro em tal passo."
  - Ex: "Me dá o estado dessa transação."

### 3.2 Estrutura de Dados
- O **CascadeDB** não conseguia organizar os dados corretamente.
- A ausência de uma chave única para as transações dificultava as consultas.

## 4. Rediscutindo a Estratégia
- A equipe revisou a necessidade de um banco de dados adequado para suas demandas.
- O foco estava nos dados transacionais, importantes para auditoria e análise futura.

### 4.1 Motivação para QSQL
- O principal motivador para considerar o **QSQL** foi a eliminação da necessidade de criar um microserviço para ouvir todas as transações.

## Conclusão
- O projeto enfrentou desafios significativos devido a limitações inesperadas do **CascadeDB**.
- A equipe precisou adaptar sua estratégia e considerar alternativas para garantir a eficiência e funcionalidade do sistema.



---

## modulo_10_11773.mp4

## Resumo da Aula sobre Configuração de Sagas

### Introdução
Nesta aula, o professor discute como configurar uma *saga* no contexto de microserviços, enfatizando a importância dos passos (steps) e da gestão de estado.

### O que é uma Saga?
- Uma *saga* é um padrão de gerenciamento de transações que permite coordenar múltiplas operações em microserviços.
- Cada *saga* é composta por uma sequência de passos que podem ser compensados em caso de falha.

### Estrutura de uma Saga
1. **Configuração de Passos**
   - Cada passo é definido dentro de uma estrutura chamada `saga step`.
   - Exemplo do passo 1: 
     - **Nome do passo**: `placeOrder`
     - **Tópico**: `placeOrder` (pode ser uma fila no RabbitMQ)
     - **Tipo de passo**: `step` ou `compensate`
     - **Status**: `pending`
     - **Dados**: Inicializados como bytes (pode ser JSON, protocol buffer, etc.)
     - **Tentativas de compensação**: Até 3 tentativas.

2. **Encadeamento de Passos**
   - **Passo 1**: Criar um pedido (`placeOrder`)
   - **Passo 2**: Gerar uma nota fiscal (`invoice`)
   - **Passo 3**: Remover o produto do estoque
   - **Passo 4**: Realizar a entrega
   - **Compensação**: Se um passo falhar, deve-se reverter os passos anteriores (ex: cancelar nota fiscal, reposicionar estoque).

### Inicialização de uma Nova Saga
- Para cada transação, uma nova *saga* é criada.
- Exemplo:
  - **Nome da saga**: `entrega` (opcional)
  - **Status**: `pending`
  - **Expiração**: 24 horas (se não resolvida, deve compensar).

### Controle de Versão
- É possível controlar a versão da *saga*, permitindo múltiplas versões da mesma.

### Execução da Saga
- Após a configuração, todos os passos são adicionados à *saga*.
- Um loop infinito pode ser utilizado para ler mensagens de uma fila.
- Cada transação inicia a *saga*, injetando dados iniciais.

### Gerenciamento de Estado
- Ao iniciar uma *saga*, um ID único é gerado e o estado é salvo em um banco de dados.
- Um log detalhado é mantido para auditoria e rastreamento de problemas.

### Importância do Event Sourcing
- O processo de *event sourcing* permite registrar cada evento ocorrido na *saga*.
- Se ocorrer um problema, é possível fazer um "replay" dos eventos para diagnosticar a falha.
- Fundamental para auditoria e compreensão do fluxo de dados.

### Conclusão
- A configuração de *sagas* em microserviços é fundamental para garantir a consistência e rastreabilidade das operações.
- No próximo vídeo, o professor abordará serviços disponíveis em provedores de nuvem, discutindo prós e contras.

### Próximos Passos
- Assistir ao próximo vídeo sobre serviços em provedores de nuvem e suas aplicações em microserviços.

### Dicas de Estudo
- **Revisar os conceitos de *sagas* e seus passos.**
- **Praticar a configuração de uma *saga* em um ambiente de desenvolvimento.**
- **Analisar casos de uso de *sagas* em diferentes cenários de microserviços.**



---

## modulo_10_11774.mp4

# Estudo sobre Sagas em Microserviços

## Introdução
Neste resumo, vamos explorar a configuração de *sagas* em microserviços, detalhando os passos necessários e os conceitos fundamentais abordados na palestra.

## O que é uma Saga?
Uma *saga* é um padrão de gerenciamento de transações distribuídas que permite o controle de operações em microserviços. Ela é composta por uma série de passos, conhecidos como *steps*, que são encadeados e podem ser compensados em caso de falhas.

## Passos da Configuração de uma Saga

### 1. Configuração dos Passos
- Cada saga é composta por múltiplos *steps*.
- Cada passo é definido em uma estrutura, como uma `struct` de *saga step*.
- Exemplo de configuração do passo:
  - **Nome do Passo**: `placeOrder`
  - **Tópico**: `placeOrder` (pode ser uma fila ou exchange, como RabbitMQ)
  - **Tipo de Passo**: 
    - `step` (ação normal)
    - `compensate` (para compensações)
  - **Status**: `pending` (pendente)
  - **Dados**: Podem ser em qualquer formato, como JSON ou protocol buffer.

### 2. Definição dos Passos da Saga
- **Passo 1**: Criar um pedido.
- **Passo 2**: Gerar uma nota fiscal (invoice).
- **Passo 3**: Remover o produto do estoque.
- **Passo 4**: Realizar a entrega.

### 3. Encadeamento de Passos
- Os passos dependem uns dos outros; por exemplo:
  - Se a entrega falhar, deve-se:
    - Repor o produto no estoque.
    - Cancelar a nota fiscal.
    - Mudar o status do pedido para cancelado.

### 4. Inicialização da Saga
- Cada transação cria uma nova saga:
  - **Nome da Saga**: `entrega` (opcional)
  - **Status**: `pending`
  - **Expiração**: 24 horas (se não resolvido, realiza compensação).

### 5. Controle de Versão
- As sagas podem ter múltiplas versões, permitindo que o sistema se adapte a mudanças na empresa.

## Execução da Saga
- Adição de todos os passos necessários.
- Utilização de um loop infinito para ler mensagens de uma fila.
- Cada transação que chega inicia a saga com os dados apropriados.

## Gerenciamento de Estado
- Ao iniciar a saga:
  - Gera um ID para a saga/transação.
  - Armazena o estado no banco de dados.
  - Processa cada etapa, registrando logs detalhados.
  
### Importância do Log
- Permite rastrear problemas:
  - Históricos de transações com problemas podem ser analisados.
  - Possibilidade de *replay* de eventos para entender falhas.

## Conclusão
- A configuração e o gerenciamento de sagas são essenciais para o funcionamento eficaz de microserviços.
- A abordagem permite um controle robusto sobre transações e facilita auditorias.

## Próximos Passos
- Na próxima apresentação, serão discutidos serviços de *saga* disponíveis em provedores de nuvem, incluindo prós e contras.

---

Esses pontos fornecem uma visão clara e concisa sobre a configuração e o funcionamento de sagas em microserviços, destacando a importância do gerenciamento de transações distribuídas.



---

## modulo_10_11775.mp4

# Estudo sobre Sagas em Microserviços

## Introdução às Sagas
- Sagas são uma forma de gerenciar transações em sistemas distribuídos.
- Elas são compostas por uma sequência de passos (steps) que são realizados em uma ordem específica.

## Estrutura de uma Saga
### Configuração dos Passos
1. **Passo 1: placeOrder**
   - Tipo: `step` (normal)
   - Status: `pending`
   - Dados: Inicialização com bytes (pode ser JSON, Protocol Buffer, etc.)
   - *Compensate retries*: Permite até 3 tentativas em caso de falha.

2. **Passo 2: Gerar Invoice**
   - Geração da nota fiscal.

3. **Passo 3: Remover Produto do Estoque**

4. **Passo 4: Realizar Entrega**
   - Se a entrega falhar, é necessário:
     - Reverter a remoção do produto do estoque.
     - Cancelar a nota fiscal.
     - Mudar o status da ordem para `cancelada`.

### Ciclo de Vida da Saga
- Cada transação gera uma nova saga.
- Exemplo: Nome da saga pode ser `entrega`, com status `pending` e expiração em 24 horas.
- Se não for resolvida em 24 horas, a saga é compensada.

## Controle de Versão da Saga
- É possível ter várias versões de uma mesma saga.
- Cada versão pode conter diferentes passos.

## Inicialização da Saga
- Para cada transação, um `init` é chamado, injetando dados iniciais.
- Um loop infinito lê mensagens de uma fila e inicia a saga baseada nos passos definidos.

## Gerenciamento de Estado
- O estado da saga é armazenado em um banco de dados.
- Cada passo é registrado, permitindo auditoria e rastreamento de problemas.
- Se ocorrer um erro, é possível fazer um *replay* dos eventos para investigar.

## Conclusão
- O gerenciamento de sagas é complexo, especialmente em relação a microserviços e operações de compensação.
- A estrutura e organização das sagas podem parecer simples, mas a implementação prática envolve desafios significativos.

## Próximos Passos
- No próximo vídeo, será abordado um serviço comum em provedores de nuvem relacionado a sagas, incluindo prós e contras.



---

## modulo_10_11776.mp4

# Estudo sobre Sagas em Microserviços

## Introdução
O conceito de *sagas* é fundamental para o gerenciamento de transações em sistemas de microserviços. Neste resumo, abordaremos a configuração de uma saga através de um exemplo prático, além dos passos e considerações importantes.

## O que são Sagas?
- Uma saga é uma sequência de transações que são realizadas em passos (steps).
- Cada passo pode depender do sucesso ou falha dos passos anteriores.

## Estrutura da Saga
### Passo 1: Configuração
- **Definição dos passos:** A configuração de uma saga começa pela definição dos seus passos.
- **Exemplo de Passo:** 
  - Nome: `placeOrder`
  - Tópico: `placeOrder` (pode ser uma fila ou uma exchange no RabbitMQ)
  - Tipo de passo: `step` (normal) ou `compensate` (para compensação)
  - Status: `pending` (pendente)
  - Dados: Inicializados como bytes (podem ser JSON, Protocol Buffers, etc.)
  - Tentativas de compensação: Exemplo de 3 tentativas.

### Passos subsequentes
1. **Geração de Invoice:**
   - Criação de uma nota fiscal.
2. **Remoção do Produto do Estoque:**
   - Atualização do estoque após a ordem.
3. **Entrega do Produto:**
   - Realização do envio para o cliente.

### Compensação
- Se ocorrer uma falha (ex: envio não realizado):
  - O produto deve ser colocado de volta no estoque.
  - A nota fiscal deve ser cancelada.
  - O status da ordem deve ser alterado para `cancelada`.

## Inicialização da Saga
- Cada transação gera uma nova saga.
- Exemplo:
  - Nome da saga: `entrega` (opcional)
  - Status: `pending`
  - Expiração: 24 horas (se não resolvida, deve compensar tudo).

## Controle de Versão
- É possível ter várias versões de uma mesma saga, permitindo adaptações ao longo do tempo.

## Execução da Saga
- **Início da Saga:**
  - O processo de *init* injeta os dados iniciais e inicia a operação.
- **Leitura de filas:**
  - Um loop infinito lê mensagens da fila e inicia a saga com os dados recebidos.

## Gerenciamento de Estado
- Cada *init* gera um ID para a saga/transação.
- O estado é armazenado em um banco de dados.
- É mantido um log detalhado do que acontece em cada etapa, permitindo auditoria e rastreamento de problemas.

## Importância do Event Sourcing
- O *event sourcing* permite visualizar cada evento que ocorreu durante a saga.
- Em caso de problemas, é possível fazer um replay dos eventos para entender o que ocorreu.

## Conclusão
- O gerenciamento de sagas é crucial em sistemas de microserviços para garantir a consistência das transações.
- A compreensão da estrutura e do funcionamento das sagas facilita o desenvolvimento de soluções eficientes.

## Próximos Passos
- No próximo vídeo, será apresentado um serviço disponível na maioria dos provedores de nuvem, incluindo prós e contras de seu uso.



---

## modulo_10_11777.mp4

# Resumo da Palestra sobre Desafios de Crescimento e Gestão de Estado em Arquitetura de Software

## Introdução
Durante a palestra, foi discutido um clássico problema de crescimento que afetou a arquitetura de um sistema de trading. A degradação do sistema após um pico de crescimento trouxe à tona diversos desafios, principalmente relacionados à estabilidade e capacidade de processamento.

## Problemas Identificados

### Degradação da Arquitetura
- Após um crescimento acentuado, a arquitetura começou a apresentar problemas.
- A capacidade de processamento foi reduzida, impactando a estabilidade do sistema.

### Impacto em Clientes Específicos
- Problemas afetaram um grupo específico de clientes com maior apetite e acordos comerciais.
- Dificuldades em cumprir acordos comerciais devido a falhas frequentes.

### Estrutura de Microserviços
- A transição de um monolito para microserviços não foi totalmente bem-sucedida.
- Problemas de refatoração e falta de conclusão de iniciativas.

## Desafios Técnicos

### Arquitetura Monolítica e Microserviços
- Dependência do monolito e seu banco de dados core.
- Interação entre serviços A e B via diferentes protocolos (HTTP e gRPC) causou complexidade.

### Problemas de Sincronização
- Dificuldades na sincronização entre o estado da base A e a base core.
- Timeout no serviço A não era corretamente propagado, levando a inconsistências.

### Comunicação Assíncrona
- Uso de sleep pooling para aguardar mudanças no banco de dados, bloqueando recursos e causando lentidão.
- Problemas de autoscaling baseados em CPU, que não ajudaram a resolver a questão.

## Dificuldades na Identificação de Estado
- Dificuldade em identificar o estado correto das transações.
- Caos na gestão do sistema, dificultando a prestação de compromissos de SLA (Service Level Agreement).

## Diálogo com o CTO
- O novo CTO trouxe uma nova perspectiva sobre a gestão do estado no sistema.
- A proposta de utilizar o padrão *Saga* para resolver problemas de gestão de estado.

## Reflexões sobre o Padrão Saga
- Padrão frequentemente utilizado em e-commerce, mas a aplicação no contexto apresentado foi questionada.
- A complexidade do sistema não se alinhava perfeitamente aos exemplos clássicos de carrinho de comércio.
- Discussão sobre a necessidade de soluções personalizadas para o sistema de trading.

## Conclusão
A palestra evidenciou a importância de uma gestão eficaz de estado em sistemas complexos, além de destacar a necessidade de adaptações nos padrões de arquitetura para atender às especificidades de cada negócio.

## Pontos de Estudo
- **Desafios de Crescimento**: Como a escalabilidade pode afetar a arquitetura de sistemas.
- **Microserviços vs Monolito**: Vantagens e desvantagens de cada abordagem.
- **Gestão de Estado**: Importância da gestão de estado e como o padrão Saga pode ser aplicado.
- **Protocolos de Comunicação**: Diferenças entre HTTP e gRPC e suas implicações.

## Tópicos para Discussão
- O que pode ser feito para melhorar a comunicação entre microserviços?
- Como gerenciar a complexidade em sistemas que exigem respostas síncronas?
- Quais outras abordagens além do padrão Saga podem ser consideradas para problemas de gestão de estado?



---

## modulo_10_11778.mp4

# Resumo da Palestra sobre Desafios de Crescimento em Arquitetura de Sistemas

## Introdução

Durante a palestra, foram discutidos os desafios enfrentados por uma empresa em crescimento, especialmente relacionados à degradação da arquitetura de sistemas e à gestão de estado em transações. O foco principal foi a transição de um monolito para uma arquitetura de microserviços e as dificuldades encontradas nesse processo.

## Problemas Identificados

### Degradação da Arquitetura
- A arquitetura começou a degenerar após um pico de crescimento.
- Problemas frequentes afetando a capacidade de processamento.
- A instabilidade impactou especialmente os clientes de alto valor.

### Questões de Sincronização
- A sincronia entre diferentes serviços e o banco de dados core não estava sendo mantida.
- Erros de timeout e problemas de comunicação entre serviços A e B.

### Experiência do Cliente
- A experiência do cliente foi prejudicada devido à espera por respostas em chamadas de API.
- O uso de *sleep pooling* para verificar o estado do banco de dados gerou ineficiências.

### Autoscaling e Desempenho
- O sistema enfrentou problemas de autoscaling, que não funcionaram adequadamente.
- A carga intensa de clientes resultou em erros 500 devido à falta de threads disponíveis.

## Estrutura de Comunicação entre Serviços

### Monolito e Microserviços
- A arquitetura inicial era baseada em um monolito, que interagia com os microserviços através de chamadas HTTP e gRPC.
- **Serviço A** e **Serviço B** tinham dependências fortes com o banco de dados core.

### Fluxo de Transação
1. O cliente inicia uma transação.
2. O sistema chama o **Serviço A**.
3. Se o **Serviço A** for bem-sucedido, chama o **Serviço B**.
4. O resultado final é retornado ao cliente, dependendo do processamento do **Serviço B**.

### Problemas de Comunicação
- Erros de comunicação e falta de clareza sobre o estado da transação.
- O cliente frequentemente ficava sem informações sobre o progresso da operação.

## Diagnóstico e Soluções Propostas

### Diálogo com o CTO
- O CTO, com vasta experiência, identificou a necessidade de uma gestão global de estado.
- A proposta de usar o padrão **Saga** foi considerada para resolver os problemas de sincronização.

### Desafios com o Padrão Saga
- A implementação do padrão Saga foi questionada, especialmente em relação à sua aplicação fora do contexto de e-commerce.
- O desafio de transformar operações assíncronas em uma experiência síncrona para o cliente foi destacado.

## Conclusões e Reflexões

- A transição para microserviços apresenta desafios significativos, incluindo a complexidade de manter a sincronia e a eficiência operacional.
- A necessidade de uma solução robusta para a gestão de estado e a comunicação entre serviços é essencial para melhorar a experiência do cliente.
- A discussão sobre a aplicabilidade do padrão Saga em contextos diferentes do e-commerce ressalta a importância de adaptar soluções para atender as necessidades específicas de cada negócio.

## Tópicos para Estudo

- **Arquitetura de Microserviços**: vantagens e desvantagens.
- **Design de APIs**: melhores práticas para comunicação entre serviços.
- **Gestão de Estado**: técnicas e padrões, incluindo o padrão Saga.
- **Desempenho e Escalabilidade**: como implementar autoscaling eficazmente.
- **Experiência do Cliente**: importância de uma comunicação clara e eficiente nas transações. 

## Palavras-Chave
- *Monolito*
- *Microserviços*
- *Saga*
- *Autoscaling*
- *Timeout*
- *Sleep Pooling*

