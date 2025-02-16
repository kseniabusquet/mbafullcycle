# Resumos dos vídeos

## modulo_11_12599.mp4

# Resumo da Aula sobre Kafka

## Apresentação
- **Instrutor:** Ronaldo Leguelas
- **Tema:** Produtores, consumidores, tópicos, partições e suas linguagens e drivers no Kafka.

## Conceitos Fundamentais

### Tópicos
- **Definição:** Unidade lógica no Kafka para dividir mensagens.
- **Analogia:** Semelhante a um **schema** em bancos de dados.
- **Partições:** 
  - Unidade física que armazena as mensagens.
  - Um tópico pode ter **milhares de partições**.
  - Importância para escalabilidade.

### Partições
- **Escalabilidade:** 
  - Para aumentar a vazão de consumo, é necessário ter mais partições.
- **Princípio FIFO:** 
  - *First In, First Out* — A primeira mensagem que chega é a primeira a sair.
- **Atributos de Mensagens:** 
  - **Valor:** Conteúdo da mensagem.
  - **Key:** Chave que identifica a mensagem.
  - **Header:** Informações adicionais (ex.: correlation ID, timestamp).

### Entrega de Mensagens
- **Partições e Hash:** 
  - A entrega é baseada no hash da key.
  - Mensagens com a mesma key são enviadas para a mesma partição.
- **Balanceamento:** 
  - Importante para evitar sobrecarga de partições.

### Redundância das Partições
- **Líder e Seguidor:**
  - Cada partição tem um broker líder e um ou mais seguidores.
  - Exemplo: Partição 0 tem broker 202 como líder e broker 203 como seguidor.
  - O Zookeeper gerencia o líder e o seguidor.

## Produtores
- **Função:** Responsável por produzir mensagens em uma partição de um tópico.
- **Propriedade ACK (Acknowledgment):**
  - **ACK 0:** 
    - Não recebe confirmação de gravação.
    - Risco de perda de mensagens (fire and forget).
  - **ACK 1:** 
    - Recebe confirmação de que a mensagem foi gravada no líder.
    - Não espera confirmação dos seguidores.

## Conclusão
- Entender esses conceitos é essencial para configurar e implementar soluções no Kafka de forma eficaz.
- **Próximas aulas:** Aprofundamento nas configurações e implementações.

### Dicas para Estudo
- **Revisar os conceitos de tópicos e partições** e suas funções.
- **Praticar a configuração de produtores e consumidores** no Kafka.
- **Experimentar com diferentes configurações de ACK** para entender como elas afetam a entrega de mensagens. 

### Glossário
- **Kafka:** Plataforma de streaming de dados.
- **Tópico:** Unidade lógica para mensagens.
- **Partição:** Unidade física que armazena mensagens.
- **Zookeeper:** Sistema que gerencia a configuração e a sincronização de serviços distribuídos.



---

## modulo_11_12600.mp4

# Resumo da Aula sobre Kafka por Ronaldo Leguelas

## Introdução
- **Apresentação**: Ronaldo Leguelas
- **Objetivo**: Explicar conceitos fundamentais do Kafka, incluindo *produtores*, *consumidores*, *tópicos*, *partições*, e suas linguagens e drivers.

## Conceitos Fundamentais

### Tópicos e Partições
- **Tópicos**: 
  - Unidades lógicas que dividem mensagens no Kafka.
  - Comparação: Tópico é como um *schema* em um banco de dados.
  
- **Partições**: 
  - Unidades físicas que armazenam as mensagens.
  - Exemplificação: Tópico = schema; Partições = tabelas.
  - Um tópico pode conter milhares de partições.
  
- **Escalabilidade**: 
  - Aumentar o número de partições melhora a *vazão* de consumo.
  
- **Princípio FIFO**: 
  - *First In First Out*: Primeira mensagem a entrar é a primeira a sair.

### Estrutura da Mensagem
- Cada mensagem em um tópico possui três atributos:
  - **Valor**: Conteúdo da mensagem.
  - **Key**: Chave que identifica a mensagem.
  - **Header**: Informações adicionais (ex: correlation ID, timestamp).

### Entrega de Mensagens
- As mensagens são entregues em partições baseadas na *hash* da key.
- Exemplo: Se a key for o CPF, mensagens com o mesmo CPF vão sempre para a mesma partição.
- Importância do balanceamento correto das partições e da key.

### Redundância das Partições
- Exemplo de partições em um tópico:
  - Partição 0 (líder: broker 202, seguidor: broker 203).
  - Partição 1 (líder: broker 203, seguidor: broker 202).
- O *Zookeeper* gerencia líderes e seguidores das partições.
- Redundância significa que, se um broker falhar, a mensagem ainda pode estar disponível em outro broker.

## Produtores
- **Definição**: Responsáveis por produzir mensagens em partições de um tópico.
- **Propriedade ACK**: 
  - Indica como o produtor quer receber confirmação da gravação da mensagem.
  
### Níveis de ACK
1. **ACK = 0**:
   - Não recebe confirmação.
   - *Fire and forget*: Mensagem pode ser perdida sem aviso.
   
2. **ACK = 1**:
   - Espera confirmação do líder da partição.
   - O produtor continua após receber confirmação do broker líder.

## Conclusão
- A compreensão dos conceitos de tópicos, partições, e a dinâmica de produtores é crucial para a configuração e implementação eficaz do Kafka em aplicações futuras.
- Em aulas posteriores, serão abordadas configurações mais avançadas e práticas para otimização do uso do Kafka.

### Observações Finais
- Fique atento ao balanceamento de partições para evitar sobrecarga em brokers.
- O conhecimento sobre ACK é fundamental para garantir a confiabilidade na entrega de mensagens.



---

## modulo_11_12601.mp4

# Estudo sobre Kafka - Aula com Ronaldo Leguelas

## Introdução
Nesta aula, Ronaldo Leguelas apresenta os conceitos fundamentais do Kafka, incluindo produtores, consumidores, tópicos, partições, e suas principais linguagens e drivers.

## Conceitos Básicos

### O que são Tópicos e Partições?
- **Tópicos**: 
  - Unidade lógica para dividir mensagens no Kafka.
  - Analogamente, o tópico é como um *schema* em um banco de dados.
  
- **Partições**:
  - Unidades físicas onde os dados são armazenados.
  - Analogamente, as partições são como *tabelas* dentro do schema.
  - Um tópico pode ter milhares de partições, garantindo escalabilidade.

### Princípio FIFO
- *First In First Out*:
  - A primeira mensagem que entra é a primeira a sair.
  - O consumidor começa sempre a consumir a partir da primeira mensagem (índice 0).

### Atributos da Mensagem
Cada mensagem possui três atributos:
1. **Valor**: Conteúdo da mensagem.
2. **Key**: Chave que identifica a mensagem.
3. **Header**: Informações adicionais (ex: correlation ID, timestamp).

### Entrega de Mensagens
- A entrega da mensagem é baseada na *hash* da key.
- Mensagens com a mesma key são sempre entregues na mesma partição.
- Importância do balanceamento correto das partições e das keys.

## Redundância das Partições
- As partições são redundantes:
  - Cada partição tem um *líder* e um ou mais *seguidores* (followers).
  - Exemplo:
    - Partição 0: Líder no broker 202, follower no broker 203.
    - Partição 1: Líder no broker 203, follower no broker 202.
- O *Zookeeper* gerencia quem é o líder e o seguidor.
- Se um broker falhar, a mensagem ainda pode estar disponível no broker seguidor.

## Produtores
- **Definição**: Responsável por produzir mensagens para as partições de um tópico.
- **Propriedade ACK**:
  - Define como e quando o produtor recebe confirmação (acknowledgment) da gravação da mensagem.
  - Três configurações:
    1. **ACK = 0**: Não recebe confirmação. (Fire and forget)
       - Risco de perda da mensagem.
    2. **ACK = 1**: Espera confirmação do líder.
       - O produtor espera que o líder confirme a gravação.

## Considerações Finais
- O entendimento dos conceitos de tópicos, partições e o funcionamento dos produtores e consumidores é crucial para a configuração e implementação eficaz do Kafka.
- A escalabilidade e a redundância são características fundamentais do design do Kafka, permitindo que ele suporte altas cargas de trabalho e assegure a disponibilidade de mensagens.

## Próximos Passos
- Avançar para aulas mais complexas sobre configuração e implementação no Kafka.
- Explorar outros aspectos como consumidores e suas interações com os tópicos e partições.



---

## modulo_11_12602.mp4

# Estudo sobre Estratégias de Commit-Seq

## Apresentação
Olá, meu nome é Rolando Manelas e nesta aula abordaremos as estratégias de *commit-seq* no contexto do Kafka. Vamos entender conceitos fundamentais como *offset*, *commit* e suas implicações no consumo de mensagens.

## O que é um Offset?
- **Definição**: Um *offset* é um número sequencial que identifica a posição de uma mensagem em um tópico ou partição.
- **Exemplo**:
  - Tópico A com partição 0:
    - Mensagem 0 -> Offset 0
    - Mensagem 1 -> Offset 1
    - Mensagem 2 -> Offset 2
- Cada mensagem tem um *offset* que incrementa à medida que novas mensagens são adicionadas.
- Importante: Não há duplicação de *offsets* dentro da mesma partição, mas diferentes partições podem ter o mesmo número de *offset*.

## O que é um Commit?
- **Definição**: O *commit* é uma marcação feita pelo *consumer group* indicando qual foi o último *offset* lido.
- **Funcionamento**:
  - O *consumer group* pode ter múltiplos consumidores (ex: Consumer A e Consumer B).
  - Cada consumidor grava sua marcação no *consumer offset*.
  - Exemplo:
    - Consumer A comita no *offset* 200.
    - Consumer B comita no *offset* 1.

### Armazenamento de Commit
- As informações de *commit* são gravadas no próprio Kafka, no tópico chamado *consumer offset*.

## Estratégias de Commit
### Auto-Commit
- **Definição**: O *auto-commit* é uma configuração padrão onde o *offset* é automaticamente comitado após a leitura da mensagem.
- **Vantagens**:
  - Alta performance em cenários onde a perda de mensagens não é crítica.
- **Desvantagens**:
  - Risco de perder mensagens se ocorrer um erro após o *commit*.
  
### Commit Manual
- **Definição**: O *commit manual* permite que o desenvolvedor controle quando o *offset* é comitado.
- **Funcionamento**:
  1. O consumidor lê a mensagem.
  2. Processa a mensagem (ex: tenta salvar em um banco de dados).
  3. Se o processamento for bem-sucedido, o *commit* é feito.
  4. Se ocorrer um erro, o *commit* não é realizado, permitindo que a mesma mensagem seja lida novamente.
- **Uso recomendado**: Em 99% dos casos, o *commit manual* é a melhor prática para evitar a perda de mensagens.

## Auto Offset Reset
- **Definição**: Configuração que determina o que acontece quando um novo *consumer group* é criado.
- **Modos de Leitura**:
  1. **Earliest**: Lê todas as mensagens desde o início do tópico.
  2. **Latest**: Começa a ler apenas novas mensagens que chegarem após a criação do *consumer group*.

## Conclusão
- A compreensão das estratégias de *commit-seq* é essencial para o manuseio eficiente de mensagens no Kafka.
- O uso correto de *offsets*, *commits* e a configuração do *auto offset reset* pode impactar significativamente a robustez e a performance da aplicação.

## Próximos Passos
- Na próxima aula, exploraremos exemplos práticos de *commit manual* e *auto-commit* no contexto do Kafka, além do funcionamento do *offset*.



---

## modulo_11_12603.mp4

# Estratégias de Commit-Seq

## Introdução
- Apresentação: Rolando Manelas.
- Tema: Estratégias de commit-seq.

## O que é um Offset?
- **Definição**: Um offset é um número sequencial que identifica a posição de uma mensagem em um tópico/partição.
- **Exemplo**:
  - Tópico A, Partição 0:
    - Mensagem 0: offset 0
    - Mensagem 1: offset 1
    - Mensagem 2: offset 2
  - Cada posição é um offset que incrementa conforme novas mensagens chegam.
  
- **Chaves e Valores**:
  - Exemplo de mensagem:
    - Chave: `hello`
    - Valor: `JSON`
    - Partição: 0
    - Offset: 2

- **Importante**:
  - Para uma mesma partição, **não há duplicação de offsets**.
  - É possível ter o mesmo offset em partições diferentes.

## O que é um Commit?
- **Definição**: O commit é uma marcação do último offset lido pelo *consumer group*.
- **Funcionamento**:
  - Exemplo com Tópico A, Partição 0:
    - Consumer A comita o offset 200, marcando que a última mensagem lida foi a 200.
    - Esta informação é gravada no tópico **consumer offset**.

## Como Funciona o Commit?
- **Auto-Commit**:
  - Habilitado por padrão em várias linguagens (Java, Golang, Python, .NET).
  - Ao receber uma mensagem (ex: offset 100), o commit é automático.
  - **Consequência**: Se ocorrer um erro após o commit, a mensagem será perdida, pois foi marcada como lida.

- **Manual Commit**:
  - Etapas de processamento:
    1. Receber a mensagem.
    2. Processar a mensagem (ex: salvar no banco).
    3. Se o processamento for bem-sucedido, então comitar.
  - **Vantagem**: Se ocorrer um erro, o Kafka reentregará a mesma mensagem, evitando perda.

## Estratégias de Commit
- **Auto-Commit**:
  - Rápido e eficiente, mas pode resultar em perda de mensagens.
  - Ideal para cenários onde a perda de mensagem não é crítica (ex: logs).

- **Manual Commit**:
  - Recomendado na maioria dos casos (99%).
  - Garante que mensagens não sejam perdidas durante o processamento.

## Auto Offset Reset
- **Definição**: Propriedade que determina como um novo *consumer group* lê mensagens.
- **Modos de Leitura**:
  1. **Earliest**: Lê todas as mensagens desde o início (offset 0 até o último offset).
  2. **Latest**: Lê apenas novas mensagens que chegarem após o início do *consumer group*.

## Conclusão
- O entendimento de offsets e commits é crucial para garantir a integridade do processamento de mensagens em sistemas que utilizam Kafka.
- A escolha entre auto-commit e manual commit deve ser feita com base nas necessidades do aplicativo e na criticidade da mensagem.

## Observações Finais
- Na prática, a escolha da estratégia de commit e a configuração do auto offset reset são essenciais para o desempenho e a confiabilidade da aplicação.
- A próxima aula abordará exemplos práticos de commit manual e automático.



---

## modulo_11_12604.mp4

# Estratégias de Commit-seq

## Introdução
- Apresentador: **Rolando Manelas**
- Tópico da Aula: **Estratégias de commit-seq**

## O que é um Offset?
- **Definição**: Um número sequencial que identifica a posição de uma mensagem em um tópico ou partição.
- **Exemplo**: 
  - Tópico A: Partição 0.
  - Mensagens:
    - Mensagem 0: Offset 0
    - Mensagem 1: Offset 1
    - Mensagem 2: Offset 2 (Exemplo: chave "hello", valor JSON)
- **Importante**:
  - O offset é único por partição; pode haver offsets iguais em partições diferentes.
  
## O que é um Commit?
- **Definição**: Uma marcação do último offset lido pelo *consumer group*.
- **Funcionamento**:
  - Cada *consumer* dentro de um *consumer group* registra seu último offset lido.
  - Exemplo: 
    - Consumer A: Commit no offset 200 na partição 0.
    - Consumer B: Commit no offset 1 na partição 0.
- **Armazenamento**: Informações de commit são registradas no tópico chamado **consumer offset**.

## Tipos de Commit
### Auto-commit
- **Definição**: O commit automático que é habilitado por padrão na maioria das linguagens (Java, Golang, Python, .NET).
- **Funcionamento**:
  - Quando uma mensagem é recebida, ela é automaticamente comitada.
  - Exemplo: Se uma mensagem com offset 100 é recebida e ocorre um erro durante o processamento, a mensagem é perdida.
- **Uso**: 
  - Útil em cenários onde a perda de mensagem é aceitável (ex: logs).
  - **Performance**: Rápido, mas arriscado.

### Commit Manual
- **Definição**: O commit é realizado manualmente após o processamento da mensagem.
- **Funcionamento**:
  - O consumidor recebe uma mensagem, processa, e só então comita se tudo ocorrer bem.
  - Se ocorrer um erro, a mensagem não é comitada, e o Kafka reentrega a mesma mensagem.
- **Importância**: 
  - Garante que mensagens não sejam perdidas durante o processamento.

## Auto Offset Reset
- **Definição**: Configuração que define como um novo *consumer group* deve ler mensagens.
- **Modos de Leitura**:
  1. **Earliest**: Lê todas as mensagens desde o início (offset 0 a 401, por exemplo).
  2. **Latest**: Lê apenas novas mensagens que chegarem após o início do *consumer group*.

## Conclusão
- O entendimento de offsets e commits é fundamental para o gerenciamento eficaz de mensagens em sistemas que utilizam Kafka.
- Na próxima parte da aula, será apresentado na prática como implementar tanto o commit manual quanto o auto-commit.



---

## modulo_11_12605.mp4

# Resumo da Aula: Estratégias de Commit-Seq

## Introdução
- **Apresentador**: Rolando Manelas
- **Tema**: Estratégias de *commit-seq* no Kafka

## Conceitos Fundamentais

### O que é um Offset?
- **Definição**: Um número sequencial que identifica a posição de uma mensagem em um tópico ou partição.
- **Exemplo**: 
  - Tópico A, Partição 0
    - Mensagem 0: Offset 0
    - Mensagem 1: Offset 1
    - Mensagem 2: Offset 2
- **Características**:
  - Cada posição é chamada de *offset* e incrementa conforme novas mensagens são adicionadas.
  - Um *offset* é único por partição (não há duplicação).

### O que é um Commit?
- **Definição**: Uma marcação que indica qual foi o último *offset* lido por um *consumer group*.
- **Funcionamento**:
  - Exemplo: 
    - Consumer A comita no offset 200.
    - Informações gravadas no tópico chamado *consumer offset*.
    - Se o Consumer B grava em outro offset (ex: 1), eles começam a ler a partir dessas posições.

## Tipos de Commit

### Auto-Commit
- **Definição**: O commit é realizado automaticamente ao receber uma mensagem.
- **Funcionamento**:
  - Quando uma mensagem é recebida (ex: offset 100), essa mensagem é automaticamente comitada.
  - Se ocorrer um erro durante o processamento, a mensagem é perdida.
- **Uso**:
  - Recomendado em cenários onde a perda de mensagem é aceitável (ex: logs).
  - É muito performático, mas não é ideal para a maioria dos casos.

### Commit Manual
- **Definição**: O commit é realizado manualmente após o processamento da mensagem.
- **Funcionamento**:
  - Após receber e processar a mensagem, o commit é feito somente se o processamento for bem-sucedido.
  - Se ocorrer um erro, a mensagem não é comitada, e o Kafka a reentregará.
- **Uso**:
  - Recomendado em 99% dos casos em que a perda de mensagens não é aceitável.

## Propriedades do Consumer

### Auto Offset Reset
- **Definição**: Configuração que determina o comportamento do consumer ao iniciar.
- **Modos de Leitura**:
  1. **Earliest**: Lê todas as mensagens desde o início (0 a 401).
  2. **Latest**: Lê apenas as novas mensagens a partir do momento em que o consumer inicia (ex: 402 em diante).
- **Importância**: Permite que novos *consumer groups* escolham como desejam processar as mensagens existentes.

## Conclusão
- **Próximos Passos**: A aplicação prática dos conceitos de commit manual e automático será abordada na seção *RedZone* da aula.

### Observações Finais
- Compreender as estratégias de commit é crucial para gerenciar eficientemente o consumo de mensagens no Kafka e evitar a perda de dados críticos.



---

## modulo_11_12606.mp4

# Estratégias de Produção de Mensagens no Kafka

## Introdução
Olá, meu nome é Ronaldo Laniaras e nesta apresentação, abordaremos as **estratégias de produção de mensagens** no Kafka. Essas estratégias podem ser aplicadas independentemente da linguagem de programação utilizada (Golang, Java, Python, Node, .NET, etc.).

## Tipos de Estratégias
Existem três principais estratégias de produção de mensagens em Kafka:

1. **At Most Once**
2. **At Least Once**
3. **Exactly Once**

Cada uma tem suas características e aplicações específicas.

---

## 1. At Most Once (At Most Once)
- **Definição**: Também conhecido como *Fire and Forget*, significa que o produtor não aguarda confirmação (ACK) do broker.
- **Uso Comum**: Ideal para situações onde a durabilidade da mensagem não é crítica, como gravação de logs.
- **Configuração**:
  - Configurar o ACK como zero (ACK = 0).
  - Indica que o produtor não quer receber nenhum tipo de retorno do broker.
- **Vantagens**:
  - **Alta Performance**: Não há latência causada pela espera por confirmação.
  - Útil quando:
    - Não se importa com a gravação da mensagem.
    - A performance é prioritária.

---

## 2. At Least Once (At Least Once)
- **Definição**: Garante que pelo menos uma mensagem será gravada no broker.
- **Importância do min-sync-replica**:
  - É uma propriedade importante que determina quantos brokers precisam replicar a mensagem antes que o ACK seja retornado.
- **Configuração**:
  - O valor de min-sync-replica deve ser ajustado conforme a necessidade de durabilidade.
- **Exemplo**:
  - Se você tem três brokers e configura min-sync-replica para três, mas o ACK para zero, o produtor não esperará confirmação.
  - Se o min-sync-replica for configurado para 2 e o ACK para all, o produtor aguardará confirmação de pelo menos dois brokers.
- **Confusão Comum**:
  - O ACK all não significa que se espera a confirmação de todos os brokers, mas sim dos brokers definidos pelo min-sync-replica.

---

## 3. Exactly Once (Exactly Once)
- **Definição**: Garante que a mensagem será gravada exatamente uma vez, evitando duplicações.
- **Funcionamento**:
  - Semelhante ao *At Least Once*, mas com um mecanismo de prevenção contra duplicidade.
- **Mecanismo de Prevenção**:
  - Utiliza a propriedade **Enable Idempotence** no produtor.
  - Quando uma mensagem é gravada sem um ACK, o produtor tenta reenviar a mensagem.
  - O broker verifica um identificador (ID) da mensagem para evitar gravações duplicadas.
- **Considerações**:
  - Adicionar idempotência pode aumentar a latência da produção, mas é aceitável na maioria dos casos.

---

## Considerações Finais
- **Escolha da Estratégia**: A escolha da estratégia depende da **necessidade de durabilidade** e da **performance** desejada.
- **Impacto da Idempotência**: Adicionar *idempotência* melhora a confiabilidade, mas pode impactar a performance.

## Resumo das Estratégias
- **At Most Once**: Alta performance, sem garantias de entrega.
- **At Least Once**: Garantia de entrega, com controle sobre a replicação.
- **Exactly Once**: Garantia de entrega única, com prevenção de duplicidade.

Essas estratégias são fundamentais para a utilização eficaz do Kafka em sistemas distribuídos e devem ser escolhidas de acordo com as exigências específicas de cada aplicação.



---

## modulo_11_12607.mp4

# Estratégias de Produção de Mensagens no Kafka

## Apresentação
- **Palestrante:** Ronaldo Laniaras
- **Tema:** Estratégias de produção de mensagens no Kafka

## Introdução
- O Kafka possui **três tipos de estratégias** de produção de mensagens, aplicáveis a qualquer produtor, independentemente da linguagem (Golang, Java, Python, Node, .NET).
  
## Tipos de Estratégias

### 1. At Most Once (File-and-Forget)
- **Definição:** Não há garantia de que a mensagem será gravada; o produtor não espera um retorno do broker.
- **Características:**
  - **Configuração:** `ACK = 0` (ou `ACK = None`)
  - **Uso Comum:** Gravação de logs, onde a durabilidade não é crítica.
  - **Vantagem:** Alta performance; ideal quando a latência é uma preocupação.
- **Desvantagens:**
  - Não é aplicável na maioria dos casos de uso do Kafka (95%).

### 2. At Least Once
- **Definição:** Garante que pelo menos uma mensagem será gravada no broker.
- **Configurações Importantes:**
  - **min-sync-replica:** Número mínimo de brokers que devem replicar a mensagem antes do retorno do `ACK`.
  - **Interação entre min-sync-replica e ACK:**
    - Se `ACK = 0`: O produtor ignora o `min-sync-replica`.
    - Se `ACK = all`: O produtor espera que todos os brokers definidos pelo `min-sync-replica` confirmem a gravação.
- **Exemplo Prático:**
  - Se existem três brokers e o `min-sync-replica` está configurado como 3, mas o `ACK` é 0, a mensagem pode não ser gravada em nenhum broker.

### 3. Exactly Once
- **Definição:** Semelhante ao At Least Once, mas garante que a mensagem não será duplicada.
- **Mecanismo de Prevenção de Duplicidade:**
  - **Configuração:** `Enable Idempotence = True`
  - **Como Funciona:** 
    - O broker atribui um ID único à mensagem.
    - Se o produtor tentar enviar a mesma mensagem novamente, o broker verifica se a mensagem já foi gravada usando o ID.
- **Considerações:**
  - A implementação de idempotência pode aumentar a latência da produção, afetando a performance.

## Considerações Finais
- É crucial entender a relação entre **ACK** e **min-sync-replica** para garantir a durabilidade e consistência das mensagens.
- A escolha da estratégia de produção deve levar em conta a necessidade de performance versus a necessidade de durabilidade das mensagens.
- A implementação de idempotência é recomendada em cenários onde a duplicação de mensagens é inaceitável, apesar do possível impacto na latência.

## Resumo das Configurações
- **At Most Once:**
  - `ACK = 0`
  - Alta performance, sem garantias de entrega
- **At Least Once:**
  - `ACK = all` ou `ACK = min-sync-replica`
  - Garante pelo menos uma entrega
- **Exactly Once:**
  - `Enable Idempotence = True`
  - Garante uma única entrega sem duplicação

## Dicas de Estudo
- Familiarize-se com os termos técnicos como `ACK`, `min-sync-replica`, e `Enable Idempotence`.
- Pratique exemplos práticos de cada estratégia em diferentes cenários de uso do Kafka.
- Considere o trade-off entre performance e durabilidade nas suas aplicações.



---

## modulo_11_12608.mp4

# Estratégias de Produção de Mensagens no Kafka

## Introdução
- Apresentador: **Ronaldo Laniaras**
- Tema: Estratégias de produção de mensagens no **Kafka**
- Importante para qualquer tipo de produtor: Golang, Java, Python, Node, .NET.

## Tipos de Estratégias de Produção
Existem três estratégias principais para garantir a entrega de mensagens no Kafka:

1. **At Most Once**
2. **At Least Once**
3. **Exactly Once**

### 1. At Most Once (Ao Menos Uma Vez)
- Também conhecido como **"Fire and Forget"**.
- **Definição**: O produtor envia a mensagem sem aguardar confirmação de entrega.
- **Uso Comum**: Ideal para loggings, onde não é crítico saber se a mensagem foi gravada.
- **Configuração**:
  - Configurar **ACK** como **zero** (ACK None).
  - **ACK**: A quantidade de confirmações que o produtor deseja do broker.
- **Vantagens**:
  - Alta performance.
  - Menos latência, pois não espera por respostas do broker.
- **Desvantagens**:
  - Não é recomendado para 95% dos casos de uso.

### 2. At Least Once (Pelo Menos Uma Vez)
- **Definição**: Garante que pelo menos uma mensagem será gravada no broker.
- **Conceitos Importantes**:
  - **min-sync-replica**: Número mínimo de brokers que devem replicar a mensagem antes de retornar o ACK.
- **Configuração**:
  - O ACK deve ser configurado conforme o valor do min-sync-replica.
  - Se **ACK** for configurado como **zero**, o min-sync-replica não tem efeito.
- **Exemplo**:
  - Se o min-sync-replica for 3 e o ACK for zero, o produtor não espera por confirmações.
  - Se o ACK for **all**, espera confirmações dos brokers definidos pelo min-sync-replica.

### 3. Exactly Once (Exatamente Uma Vez)
- **Definição**: Assegura que uma mensagem seja escrita apenas uma vez, mesmo em caso de falhas.
- **Semelhança com At Least Once**:
  - Utiliza **min-sync-replica** e **ACK all**.
- **Problema de Duplicidade**:
  - Em caso de timeout antes da confirmação, o produtor pode tentar enviar a mensagem novamente, resultando em duplicações.
- **Solução**:
  - Ativar a configuração **enable-idempotence-true**.
  - O broker verifica se a mensagem já foi gravada utilizando um ID único para cada mensagem.
- **Considerações**:
  - Habilitar a idempotência pode adicionar latência à produção.
  - Na maioria dos casos, essa penalidade de performance é mínima e aceitável.

## Conclusão
- As estratégias de produção de mensagens no Kafka são fundamentais para garantir a integridade e a eficiência da troca de dados.
- É importante escolher a estratégia adequada com base nas necessidades de durabilidade e performance.

## Dicas para Estudo
- **Entender** a diferença entre as três estratégias.
- **Praticar** a configuração dos parâmetros em um ambiente de desenvolvimento.
- **Refletir** sobre casos de uso reais e como cada estratégia se aplicaria.

### Referências
- Consulte a documentação oficial do Kafka para detalhes sobre configuração e otimização de produção de mensagens.



---

## modulo_11_12609.mp4

# Estratégias de Produção de Mensagens no Kafka

## Introdução
- Palestrante: **Ronaldo Laniaras**
- Tema: Estratégias de produção de mensagens utilizando o Kafka.
- Aplicação: Funciona em diversas linguagens como Golang, Java, Python, Node, .NET.

## Tipos de Estratégias de Produção
Existem três estratégias principais para a produção de mensagens no Kafka:

1. **At Most Once (At Most Once)**
2. **At Least Once (At Least Once)**
3. **Exactly Once (Exactly Once)**

## 1. At Most Once
- Também conhecido como **"Fire and Forget"**.
- Características:
  - O produtor não aguarda confirmação de entrega da mensagem.
  - Ideal para situações onde a durabilidade não é crítica, como registros de log.
- Configuração:
  - **ACK zero**: O produtor não espera nenhum retorno do broker.
- Vantagens:
  - Alta performance: Redução de latência, pois não há espera pela resposta do broker.
- Desvantagens:
  - Não é adequado para a maioria dos casos de uso no Kafka.

## 2. At Least Once
- Requisitos:
  - Pelo menos uma mensagem deve ser gravada no broker.
- Conceitos importantes:
  - **min-sync-replica**: Número mínimo de brokers que devem replicar a mensagem antes do ACK ser retornado.
- Configuração:
  - Se o **min-sync-replica** está configurado para 3 e o **ACK** para 0, o produtor ignorará a configuração do min-sync.
  - Usar **ACK all** ou **ACK -1** (dependendo da linguagem) garante que a mensagem foi gravada em pelo menos o número mínimo de brokers definidos no min-sync.
- Exemplo:
  - Se o min-sync-replica é 2 e o ACK é all, a mensagem deve ser gravada em pelo menos 2 brokers para ser considerada como entregue.

## 3. Exactly Once
- É semelhante ao At Least Once, mas evita a duplicação de mensagens.
- Problemas potenciais:
  - Se o produtor não recebe um ACK, ele pode tentar reenviar a mensagem, resultando em duplicação.
- Solução:
  - A propriedade **enable-idempotence=true** deve ser ativada no produtor.
    - Isso gera um ID único para cada mensagem, permitindo que o broker verifique se a mensagem já foi gravada.
- Considerações:
  - A adição de idempotência pode impactar a performance, aumentando a latência.
  - Na maioria dos casos, a latência adicional não é um problema, mas em cenários críticos, pode ser relevante.

## Considerações Finais
- **Desempenho vs. Durabilidade**: A escolha da estratégia deve considerar a necessidade de desempenho e a aceitação de perda de mensagens.
- **Configurações de ACK e min-sync-replica**: Entender estas configurações é crucial para implementar a estratégia de produção de mensagens que melhor se ajusta ao seu caso de uso.

## Resumo Visual
| Estratégia       | Descrição                                            | Configuração de ACK | Ideal para                 |
|------------------|-----------------------------------------------------|---------------------|-----------------------------|
| At Most Once     | "Fire and Forget", não aguarda confirmação         | ACK 0               | Logs, alta performance      |
| At Least Once    | Garante que pelo menos uma mensagem seja gravada    | ACK all ou -1      | Casos gerais de uso        |
| Exactly Once     | Garante entrega única de mensagens                   | ACK all + idempotência | Aplicações críticas        | 

## Dicas para Estudo
- **Revisar os conceitos** de ACK e min-sync-replica.
- **Praticar** a configuração em diferentes linguagens.
- **Analisar casos de uso** onde cada estratégia é mais apropriada.
- **Discutir as trade-offs** entre desempenho e durabilidade.



---

## modulo_11_12612.mp4

# Estudo sobre Kafka Connect com PostgreSQL

## Introdução
Nesta aula, Ronaldo Lanieras apresenta como usar o Kafka Connect para extrair dados de um banco de dados PostgreSQL e gravá-los em um tópico do Kafka.

## Preparação do Ambiente

### Docker Compose
- **Docker Compose** já foi criado na aula anterior com os serviços necessários.
- **Adição do PostgreSQL**:
  - Procurar e copiar a imagem do PostgreSQL do Docker Hub.

### Plugin JDBC
- Acesse o **Confluent Hub** para baixar o conector JDBC.
- Criar um diretório chamado `data/plugins` para armazenar os plugins.

## Configuração do PostgreSQL

### Criação do Banco de Dados
- Usar **DataGrip** para conectar ao PostgreSQL.
- Configuração:
  - **Usuário**: postgres
  - **Senha**: example
  - **Porta**: 5432 (configurar no Docker Compose).

### Criação da Tabela
- Criar uma tabela chamada `client` com os seguintes campos:
  - **id**: inteiro (chave primária)
  - **name**: varchar

## Configuração do Kafka Connect

### Subindo o Cluster
- Subir o cluster do Kafka Connect após a instalação do plugin.

### Criação do Conector JDBC
- Criar um conector JDBC que se comunica com a tabela `client`.
- Configurações do conector:
  - **Nome**: source JDBC postgrip
  - **Classe**: (não especificada no resumo)
  - **Tópico**: (não aplicável para conector source)
  - **Modo de Incremento**: baseado no ID (incrementing).
  - **Consulta**: (deixe o conector construir automaticamente).
  - **Intervalo de Polling**: 5 segundos.

## Operações com Dados

### Inserção de Dados
- Inserir registros na tabela `client`:
  - Exemplo: `INSERT INTO client (id, name) VALUES (1, 'Ronaldo')`
  
### Monitoramento do Conector
- Verificar o status do conector:
  - O conector deve estar em estado **running**.
- Usar **AKHQ** para visualizar o estado do conector.

## Tópicos do Kafka
- O Kafka Connect cria automaticamente tópicos:
  - **Tópicos de Configuração**: Armazena as configurações do conector.
  - **Tópicos de Offset**: Armazena o último ID lido (exemplo: se leu o ID 2, o próximo será 3).
  - **Tópicos de Status**: Mostra o estado do conector (ex: running).

## Conclusão
Ronaldo encerra a aula enfatizando o funcionamento do Kafka Connect com PostgreSQL e a importância do monitoramento das operações. Ele espera que os alunos tenham gostado e se despede.

## Dicas de Estudo
- **Pratique a instalação do Docker e do PostgreSQL**: Tente reproduzir o ambiente de aula.
- **Explore as configurações do conector JDBC**: Entenda cada parâmetro e sua importância.
- **Experimente inserir diferentes tipos de dados**: Veja como o Kafka processa essas informações.
- **Utilize ferramentas de monitoramento**: Familiarize-se com o AKHQ para acompanhar o estado dos conectores e tópicos.

## Referências
- **Docker Hub**: Para imagens de containers.
- **Confluent Hub**: Para plugins e conectores Kafka.
- **DataGrip**: Ferramenta de gerenciamento de banco de dados.



---

## modulo_11_12613.mp4

# Estudo sobre Kafka Connect e PostgreSQL

## Apresentação
- **Palestrante**: Ronaldo Lanieras
- **Tema**: Uso do Kafka Connect para extrair dados de um PostgreSQL e gravar em um tópico do Kafka.

## Objetivos da Aula
- Configurar um ambiente usando Docker Compose.
- Conectar um banco de dados PostgreSQL ao Kafka Connect.
- Criar e configurar um conector JDBC para transferir dados.

## Configuração do Ambiente

### Preparação do Docker Compose
- **Adicionar Serviço PostgreSQL**:
  - Buscar a imagem do PostgreSQL no Docker Hub.
  - Inserir no arquivo `docker-compose.yml`.

### Plugins Necessários
- **Plugin JDBC**:
  - Acessar o [Confluent Hub](https://www.confluent.io/hub/) para encontrar o conector JDBC.
  - Criar um diretório `data/plugins` e mover o plugin JDBC para esse diretório.

## Configuração do Banco de Dados

### Conexão ao PostgreSQL
- Utilizar o DataGrip para conectar ao PostgreSQL.
- Configurar a porta correta (5432) no Docker.

### Criação da Tabela
- Criar a tabela `client` com as colunas:
  - `id` (inteiro, chave primária)
  - `name` (varchar)

## Configuração do Conector JDBC

### Criar o Conector
1. Acessar a interface do Kafka Connect.
2. Definir as propriedades do conector:
   - **Nome**: `source JDBC postgrip`
   - **Classe do Conector**: classe específica do JDBC.
   - **Modo de Leitura**: modo incremental.
   - **Tabela a ser monitorada**: `client`.

### Propriedades Importantes
- **Connection URL**: usar a URL de conexão do DataGrip, substituindo `localhost` por `DB`.
- **Usuário e Senha**: configurar usuário `postgres` e senha `example`.
- **Coluna de Incremento**: usar `id` como coluna de incremento.

### Configurações Adicionais
- **Intervalo de Polling**: a cada 5 segundos.
- **Prefixo do Tópico**: configurar um prefixo para os tópicos gerados.

## Monitoramento do Conector
- Verificar status do conector:
  - Conector deve estar em estado "running".
  - Visualizar no AKHQ (interface gráfica do Kafka).

## Teste de Inserção de Dados
- Realizar um `INSERT` na tabela `client`:
  - Exemplo: `INSERT INTO client (id, name) VALUES (1, 'Ronaldo')`.
- Esperar a coleta e envio do dado para o Kafka.

## Tópicos de Controle do Kafka Connect
- **Tópicos Utilizados**:
  - `config`: armazena as configurações do conector.
  - `offset`: controla o último dado lido pelo conector.
  - `status`: informa o estado do conector.

## Conclusão
- O conector JDBC permite a leitura incremental de dados do PostgreSQL para o Kafka.
- O Kafka Connect utiliza tópicos específicos para controlar a configuração, offset e status dos conectores.
- A prática de inserção e monitoramento é crucial para garantir a funcionalidade e eficiência na transferência de dados.

## Próximos Passos
- Explorar mais sobre Kafka e outros conectores disponíveis.
- Testar diferentes modos de leitura e configurações de conectores.

## Recursos Adicionais
- [Documentação do Kafka Connect](https://kafka.apache.org/documentation/#connect)
- [Confluent Hub para Plugins](https://www.confluent.io/hub/)



---

## modulo_11_12614.mp4

# Estudo sobre Kafka Connect com PostgreSQL

## Apresentação
Olá, meu nome é **Ronaldo Lanieras** e nesta aula abordaremos como utilizar o **Kafka Connect** para extrair dados de um **PostgreSQL** e gravar esses dados em um tópico do Kafka.

## Estrutura Inicial
1. **Docker Compose**
   - Já temos um Docker Compose criado com os serviços necessários.
   - Adicionaremos o serviço do PostgreSQL.

2. **Busca pela Imagem do Postgre**
   - Acesse o **Docker Hub** para encontrar a imagem do PostgreSQL.
   - Copie o trecho necessário para o Docker Compose.

3. **Plugin JDBC**
   - Acesse o **Confluent Hub** e busque pelo plugin JDBC.
   - Crie um diretório chamado `data` e dentro dele, um diretório `plugins`.

## Configuração do Banco de Dados
- **Criando um Banco de Dados**
  - Usar o **DataGrip** para criar uma tabela chamada `client` com os seguintes campos:
    - ID (inteiro, chave primária)
    - Name (varchar)

- **Conexão com o Banco**
  - Verifique se o cluster está ativo e retorne a informação do `simplecluster`.

## Criação do Conector JDBC
1. **Criando o Conector**
   - Nome do conector: `source JDBC postgrip`
   - Configurações:
     - Classe: *JDBC*
     - Tipo de conversão: *string JSON*
     - Tópico: *Não aplicável para source*
     - Connection URL: Usar o URL do DataGrip, substituindo `localhost` pela rede do Docker (`DB`).
     - Tabela a observar: `client`
     - Modo: *incremental* (baseado no ID)
     - Intervalo de polling: *5 segundos*
     - Prefixo do tópico: `learning average`

2. **Configuração do Conector**
   - Após configurar, verifique o status do conector para garantir que está **running**.

## Testando o Conector
- **Inserindo Dados**
  - Execute um `INSERT` na tabela `client`:
    ```sql
    INSERT INTO client (ID, name) VALUES (1, 'Ronaldo');
    ```
  - Verifique se o conector captura a informação e a envia para o Kafka após alguns segundos.

- **Verificando Dados no Tópico**
  - Acesse o tópico gerado e observe o payload que inclui o ID e o nome.

## Controle e Monitoramento
- O Kafka Connect utiliza tópicos para controlar offset, configurações e status:
  - **Tópico de config**: guarda as configurações do conector.
  - **Tópico de offset**: registra o último dado lido pelo conector.
  - **Tópico de status**: indica o estado do conector (running ou não).

## Conclusão
Esta aula abordou a configuração do Kafka Connect com PostgreSQL, desde a criação do banco até a inserção de dados e a verificação do funcionamento do conector. Espero que tenham gostado e até a próxima!



---

## modulo_11_12615.mp4

# Estudo sobre Kafka Connect com PostgreSQL

## Introdução
Nesta aula, Ronaldo Lanieras apresenta como usar o **Kafka Connect** para extrair dados de um banco de dados **PostgreSQL** e gravar esses dados em um tópico do Kafka.

## Estrutura do Ambiente
1. **Docker Compose**: Utilizado para gerenciar os serviços necessários.
2. **PostgreSQL**: Adiciona um serviço de banco de dados PostgreSQL ao ambiente.
3. **Plugin JDBC**: Necessário para conectar o Kafka Connect ao PostgreSQL.

### Passos Iniciais
- Criar um diretório chamado `data` para armazenar os plugins.
- Criar um subdiretório `plugins` dentro de `data`.
- Baixar e extrair o plugin JDBC do Confluent Hub.

## Configuração do Ambiente
- **Subir o Cluster**: Iniciar o cluster do Kafka Connect.
- **Conectar ao PostgreSQL**: Utilizar uma ferramenta como o DataGrip para verificar a conexão com o PostgreSQL.

### Configuração do Banco de Dados
- **Criar Tabela**: Criar uma tabela chamada `client` com as colunas `id` (inteiro) e `name` (varchar).
- **Verificação**: Garantir que a tabela está acessível e retorna os dados corretamente.

## Configuração do Conector JDBC
1. **Criar o Conector**:
   - Nome: `source JDBC postgrip`
   - Classe: Definida pela configuração do plugin.
   - Tópico: Não é necessário, pois o conector irá determinar o tópico baseado no nome da tabela.

2. **Configurações Importantes**:
   - **Connection URL**: URL de conexão com o PostgreSQL.
   - **Modo de Leitura**: Usar modo **incremental** baseado no ID.
   - **Coluna de Incremento**: Definir a coluna de incremento (ID).
   - **Intervalo de Verificação**: O conector verifica a tabela a cada 5 segundos.

### Exemplo de Configuração
- **Tópico Prefixo**: `learning average`
- **Tipo de Tabela**: `table` (pode ser alterado para `view`).

## Execução e Monitoramento do Conector
- **Verificação de Status**: Confirmar se o conector está rodando através da interface gráfica ou via Postman.
- **Inserção de Dados**: Testar a inserção de dados na tabela `client` e observar como são refletidos no tópico do Kafka.

### Inserção de Dados
- Comando SQL para inserção:
  ```sql
  INSERT INTO client (id, name) VALUES (1, 'Ronaldo');
  ```
- Verificar os dados que foram enviados para o tópico Kafka após a inserção.

## Controle e Gerenciamento
- **Tópicos de Controle**: O Kafka Connect utiliza tópicos especiais para gerenciar configurações, offsets e status do conector.
- **Configurações no Tópico**: O tópico de configuração armazena todas as configurações do conector.
- **Offsets**: O tópico de offset registra o último ID lido, permitindo que o conector saiba qual é o próximo a ser processado.

## Conclusão
Ronaldo conclui a aula reiterando a importância do Kafka Connect e sua integração com o PostgreSQL. Ele incentiva a prática e exploração do conteúdo apresentado.

## Dicas de Estudo
- **Praticar**: Siga os passos da aula para configurar seu próprio ambiente Kafka Connect.
- **Explorar Documentação**: Leia a documentação oficial do Kafka Connect e do plugin JDBC para um entendimento mais profundo.
- **Realizar Experimentos**: Teste diferentes modos de leitura e configurações para ver como eles afetam a coleta de dados.



---

## modulo_11_12616.mp4

# Aula sobre o uso do esquema RESTRI em Golang

## Apresentação
- **Instrutor**: Ronaldo Lanieras
- **Objetivo**: Demonstrar na prática como utilizar o esquema RESTRI em Golang.

## Estrutura do Projeto
- O projeto utiliza **Docker Compose** com os seguintes componentes:
  - **Keeper**
  - **Broker**
  - **AKHQ**
  - **Esquema RESTRI** (imagem do Confluent)

### Configuração do Docker Compose
- O esquema RESTRI está na porta **8031**.
- O AKHQ necessita da configuração do esquema para desserializar mensagens corretamente.

## Produção e Consumo de Mensagens
### Tópico CLIENT
- Mensagens são armazenadas em um tópico chamado **CLIENT**.
- Mensagens são representadas em **JSON** e possuem um novo atributo chamado **SCHEMA**.
- O **SCHEMA** vincula a mensagem ao seu esquema definido, que no exemplo é em **Avro**.

### Versões do Esquema
- O esquema tem **duas versões**:
  - **Versão 1**: Sem o campo "cidade".
  - **Versão 2**: Com o campo "cidade".

### Subject
- O **Subject** é formado pela combinação do nome do tópico e um sufixo:
  - Para **value**: `tópico-value`
  - Para **key**: `tópico-key`
- O Subject é utilizado para aplicar o esquema ao value ou à chave da mensagem.

## Implementação em Golang
### Produção de Mensagens
1. **Criar um cliente** usando o pacote **Schema Register**.
   - URL do schema: `8031` (definido no Docker Compose).
2. **Criar um serializer** para serializar a mensagem.
   - O serializer pode ser configurado como **value** ou **key**.
3. **Serializar a mensagem**:
   - A mensagem é transformada em um **byte array** para ser enviada ao Kafka.

### Consumer
1. **Criar o consumer** e definir o client de schema, semelhante ao producer.
2. **Desserializar a mensagem** usando o método `deserializeInto`.
   - O consumer deve converter o **byte array** de volta para uma struct.

## Gerenciamento de Esquemas
- O produtor é responsável por:
  - Criar definições de esquema.
  - Adicionar ou remover campos.
  
- O consumidor utiliza o arquivo **Avro** fornecido pelo produtor para gerar suas structs em Golang.

### Ferramenta AvroGo
- **AvroGo** permite gerar structs automaticamente a partir do arquivo Avro.
- Gera funções necessárias para manipulação dos dados.

## Exemplificação Prática
- **Produção**: Mensagem é produzida e verificada no AKHQ.
- **Consumo**: Mensagem é consumida e desserializada corretamente, demonstrando a funcionalidade.

## Conclusão
- O uso do esquema RESTRI em Golang facilita a interoperabilidade entre produtor e consumidor, permitindo que aplicações diferentes se comuniquem sem necessidade de alterações frequentes no código, desde que o formato Avro seja respeitado.



---

## modulo_11_12825.mp4

# Aula sobre Schema RESTRI em Golang

## Introdução
- Apresentação do instrutor: **Ronaldo Lanieras**.
- Tema da aula: utilização do **schema RESTRI** em **Golang**.
- Estrutura da aula: produção e consumo de mensagens utilizando o schema.

## Configuração do Docker Compose
- **Componentes principais**:
  - Keeper
  - Broker
  - AKHQ
- **Novo componente**:
  - Schema RESTRI da Confluent na porta **8031**.
- Importância do Schema:
  - Necessário para a **desserialização** de mensagens no AKHQ.
  - Sem a configuração, as mensagens não serão legíveis.

## Estrutura das Mensagens
- Mensagens são enviadas em formato **JSON**.
- Atributo novo em mensagens: **SCHEMA**.
  - Direcionamento para o esquema definido (neste caso, **Avro**).
- Exemplo de versões do esquema:
  - **Versão 1**: sem campo "cidade".
  - **Versão 2**: inclui o campo "cidade".

## Subjects
- Definição de **Subject**:
  - Composição do nome do tópico + traço + value (ou key).
- Exemplo:
  - Para value: `tópico-value`.
  - Para key: `tópico-key`.
- **Tipo de esquema** e número de versões são exibidos no AKHQ.

## Produzindo Mensagens
### Configuração do Producer
1. Criar um produtor normal em Golang.
2. Criar um client usando o pacote **Schema Register**.
   - URL do schema: **8031**.
3. Criar um **serializer**:
   - Responsável por serializar a mensagem no formato desejado (neste caso, **Avro**).
   - Define se é um `value` ou `key`.

### Processo de Serialização
- Mensagens são convertidas em um **byte array**.
- O producer envia a mensagem serializada; o consumer desserializa para o formato utilizado (e.g., struct).

### Criação do Subject
- Normalmente feita de forma automática via código.
- Pode ser feita manualmente usando APIs do schema registry.

## Consumindo Mensagens
### Configuração do Consumer
1. Criar o consumer normalmente.
2. Definir o client de esquema.
3. Utilizar **deserialize** em vez de serialize.
4. Inscrever-se no tópico correspondente.

### Processo de Desserialização
- O consumer converte o byte array recebido em uma struct.
- O arquivo Avro gerado pelo producer é utilizado para gerar as structs necessárias.

## Demonstração Prática
1. Produção de uma mensagem:
   - Exibição de dados produzidos (nome, cidade, país).
2. Consumo da mensagem:
   - Verificação se a mensagem consumida é a mesma que foi produzida.

## Vantagens do Uso do Schema RESTRI
- Compartilhamento de contratos entre diferentes produtores e consumidores.
- Facilita a governança e a produtividade.
- Acesso a um portal de arquivos Avro para facilitar o consumo de contratos.

## Conclusão
- Expectativa de que os alunos tenham compreendido a importância do Schema RESTRI.
- Agradecimentos e convite para a próxima aula.



---

## modulo_11_12826.mp4

# Aula sobre o Esquema RESTRI em Golang

## Introdução
- **Palestrante:** Ronaldo Lanieras
- **Tema:** Utilização do esquema RESTRI em Golang.
- **Objetivo:** Demonstração prática de produção e consumo com o esquema RESTRI.

## Estrutura do Docker Compose
- **Componentes:**
  - Keeper
  - Broker
  - AKHQ
  - Esquema RESTRI (imagem da Confluent)
- **Configurações:**
  - Porta do esquema: 8.81
  - Dependência do Broker para funcionamento.
  - Necessidade de definir o esquema para desserialização de mensagens no AKHQ.

## Diferenças ao Usar o Esquema RESTRI
- Tópico criado: **CLIENT**
- Mensagem:
  - Formato: JSON
  - Novo atributo: **SCHEMA**
  - Visualização no AKHQ:
    - Acesso ao esquema Avro.
    - Definições de campos e versões do esquema.

## Compreensão do SUBJECT
- **Definição:** Combinação do nome do tópico, um traço (-) e um valor.
  - Exemplo: Para valor, é "nome do tópico-value".
  - Exemplo: Para chave, é "nome do tópico-key".
- **Flexibilidade:** Possibilidade de personalizar a criação do SUBJECT.

## Implementação do Código
### Produção de Mensagens
1. **Criação do Client:**
   - Uso do pacote Schema Register.
   - Definição da URL do esquema (8031).
2. **Serializer:**
   - Define como a mensagem será serializada (value ou key).
   - Conversão de mensagem para byte array.
3. **Criação do Subject:**
   - Normalmente feito automaticamente.
   - Possibilidade de criação manual via APIs.

### Consumo de Mensagens
1. **Criação do Consumer:**
   - Definição do client de esquema.
   - Utilização do método `deserialize`.
2. **Estruturas Geradas:**
   - Uso da ferramenta **Avro Go** para gerar structs a partir do arquivo Avro.
   - Propriedade do produtor sobre a definição do esquema.

## Vantagens do Uso do Esquema RESTRI
- **Facilidade de Compartilhamento:**
  - Contratos entre produtor e consumidor.
  - Atualizações de schema simplificadas.
- **Governança:**
  - Portais de arquivos Avro para compartilhamento de contratos.

## Conclusão
- O uso do **esquema RESTRI** em Golang proporciona uma abordagem organizada e eficiente para comunicação entre serviços, permitindo que produtores e consumidores operem de forma independente e com segurança em relação aos dados trocados.

## Dicas para Estudo
- Rever as configurações do Docker Compose.
- Praticar a criação e consumo de mensagens utilizando o esquema RESTRI.
- Experimentar a geração de structs com a ferramenta Avro Go.
- Discutir as vantagens e desvantagens do uso de esquemas em projetos reais.



---

## modulo_11_12906.mp4

# Resumo da Aula sobre Kafka - Ronaldo Leguelas

## Introdução
- Apresentação do tema: Produtores, consumidores, tópicos, partições e suas linguagens e drivers no Kafka.
- Objetivo: Fornecer uma visão geral dos conceitos para futuras aulas mais avançadas.

## Tópicos e Partições
### Definições
- **Tópicos**: Unidades lógicas que dividem mensagens no Kafka.
- **Partições**: Unidades físicas onde as mensagens são armazenadas.
  - Analogia: Tópico é como um *schema* e partições são como *tabelas* dentro do schema em um banco de dados.
  
### Características
- Um tópico pode ter milhares de partições.
- As partições garantem escalabilidade: para aumentar a vazão de consumo, é necessário ter mais partições.
- **FIFO** (First In First Out): A primeira mensagem a entrar é a primeira a sair.
  
### Atributos da Mensagem
Cada mensagem possui três atributos:
1. **Valor**: Conteúdo da mensagem.
2. **Key**: Chave que identifica a mensagem.
3. **Header**: Informações adicionais (ex: Correlation ID, Timestamp).

### Distribuição de Mensagens
- As mensagens são entregues fisicamente em uma partição, determinada pela *Hash* da Key.
- Importância do balanceamento correto das partições e da Key para evitar sobrecarga.

### Redundância das Partições
- Cada partição tem um **líder** e **seguidores** (followers), gerenciados pelo *Zookeeper*.
- Redundância: Se o broker líder cair, a mensagem ainda pode estar disponível no broker seguidor.

## Produtores
### Definição
- Responsáveis por produzir mensagens em uma partição de um tópico.

### Propriedade ACK (Acknowledgment)
Tipos de configuração de ACK:
1. **ACK 0**: Não recebe confirmação de que a mensagem foi gravada (fire and forget).
2. **ACK 1**: Recebe confirmação apenas do líder.
3. **ACK all**: Recebe confirmação de que todos os brokers gravaram a mensagem.

### Importância do ACK
- Entender a estratégia de ACK é crucial para avaliar se é aceitável perder mensagens.

## Consumidores
### Grupos de Consumidores
- Consumidores são distribuídos em *consumer groups*.
- Cada mensagem de uma partição é entregue a apenas um consumidor dentro do mesmo grupo.

### Exclusividade e Unicidade
- Mensagens são únicas dentro de um *consumer group*, mas podem ser replicadas em diferentes grupos.
- Importância de colocar todas as instâncias de uma aplicação no mesmo *consumer group* para garantir unicidade.

### Relação entre Partições e Consumidores
- Cada partição pode ser lida por apenas um consumidor de um mesmo grupo.
- Permite escalabilidade e eficiência na leitura das mensagens.

### Comitando Mensagens
- O ato de *comitar* significa informar ao Kafka que uma mensagem foi lida e não deve ser entregue novamente.
  
### Formas de Comitar
1. **At Most Once**: Comita antes do processamento. Pode perder mensagens.
2. **At Least Once**: Comita após o processamento. Aceita mensagens duplicadas.
3. **Exactly Once**: Comita após o processamento, garantindo que não haverá duplicatas. Requer lógica adicional para verificar se a mensagem já foi processada.

## Linguagens e Drivers
### Diversidade de Linguagens
- O Kafka suporta várias linguagens, incluindo Java, Golang, Python, .NET, Node.js, Scala, entre outras.
- Link para exemplos de como produzir e consumir mensagens em diferentes linguagens.

### Utilização da Biblioteca RD Kafka
- A maioria das linguagens utiliza uma biblioteca chamada *RD Kafka*, escrita em C, para comunicação com o Kafka.
- Importância de instalar a biblioteca de baixo nível para que os wrappers de alto nível funcionem corretamente.

## Conclusão
- Recapitulando: Entender a estrutura de tópicos, partições, produtores e consumidores é essencial para trabalhar com Kafka.
- Importância da configuração correta para garantir a eficiência e a integridade das mensagens.

### Próximos Passos
- Aprofundar-se nas configurações e práticas de implementação em aulas futuras.



---

## modulo_11_13097.mp4

# Aula Prática sobre o Esquema RESTRI em Golang

## Introdução
- Apresentador: **Ronaldo Lanieras**
- Tema: Utilização do esquema **RESTRI** em **Golang**.
- Objetivo: Demonstração prática de produção e consumo utilizando o esquema RESTRI.

## Estrutura do Docker Compose
- Composição:
  - **Keeper**
  - **Broker**
  - **AKHQ**
  - **Esquema RESTRI** (imagem da Confluent)
- Importância:
  - O esquema depende do Broker para funcionar.
  - Necessidade de especificar a localização do esquema RESTRI no AKHQ para desserialização de mensagens.

## Mensagens e Esquema
- Mensagens são enviadas em formato **JSON**.
- Novo atributo: **SCHEMA** adicionado às mensagens.
  - Direciona para o esquema definido (ex: **Avro**).
  - Versões do esquema:
    - Versão 1: não contém a cidade.
    - Versão 2: inclui a cidade.

## Entendendo o Subject
- Definição:
  - Composição do **Subject**: `nome do tópico - value` ou `nome do tópico - key`.
- Exemplo: 
  - Se o esquema for aplicado ao value, utiliza-se `value inside`.
  - Se for aplicado à chave, utiliza-se `key inside`.

## Produção de Mensagens
1. **Criação do Cliente**:
   - Usar o pacote **Schema Register**.
   - Especificar a URL do esquema (ex: `8031`).
2. **Serialização**:
   - Criar um **serializer** para converter mensagens no formato desejado (ex: Avro).
   - As mensagens são enviadas como **byte array**.
3. **Criação do Subject**:
   - Normalmente feita de forma automática, mas pode ser feita manualmente via API.

## Consumindo Mensagens
- O consumidor deve:
  1. **Criar o Consumer**: similar ao processo do produtor.
  2. **Deserializar**:
     - Usar `deserializeInto` para converter **byte array** de volta para a estrutura desejada.
- Estruturas geradas automaticamente a partir do arquivo **Avro**.

## Vantagens do Uso do Esquema RESTRI
- Compartilhamento do contrato entre produtores e consumidores.
- Facilita a atualização de contratos sem risco de erros manuais.
- Semelhança com sistemas como **SOAP** e **WSDL**.

## Demonstração Prática
1. Produzir uma mensagem:
   - Mensagem é criada e enviada.
2. Consumir a mensagem:
   - O consumidor lê a mensagem produzida.

## Conclusão
- Vantagens do uso de **Avro** e **Schema Registry**:
  - Compartilhamento eficiente de contratos.
  - Governança e produtividade nas aplicações.
- Agradecimento e encerramento.

---

### Dicas para Estudo
- Rever a estrutura do Docker Compose e suas dependências.
- Praticar a criação e a utilização de serializers e deserializers em Golang.
- Compreender bem a relação entre produtores e consumidores no contexto de *messaging*.
- Explorar mais sobre o uso de Avro e suas vantagens em sistemas distribuídos.



---

## modulo_11_13098.mp4

# Aula sobre Cacique ODB e Streaming com Kafka

## Introdução
- **Apresentador**: Ronaldo Laniellas
- **Objetivo**: Demonstrar como usar o *Cacique ODB* para criar um filtro baseado em tópicos existentes.

## Contexto
- Em aulas anteriores, foi criado um **Kafka Connect Source** que lê do PostgreSQL e grava em um tópico de clientes.
- Nesta aula, será criado um streaming para monitorar eventos de novos clientes e gerar uma **view materializada**.

## Conceitos Principais
- **Cacique ODB**: Um sistema separado do Kafka para gerenciar dados em streaming.
- **Streaming**: Processo de receber e processar dados continuamente.
- **View Materializada**: Estrutura que armazena resultados de consultas em uma tabela.

## Passos para Implementação

### 1. Preparação do Ambiente
- **Docker Compose**: Usar um ambiente já configurado com banco de dados e Kafka Connect.
- **Seção do Cacique**:
  - Configurar o servidor do Cacique e o CLI para execução de comandos.

### 2. Configuração do Kafka Connect
- Criar um conector JDBC que lê do PostgreSQL e grava no tópico.
- Confirmar que o Kafka Connect está funcionando corretamente.

### 3. Inserindo Dados
- Inserir um cliente chamado "Paul" para verificar se o Kafka Connect está funcionando.
  
### 4. Criando Streaming
- Acessar o CLI do Cacique e criar um novo streaming:
  - **Comando**: `create streaming clients_created`
  - **Colunas**: ID, nome, e tópico `lanielas.client` com formato JSON.

### 5. Consultas no Streaming
- **Push Query**: Utilizar `emit changes` para receber notificações de novos clientes.
- **Pull Query**: Consultar todos os registros sem notificações em tempo real.

### 6. Criando uma Tabela Baseada no Streaming
- Criar uma tabela chamada `last_clients` para agrupar dados por nome:
  - Utilizar `group by name` e funções de agregação como `latest by offset` para capturar o último ID e contagem.

### 7. Visualização dos Dados
- Acompanhar a criação do tópico `last_clients` no AKHQ.
- Inserir mais dados e observar as mudanças na contagem e no último ID.

### 8. Funções e Consultas Avançadas
- Possibilidade de criar outras tabelas e realizar operações adicionais, como manipulação de chaves e filtros.
- Referência à documentação do Cacique para explorar mais funções e operações.

## Considerações Finais
- Para visualizar tabelas e streams criados, utilizar:
  - **Comandos**: `show tables` e `show streams`.
- O Cacique ODB oferece uma ampla gama de funcionalidades para manipulação de dados em tempo real.

## Recursos Adicionais
- **Documentação do Cacique**: Disponível para consulta sobre funções e operações.
- **Revisão das Aulas Anteriores**: Importante para entender a configuração do Kafka Connect e o uso do conector JDBC.

---

Esperamos que este guia seja útil para sua compreensão e prática com o Cacique ODB e o Kafka!



---

## modulo_11_13099.mp4

# Aula sobre Cacique ODB e Streaming com Kafka Connect

## Apresentação
- **Instrutor:** Ronaldo Laniellas
- **Tema:** Uso do Cacique ODB para criar filtros e streaming baseado em tópicos do Kafka.

## Objetivos da Aula
- Criar um streaming que monitora eventos de clientes.
- Criar uma **view materializada** que conta quantas vezes um cliente foi registrado com o mesmo nome e qual foi o último ID atribuído.

## Contexto Prévio
- Em aulas anteriores, foi criado um **Kafka Connect Source** que lê dados de um banco de dados PostgreSQL e grava em um tópico de clientes.
- O foco agora é usar o **Cacique ODB** para processar esses dados.

## Passos para Implementação

### 1. Configuração Inicial
- **Docker Compose:** Iniciar o ambiente que inclui o banco de dados e Kafka Connect.
- **Adicionar Cacique ODB:** 
  - Copiar a seção de configuração do Cacique.
  - Ajustar a porta do broker.

### 2. Verificação do Kafka Connect
- Certificar-se de que o Kafka Connect está funcionando corretamente.
- **Conector JDBC:** Certificar-se de que o conector JDBC foi criado para ler do PostgreSQL.

### 3. Criação do Streaming
- **Comando para criar streaming:**
  ```sql
  CREATE STREAM clients_created (ID INT, name STRING) 
  WITH (KAFKA_TOPIC='lanielas.client', VALUE_FORMAT='JSON');
  ```
- **Execução do streaming:** Usar `SELECT` com `EMIT CHANGES` para receber notificações sobre novos registros.

### 4. Criação da View Materializada
- **Comando para criar a tabela:**
  ```sql
  CREATE TABLE last_clients AS 
  SELECT name, COUNT(*) AS quantidade, LATEST_BY_OFFSET(ID) AS last_id 
  FROM clients_created 
  GROUP BY name;
  ```
- **Funções de Agregação:** Utilizar funções como `LATEST_BY_OFFSET` para manter apenas os dados mais recentes.

### 5. Testes e Inserções
- Realizar **inserts** na tabela de clientes para verificar o funcionamento do streaming e da view materializada.
- **Verificação no AKHQ:** Confirmar a criação do tópico `last_clients` e a atualização dos dados.

## Observações Finais
- A view materializada contabiliza a quantidade de vezes que um nome de cliente é registrado e o último ID associado.
- O sistema permite fazer streaming e tabelas com filtros e funções de agregação.
- A documentação do Cacique ODB é rica e fornece detalhes sobre as funções disponíveis.

## Recursos Adicionais
- **Documentação do Cacique:** Explorar as funções de tabela e streaming disponíveis.
- **Kafka Connect:** Revisar como criar conectores JDBC e trabalhar com tópicos.

## Conclusão
- O uso do Cacique ODB junto com Kafka Connect permite a criação de soluções eficientes para monitorar e processar dados em tempo real.
- A prática com comandos e a verificação dos resultados são fundamentais para entender o funcionamento do sistema. 

Espero que essa aula tenha sido útil! Até a próxima!



---

## modulo_11_13100.mp4

# Resumo da Aula sobre Cacique ODB

## Introdução
- Palestrante: **Ronaldo Laniellas**
- Tema: Uso do **Cacique ODB** para criar filtros em tópicos existentes.

## Contexto
- Nas aulas anteriores, foi criado um **Kafka Connect Source** que lê dados do **PostgreSQL** e grava em um tópico de clientes.
- Nesta aula, o objetivo é:
  - Criar um streaming que captura eventos de novos clientes.
  - Criar uma **view materializada** para contar quantas vezes um cliente foi criado com o mesmo nome e qual é o último ID.

## Estrutura da Aula

### 1. Preparativos
- Acessar o **Docker Compose** já configurado, que contém:
  - Banco de dados
  - Kafka Connect
- Adicionar a seção do Cacique no Docker Compose:
  - Configuração do servidor Cacique e CLI.

### 2. Configuração do Cacique
- Modificar a porta do broker.
- Executar `Docker Compose up` para iniciar os serviços.
- Confirmar se o cluster de Kafka Connect está funcionando corretamente.

### 3. Criação do Streaming
- Criar um streaming chamado **clients created**:
  - Campos: ID e nome.
  - Tópico de origem: `lanielas.client`.
  - Formato do valor: JSON.

### 4. Consultas em Streaming
- Consultas em streaming:
  - **Push Query**: Notifica eventos novos.
  - **Pull Query**: Retorna todos os registros atuais sem notificações.

### 5. Criação da Tabela
- Criar uma tabela chamada **last clients**:
  - Baseada no streaming **clients created**.
  - Utilizar `GROUP BY` para contar repetições de nomes.
  - Usar a função de agregação **latest by offset** para pegar o último ID.

### 6. Exemplo Prático
- Inserir novos clientes na base de dados e observar o comportamento:
  - Exemplo com clientes: Ronaldo e Paul.
  - Monitorar atualizações na view materializada.

### 7. Visualização e Testes
- Usar **AKHQ** para visualizar tópicos e consumidores.
- Testar inserções e verificar se a contagem e o último ID estão corretos.
- Comprovar que a tabela e o tópico foram criados corretamente.

## Funcionalidades Adicionais
- O Cacique possui diversas funções de agregação que podem ser usadas em views materializadas.
- Possibilidade de criar múltiplos streamings e tabelas, aplicando filtros e transformações.

## Documentação
- A documentação do Cacique é rica e fornece informações detalhadas sobre:
  - Funções disponíveis
  - Exemplos de uso e aplicações.

## Conclusão
- O Cacique ODB permite uma manipulação avançada de dados em streaming, agregando e contando informações de maneira eficiente.
- É importante praticar e explorar a documentação para aprofundar o conhecimento.

## Próximos Passos
- Revisar as seções anteriores sobre Kafka Connect para garantir a compreensão do fluxo de dados.
- Experimentar com outras configurações e funcionalidades do Cacique ODB.



---

## modulo_11_13101.mp4

# Configuração de Kafka Broker em Produção

## Introdução
Nesta aula, Ronaldo Lanielas discute as melhores práticas para configurar um Kafka Broker em ambiente de produção, abordando preocupações relevantes e propriedades essenciais a serem consideradas.

## Principais Temas Abordados

### Governança de Tópicos
- **Autocriação de Tópicos**: 
  - **Recomendação**: Não permitir a autocriação de tópicos.
  - **Motivo**: Evitar a criação de tópicos com nomes errados por aplicações novas, o que pode causar desorganização.
  - **Estratégia**: 
    - Criar tópicos de forma manual ou via pipeline.
    - Disponibilizar tópicos para produtores e consumidores, mantendo a governança.

### Compressão de Mensagens
- **Compressão**: 
  - **Métodos**: Permitir que o produtor escolha a compressão pode não ser eficaz em empresas grandes.
  - **Recomendação**: Configurar a compressão para *LZ4*, garantindo que todas as mensagens sejam comprimidas independentemente da configuração do produtor.

### Retenção de Mensagens
- **Política de Retenção**: 
  - **Configuração Padrão**: 7 dias.
  - **Recomendação**: Avaliar a necessidade de retenção; 2 a 3 dias costumam ser suficientes.
  - **Importância**: Monitorar e alertar sobre a aplicação, principalmente se estiver parada por longos períodos.

### Tamanho Máximo de Mensagens
- **Tamanho Padrão**: 1 MB.
- **Recomendação**: Reduzir o tamanho máximo para 10 KB.
  - **Justificativa**: Reduzir a quantidade de dados trafegados, ajudando na performance e no uso de banda.
  - **Análise**: Verificar se o payload maior é realmente necessário; considerar trafegar apenas IDs.

### Configuração do Binsync Replica
- **Replica Factor**: Importante para garantir que as mensagens sejam replicadas em múltiplos nós.
- **ACK do Produtor**: 
  - **Configuração**: Permitir que o produtor receba confirmação após replicar para pelo menos 2 brokers, aumentando a performance.
  - **Risco**: Existe a possibilidade de perda de mensagem se os brokers 1 e 2 falharem antes do 3 receber a mensagem.
  - **Recomendação**: Para mensagens críticas, considerar a configuração para 3.

## Considerações Finais
- **Importância das Propriedades**: 
  - A configuração do broker de produção deve ser feita com atenção às propriedades discutidas.
  - As variáveis de configuração, como broker ID, permanecem constantes, mas as propriedades adicionais são cruciais para garantir a performance e a segurança dos dados.

## Conclusão
A configuração de um Kafka Broker em produção requer atenção a diversas propriedades que impactam diretamente a governança, compressão, retenção e performance. É essencial personalizar essas configurações de acordo com as necessidades específicas de cada aplicação.



---

## modulo_11_13103.mp4

# Configuração de Kafka Broker em Produção

## Introdução
Nesta aula, Ronaldo Lanielas discute a configuração de um Kafka Broker em ambiente de produção, destacando preocupações e melhores práticas.

## Relembrando a Aula Anterior
- Cálculo de TPS (transações por segundo)
- Tamanho de disco
- Memória e CPU
- Testes de performance

## Propriedades Importantes para Configuração

### 1. **Autocriação de Tópicos**
- **Recomendação**: Não permitir a autocriação de tópicos.
- **Justificativa**:
  - Previne a criação inadvertida de tópicos com nomes incorretos.
  - Mantém uma governança sobre os tópicos criados.
  - Evita surpresas com a criação de milhares de tópicos sem sentido.
  - Protege contra loops infinitos que podem afetar o broker.

### 2. **Compressão de Mensagens**
- **Opção de Compressão**: Forçar o uso de LZ4.
- **Motivos**:
  - Muitas empresas não utilizam a compressão por falta de conhecimento.
  - LZ4 é uma das melhores opções de compressão disponíveis.
  - Garante que todas as mensagens sejam comprimidas, independentemente da configuração do produtor.

### 3. **Retenção de Mensagens**
- **Propriedade**: `retention.hours`
- **Configuração Padrão**: 7 dias, porém:
  - Em muitos casos, 2 a 3 dias são suficientes.
  - Avaliar a necessidade de retenção com base na arquitetura da aplicação.

### 4. **Tamanho Máximo da Mensagem**
- **Configuração Padrão**: 1 MB (megabyte)
- **Recomendação**: Reduzir para 10 KB.
- **Justificativa**:
  - Mensagens de 1 MB podem ser excessivas.
  - Avaliar se o payload deve ser enviado via Kafka ou se apenas um ID deve ser trafegado.

### 5. **Mínimo de Réplicas (MinInSyncReplicas)**
- **Função**: Define o número mínimo de réplicas que devem receber a mensagem antes que o produtor receba um ACK.
- **Configuração Comum**: 2 réplicas.
- **Considerações**:
  - Aumenta a performance ao não esperar pela réplica de todos os brokers.
  - Pode haver risco de perda de mensagem se as réplicas não forem bem geridas.

## Conclusão
- A configuração de um Kafka Broker em produção exige atenção a várias propriedades.
- A abordagem deve ser adaptada conforme a carga de trabalho e requisitos de performance.
- O processo de configuração é semelhante ao discutido nas aulas anteriores, mas deve incluir essas considerações adicionais.

## Dicas Finais
- **Monitoramento**: Implementar monitoria e alertas para identificar problemas rapidamente.
- **Validação de Configurações**: Sempre revisar e ajustar as configurações com base na performance observada.
- **Documentação**: Manter uma documentação atualizada das configurações e práticas recomendadas.

## Próximos Passos
- Aplicar o que foi aprendido em um ambiente de teste.
- Realizar simulações para entender o impacto das configurações no desempenho do Kafka Broker.



---

## modulo_11_13104.mp4

# Configuração de Kafka Broker em Produção

## Apresentação
Olá, meu nome é Ronaldo Lanielas e nesta aula discutiremos como configurar um Kafka Broker em produção e as principais preocupações a serem consideradas.

## Revisão de Conceitos Anteriores
- Na aula passada, abordamos temas como:
  - Cálculo de TPS (transações por segundo)
  - Tamanho do disco
  - Memória e CPU
  - Testes de performance
  - Propriedades de configuração do Kafka

## Considerações sobre a Configuração do Kafka

### Governança de Tópicos
- **Desativar a Autocriação de Tópicos**
  - **Motivo**: Permitir a criação automática pode resultar em tópicos com nomes incorretos.
  - **Solução**: Criar tópicos manualmente ou via pipeline, garantindo uma governança adequada.
  - **Benefícios**:
    - Organização dos tópicos
    - Prevenção de erros como a criação excessiva de tópicos.

### Compressão de Mensagens
- **Configuração de Compressão**
  - **Método**: Forçar a compressão usando LZ4.
  - **Justificativa**: Muitas empresas não utilizam compressão por falta de conhecimento.
  - **Resultado**: Garantia de que todas as mensagens sejam comprimidas, melhorando a eficiência.

### Retenção de Mensagens
- **Configuração de Retenção**
  - **Padrão**: 7 dias.
  - **Recomendação**: Ajustar o tempo de retenção conforme a necessidade específica da aplicação. 
    - 3 dias geralmente é suficiente para a maioria dos casos.

### Tamanho Máximo de Mensagem
- **Limite de Tamanho**: Configurar o limite máximo de mensagens para 10K.
  - **Racional**:
    - Um tamanho de 1MB pode ser excessivo.
    - Considerar a necessidade de trafegar dados e a eficiência na utilização de banda.
    - Proporção entre payload e a lógica de consulta em bases de dados.

### Replicação e Performance
- **Fator de Replicação**
  - **Binsync Replica**: Especificar quantas réplicas precisam ser confirmadas antes de retornar um ACK ao produtor.
  - **Configuração Recomendada**: 
    - Para performance, pode-se configurar para 2 réplicas.
    - Atenção: Risco de perda de mensagens se os brokers 1 e 2 falharem.
    - Para mensagens críticas, considerar a configuração para 3.

## Considerações Finais
- A configuração do broker em produção é similar ao que foi discutido nas aulas anteriores, com foco em variáveis como broker ID.
- É crucial prestar atenção nas propriedades adicionais ao configurar para garantir performance e segurança.
- Monitoramento e alertas são essenciais para manter a saúde da aplicação.

Agradeço pela atenção e espero que tenham gostado da aula! Até a próxima.



---

## modulo_11_13105.mp4

# Ferramentas para Gerenciamento de Cluster Kafka

## Introdução
Nesta aula, foram apresentadas duas ferramentas para gerenciar clusters Kafka: uma interface gráfica open source chamada **AKHQ** e uma ferramenta não gráfica via terminal.

## AKHQ

### Instalação
- **Métodos de instalação:**
  - Via **Docker**
  - Usando **Java Jar**
  - No **Kubernetes** com **Helm**
  - Standalone, baixando o arquivo Jar diretamente

### Recursos Principais
- **Versão:** 0.24
- **Autenticação:**
  - Integração com **LDAP** para federar logins e criar grupos de acesso.
  - Integração com **GitHub SSO** para autenticação federada.
  
- **Gerenciamento de Tópicos e Consumer Groups:**
  - Visualização de **Consumer Groups** e seus membros.
  - Informações de **lag**, últimos offsets lidos, e status de consumo.
  - Opção de **Live Tail** para acompanhar mensagens em tempo real.
  
- **Configuração de Tópicos:**
  - Informações sobre nome, quantidade de mensagens, tamanho, e partições.
  - Configurações de **replica factor** e **in-sync replicas**.

### Visualização do Cluster
- **Balanceamento de Partições:**
  - Mostra a distribuição de partições entre os brokers.
  - Identificação de **hot partitions** e problemas de balanceamento.

- **Configurações do Nó:**
  - Exibição de todas as configurações do nó, como **compression type** e outras propriedades.

### Suporte a Múltiplos Clusters
- Capacidade de gerenciar e visualizar vários clusters simultaneamente (ex: dev, prod, on-premises, cloud).

## Ferramenta de Linha de Comando (CLI)

### Funcionalidades
- Utilização de scripts `.sh` para gerenciar tópicos e propriedades do Kafka.
- Comandos úteis incluem:
  - `sh kafka-topics.sh` para listar tópicos.
  - `sh kafka-console-producer.sh` para produzir mensagens.
  - `sh kafka-console-consumer.sh` para consumir mensagens.

### Vantagens do CLI
- Ideal para automação e ambientes sem acesso ao AKHQ.
- Complementa a interface gráfica, permitindo operações rápidas e configurações avançadas.

## Outras Ferramentas
- **Confluent Control Center:** Ferramenta paga e robusta para gerenciamento de Kafka.
- **Conductor:** Outra ferramenta paga, mas também eficiente.

## Conclusão
- O **AKHQ** é uma excelente ferramenta open source que atende bem às necessidades de gerenciamento de Kafka.
- O conhecimento das ferramentas gráficas e de linha de comando é essencial para uma gestão eficaz do cluster Kafka.

## Agradecimentos
- Agradeço pela atenção e até a próxima aula!



---

## modulo_11_13175.mp4

# Estudo sobre Cacique ODB e Streaming com Kafka Connect

## Introdução
Nesta aula, Ronaldo Laniellas apresenta como utilizar o *Cacique ODB* para criar um filtro baseado em um tópico existente. Ele faz referência a aulas anteriores onde foi criado um *Kafka Connect Source* que lê dados do *PostgreSQL* e grava em um tópico relacionado a clientes.

## Objetivos da Aula
- Criar um streaming que processa eventos de novos clientes.
- Criar uma view materializada para contar quantas vezes um cliente com o mesmo nome foi criado e qual foi seu último ID.

## Pré-requisitos
- Ter um cluster de Kafka Connect configurado.
- Ter um conector JDBC que lê do PostgreSQL e grava no tópico.

## Passo a Passo

### 1. Configuração do Docker Compose
- **Adicionar seção do Cacique** ao arquivo `docker-compose.yml`.
- Configurar a porta correta para o broker.
- Executar o comando: `docker-compose up`.

### 2. Verificação do Kafka Connect
- Confirmar que o cluster do Kafka Connect está funcionando.
- Criar o conector JDBC se não estiver criado previamente.

### 3. Preparação do Banco de Dados
- Criar a tabela necessária no PostgreSQL.
- Inserir um cliente de exemplo (e.g., "Paul") para verificar a funcionalidade do Kafka Connect.

### 4. Interação com o Cacique
- Acessar o CLI do Cacique.
- Criar um streaming chamado `clients created`:
  - Incluir campos: ID, nome.
  - Ler do tópico `lanielas.client`.
  - Formato dos valores: JSON.
  
#### Comando para criar o streaming:
```
create streaming clients created (id INT, name STRING) 
from 'lanielas.client' 
value format 'JSON';
```

### 5. Consultas no Streaming
- **Push Query**: Usar `emit changes` para notificações de novos eventos.
  - Exemplo: `select clients created emit changes;`
- **Pull Query**: Realizar consultas sem `emit changes` para retornar todos os registros.

### 6. Criação da Tabela Materializada
- Criar uma tabela chamada `last clients` que agregará informações.
- Utilizar funções de agregação para obter dados mais recentes e contagem de clientes.

#### Comando para criar a tabela:
```sql
create table last_clients as 
select name, count(*) as quantidade, latest_by_offset(id) as last_id 
from clients_created 
group by name emit changes;
```

### 7. Verificação e Testes
- Inserir novos clientes e verificar o funcionamento da tabela materializada.
- Confirmar se os dados estão sendo atualizados corretamente no tópico `last clients`.

### 8. Observações Finais
- A tabela `last_clients` é atualizada à medida que novos clientes são inseridos.
- A contagem de clientes e o último ID são exibidos corretamente.
- A documentação do Cacique ODB é rica e contém informações sobre funções e operações possíveis.

## Conclusão
Ronaldo finaliza a aula incentivando os alunos a explorarem a documentação do Cacique ODB e a praticarem as funcionalidades apresentadas.

---

## Dicas para Estudo
- **Revisar conceitos de Kafka** e como funciona o Kafka Connect.
- **Praticar comandos SQL** utilizados para criar streams e tabelas.
- **Familiarizar-se** com a interface do Cacique ODB e suas funcionalidades.
- **Experimentar** com diferentes tipos de dados e cenários para entender melhor o fluxo de dados e agregações.

