# Resumos dos vídeos

## modulo_9_11351.mp4

# Aula sobre Arquitetura Hexagonal

## Introdução
- Início do módulo prático da arquitetura hexagonal.
- Objetivo: Melhorar o código do projeto *BigBolfMod* que apresenta problemas de reutilização e organização.

## Estrutura do Projeto
- O projeto segue um modelo de arquitetura em camadas:
  - **Entidades**:
    - *Customer*: Representa os clientes.
    - *Partner*: Casa de shows ou organizador de eventos.
    - *Event*: Eventos criados pelo partner, com uma lista de tickets.
    - *Ticket*: Comprado pelo customer para participar de um evento.

## Problemas Identificados
- **Controller**:
  - Contém consultas (queries) diretas, dificultando a manutenção.
  - Validações feitas manualmente e falta de regras de negócio.
- **Serviços (Service)**:
  - Apresenta o antipadrão *middleman*, que não agrega valor.
  - Deveria conter regras de negócio, mas não está estruturado corretamente.
  
## Análise do Controller
- O código do controller apresenta:
  - Validações inadequadas e falta de segurança nas operações.
  - Dificuldade em expor a aplicação para diferentes interfaces, como CLI ou GraphQL.

## Introduzindo GraphQL
- Proposta de refatorar o código para incluir suporte a GraphQL.
- Necessidade de criar um *CustomerResolver*:
  - Controller para gerenciar requisições GraphQL.
  - Implementação de mutações e queries para manipulação de dados.

### Passos para Implementação de GraphQL
1. Criar um package chamado `GraphQL`.
2. Implementar a classe `CustomerResolver`.
3. Definir DTOs e mapeamentos para GraphQL:
   - Mapeamento de mutações e queries.
4. Habilitar o GraphQL no Spring.
5. Criar o arquivo `esquema.gqls` para definir tipos e entradas.

## Refatoração do Código
- A necessidade de refatorar o código é evidente para evitar duplicação e garantir a manutenção:
  - Implementar as regras de negócio dentro do *CustomerService*.
  - Garantir que as validações sejam feitas corretamente.
- A arquitetura atual não impõe restrições que evitem a cópia de código mal feito.

## Conclusão
- A prática de copiar e colar código está levando a um projeto frágil e não escalável.
- A próxima aula será dedicada a ensinar como implementar as práticas corretas para melhorar a qualidade e a escalabilidade do código.

## Reflexões Finais
- Questione-se sobre os problemas que uma estrutura de código mal organizada pode causar.
- Considere como a arquitetura hexagonal pode ajudar a resolver esses problemas, promovendo uma melhor separação de preocupações e facilitando a manutenção e evolução do sistema.

### Dicas de Estudo
- Revise os conceitos de *arquitetura hexagonal* e *padrões de projeto*.
- Pratique a refatoração de código em pequenos projetos.
- Experimente implementar GraphQL em um projeto simples para entender os conceitos na prática.



---

## modulo_9_11352.mp4

# Aula: Módulo Prático da Arquitetura Hexagonal

## Introdução
- **Boas-vindas** a mais uma aula do módulo prático da arquitetura hexagonal no MBA de arquitetura.
- **Objetivo**: Melhorar um código existente e entender melhor o problema a ser resolvido.

## Contexto do Projeto
- O projeto em questão é o **BigBolfMod**, que apresenta problemas de reaproveitamento e estrutura.
- **Entidades principais**:
  - **Customer**: Representa os clientes.
  - **Partner**: Representa uma casa de show ou alguém que organiza eventos.
  - **Event**: Eventos organizados pelos partners, que possuem uma lista de tickets.
  - **Ticket**: Comprado pelo customer para acessar o evento.

## Estrutura do Projeto
- O projeto segue uma **arquitetura em camadas**, com as seguintes camadas:
  - **Controllers**: Camada de apresentação (presentation layer).
  - **Services**: Onde deveriam estar as regras de negócio.
  - **Repositories**: Utiliza o **Spring Data JPA** para interação com o banco de dados.

## Problemas Identificados
- **Queries no Controller**: As queries estão sendo lançadas diretamente no controller, o que não é uma prática recomendada.
- **Service como Middleman**: O Customer Service não está agregando valor, funcionando apenas como um intermediário.
- **Validações ausentes**: Falta de validações essenciais (ex: e-mail e CPF) nas operações de criação de clientes.

## Reflexões e Dúvidas
- **Flexibilidade da Aplicação**: Se o código atual é acoplado a um REST API, como expor as regras de negócio em um CLI ou GraphQL?
- **Duplicação de Código**: A necessidade de duplicar a lógica para suportar diferentes interfaces (REST/GraphQL) é preocupante.

## Abordagem para Correção
1. **Configuração do Ambiente**:
   - O conteúdo do MBA é avançado; não são abordadas configurações de Java ou IDE.
   - Recomenda-se configurar o ambiente antes de continuar.

2. **Criação do CustomerResolver**:
   - Criar um novo controller para gerenciar as requisições do GraphQL.
   - Implementar a injeção de dependências pelo construtor para evitar dependências cíclicas.

3. **Implementação de GraphQL**:
   - Criar um esquema para o GraphQL com tipos e mutações necessárias.
   - Habilitar o GraphQL na aplicação e testar com o MySQL.

### Exemplo de Código
- **Customer DTO**: Estruturas para o cliente e suas operações em GraphQL.
- **Mutações e Consultas**: Implementação de mutações (ex: criar um cliente) e consultas (ex: buscar um cliente por ID).

## Problemas com a Implementação Atual
- **Código Suscetível a Erros**: A necessidade de copiar e colar código repetidamente indica problemas na arquitetura.
- **Testes Ineficientes**: Dependência excessiva de testes de integração, sem uma abordagem equilibrada para testes unitários.

## Conclusão
- **Problemas comuns** em projetos de aprendizado, como o BigBolfMod, são frequentes e podem levar a códigos ruins e não escaláveis.
- **Próximos Passos**: Aprender a implementar uma arquitetura melhor e mais organizada na próxima aula. 

## Dicas para Estudo
- **Revisar** os conceitos de arquitetura hexagonal e como eles se aplicam a projetos reais.
- **Praticar** a identificação de problemas em códigos existentes e sugerir melhorias.
- **Explorar** a diferença entre REST e GraphQL e as implicações de design de software ao usar cada um.



---

## modulo_9_11353.mp4

# Aula Prática: Arquitetura Hexagonal

## Introdução
- **Módulo Prático:** Início do módulo prático da arquitetura hexagonal no MBA de arquitetura.
- **Objetivo:** Melhorar um código existente que apresenta problemas de reaproveitamento e organização.

## Contexto do Projeto
- **Projeto Criado por:** O professor que está conduzindo a aula.
- **Entidades Principais:**
  - **Customer:** Representa os clientes.
  - **Partner:** Casa de show ou organizador de eventos.
  - **Event:** Eventos criados pelos partners, com uma lista de tickets.
  - **Ticket:** Comprado pelos customers para participar de eventos.

## Problemas Identificados
- **Código Atual:**
  - Queries lançadas diretamente no controller.
  - Camadas de arquitetura não estão bem definidas.
- **Camadas do Projeto:**
  - **Controllers:** Lógica de apresentação.
  - **Services:** Deveriam conter regras de negócio, mas estão vazias.
  - **Repositories:** Usam Spring Data JPA, mas a implementação não está ideal.

## Análise do Código
- **Middleman Antipattern:** 
  - O serviço não agrega valor e apenas faz proxy entre a camada de controle e repositórios.
- **Controller Problemas:**
  - Validações manuais e sem estrutura.
  - Acoplamento excessivo à REST API, dificultando a reutilização do código em diferentes contextos (CLI, GraphQL).

## Melhoria Proposta
1. **Refatoração Necessária:**
   - Mover regras de negócio para a camada de serviço.
   - Implementar uma estrutura que permita a reutilização do código para diferentes interfaces (REST, GraphQL).
  
2. **Exemplo de GraphQL:**
   - Criação de um `CustomerResolver` para gerenciar entradas via GraphQL.
   - Implementação de métodos de mutação e consulta para gerenciar `Customer`.

3. **Configuração do Ambiente:**
   - Uso de Docker para gerenciar dependências como o MySQL.
   - Estrutura de pastas e arquivos para o GraphQL.

## Implementação do GraphQL
- **Estrutura do GraphQL:**
  - Definição de tipos (`type customer`) e entradas (`input customer input`).
  - Implementação de operações de mutação e consulta.

## Execução e Testes
- **Subida da Aplicação:**
  - Conexão ao MySQL e verificação de que a aplicação está funcionando corretamente.
- **Testes Realizados:**
  - Verificação de erros e exceções geradas durante a execução para assegurar a robustez do sistema.

## Conclusão
- **Reflexão Final:**
  - Importância de um código bem estruturado e escalável.
  - Necessidade de evitar cópias e colagens que levam a um código frágil e difícil de manter.

## Próximos Passos
- **Próxima Aula:**
  - Continuação da refatoração do código e aplicação das boas práticas discutidas.

---

### Dicas de Estudo
- **Reveja os conceitos de arquitetura hexagonal e padrões de design.**
- **Pratique a refatoração de código com ênfase na separação de responsabilidades.**
- **Experimente implementar um pequeno projeto utilizando GraphQL e Spring Data JPA.**



---

## modulo_9_11354.mp4

# Aula: Módulo Prático da Arquitetura Hexagonal

## Introdução
- Boas-vindas à aula sobre arquitetura hexagonal na pós-graduação em MBA de arquitetura.
- Objetivo: melhorar um código existente, que apresenta problemas de reaproveitamento e organização.

## Problemas Identificados no Código
- O projeto BigBolfMod apresenta:
  - **Queries** lançadas diretamente no *controller*.
  - Estrutura não adequada para reutilização e manutenção.

## Estrutura do Projeto
- **Entidades principais**:
  - **Customer**: representa os clientes.
  - **Partner**: casas de show ou eventos.
  - **Event**: eventos realizados, cada um com uma lista de *tickets*.
  - **Ticket**: comprado pelo *customer*.

### Camadas da Arquitetura
1. **Controllers**: camada de apresentação (Y-layer).
2. **Services**: onde deveriam estar as regras de negócio.
3. **Repositories**: utiliza o Spring Data JPA para gerenciamento de dados.

## Análise do Código Atual
- O *customer service* se tornou um *middleman*:
  - Não agrega valor, apenas repassa informações.
- **Controller**:
  - Validações manuais sem checagens adequadas (ex: CPF, e-mail).
  - Operações diretas com o banco de dados sem abstrações.

## Problemas Adicionais
- Dificuldade em expor a aplicação para diferentes interfaces:
  - Transformar um *REST controller* em uma interface CLI ou GraphQL é complicado.
- Quando se tenta usar GraphQL, a necessidade de duplicar esforços fica evidente.

## Refatoração Proposta
- Criar uma classe **CustomerResolver** para gerenciar a lógica de GraphQL.
- Implementar injeção de dependência via construtor para evitar acoplamento.
  
### Criando a Estrutura de GraphQL
1. Habilitar o GraphQL no projeto:
   - Configuração no `application.properties`.
   - Criar um diretório *GraphQL* e um arquivo `schema.gqls`.
2. Definir tipos e mutações:
   - **Type**: `customer` com id, nome, e-mail e CPF.
   - **Mutation**: `createCustomer`.

## Implementação e Testes
- Usar *Docker* para configurar o MySQL e testar a aplicação.
- Verificar se as mutações e consultas funcionam corretamente no GraphQL.
- Exibir resultados e erros durante a execução.

## Conclusão e Próximos Passos
- O código atual é suscetível a cópias e colagens, o que torna a manutenção inviável.
- Necessidade de um refactoring significativo e criação de testes adequados.
- Aprender a construir uma arquitetura escalável e sustentável será o foco da próxima aula.

## Reflexões para Estudo
- Quais problemas específicos você consegue identificar nas práticas atuais?
- Como a arquitetura hexagonal pode ajudar a resolver esses problemas?
- Pense em como a estrutura do código pode ser organizada para permitir uma melhor escalabilidade e manutenção.



---

## modulo_9_11355.mp4

# Resumo da Aula: Extração de Casos de Uso em Controllers

## Introdução
- Apresentação da aula focada na extração de casos de uso.
- Objetivo: Tornar os controllers da aplicação mais leves e organizados.

## Estrutura do Controller
- Importância de um controller “fininho”.
- Necessidade de garantir uma cobertura de testes ampla.
- Abordagem de testes unitários e integração.

## Casos de Uso
### 1. Criar Evento
- **Caso de Uso**: `createEvent`
- **Estrutura**:
  - Extensão de `useCase`.
  - Utilização de `public record input` e `output`.
- **Atributos do Input**:
  - `String date`
  - `String name`
  - `Integer totalSpots`
  - `Long partnerId`
- **Atributos do Output**:
  - Retorno simplificado do evento:
    - `date`
    - `name`
    - `partnerId`
    - `eventId`

### 2. Comprar Ticket
- **Caso de Uso**: `buyEventTicket`
- **Estrutura**:
  - Extensão de `useCase`.
  - Utilização de `public record input` e `output`.
- **Atributos do Input**:
  - `Long eventId`
  - `Long customerId`
- **Atributos do Output**:
  - `Long ticketId`
  - `String ticketStatus`

## Implementação
### Criar Evento
- Extração de dependências:
  - `partnerService`
  - `eventService`
- Validação de entrada utilizando `ValidationException`.
- Lógica de criação de evento com tratamento de exceções.

### Comprar Ticket
- Validações:
  - Verificação se o evento existe.
  - Verificação de capacidade do evento (sold out).
- Lógica de geração de ticket e retorno das informações pertinentes.

## Atualizações no Controller
- Substituição de chamadas diretas por instâncias de casos de uso.
- Garantia de tratamento de exceções com `try-catch`.
- Utilização de `ResponseEntity` para retorno de respostas HTTP.

## Testes
- Importância de rodar todos os testes da aplicação após alterações.
- Garantia de que não houve quebras nas funcionalidades existentes.

## Conclusão
- Isolamento da lógica de negócio em casos de uso.
- Melhoria na legibilidade do código.
- Planejamento para a próxima aula:
  - Implementação do GraphQL para eventos.
  - Criação de testes unitários para os casos de uso.

## Observações Finais
- Importância de manter o código organizado e modular.
- Relevância de testes automatizados para assegurar a qualidade do software.

Este resumo cobre os principais pontos discutidos na aula sobre a extração de casos de uso em controllers, estruturando a informação de forma clara e concisa para facilitar o estudo.



---

## modulo_9_11356.mp4

# Resumo da Aula - Extração de Casos de Uso

## Introdução
- **Tema da Aula**: Extração de casos de uso e melhoria da estrutura dos controllers da aplicação.
- **Objetivo**: Tornar os adapters da REST API e do GraphQL mais eficientes e menos acoplados.

## Estrutura dos Controllers
- **Foco no Último Controller**: Controller do evento.
- **Objetivo**: Reduzir o acoplamento e deixar o controller mais enxuto.
- **Cobertura de Testes**: Garantir que todos os casos de uso tenham testes, tanto integrados quanto unitários.

## Casos de Uso
### 1. Criar Evento
- **Definição do Caso de Uso**: `create event`.
- **Componentes**:
  - **Input**: 
    - `String date`
    - `String name`
    - `Integer totalSpots`
    - `Long partnerId`
  - **Output**: Retorno simplificado do evento.
  
- **Processo**:
  - Validação dos inputs.
  - Criação do evento utilizando serviços dependentes.
  - Retorno de uma cópia simplificada do evento.

### 2. Comprar Ticket
- **Definição do Caso de Uso**: `subscribe customer to event`.
- **Componentes**:
  - **Input**:
    - `Long eventId`
    - `Long customerId`
  - **Output**:
    - `Long ticketId`
    - `String ticketStatus`
  
- **Processo**:
  - Validação dos dados de entrada.
  - Verificação se o evento está esgotado.
  - Geração do ticket e retorno das informações relevantes.

## Melhoria do Código
- **Otimizações Realizadas**:
  - Simplificação do tratamento de exceções.
  - Melhoria na legibilidade do código.
  - Uso de métodos mais enxutos e claros para validações.

## Atualização do Controller
- **Modificações no Controller**:
  - Atualização para utilizar os novos casos de uso.
  - Inclusão de tratamento de exceções (`try-catch`) para validação.
  - Retorno das informações relevantes de forma adequada.

## Testes
- **Importância dos Testes**:
  - Garantir que todas as funcionalidades estejam funcionando corretamente.
  - Rodar todos os testes da aplicação após as mudanças.

## Próximos Passos
- Implementação do GraphQL para o evento.
- Criação dos testes unitários para os novos casos de uso.
- Melhoria contínua das regras de negócio e estrutura do código, buscando evitar entidades anêmicas.
- Trabalhar na parte das portas de saída do hexágono.

## Conclusão
- **Objetivo Alcançado**: Isolar as regras de negócio em casos de uso mais semânticos e melhorar a qualidade do código.
- **Expectativa**: Continuar o trabalho nas próximas aulas para aprimorar a aplicação e o entendimento dos conceitos.



---

## modulo_9_11357.mp4

# Aula sobre Extração de Casos de Uso

## Introdução
- A aula se concentra na extração de casos de uso em uma aplicação.
- O objetivo é melhorar a estrutura dos controllers, tornando-os mais limpos e menos acoplados.

## Objetivos da Aula
- Extrair o último controller relacionado a eventos.
- Reduzir o acoplamento entre serviços.
- Implementar testes unitários para os casos de uso.

## Casos de Uso em Destaque
1. **Criar Evento** (`create event`)
2. **Comprar Ticket** (`buy event ticket`)

## Criando o Caso de Uso: Criar Evento

### Estrutura Inicial
- Extensão da classe `UseCase`.
- Definição da entrada e saída usando `public record input` e `output`.

### Parâmetros do Evento
- **Entrada**:
  - `String date`
  - `String name`
  - `Integer totalSpots`
  - `Long partnerId`
  
### Lógica de Implementação
- Retorno de uma cópia simplificada do evento.
- Validação de entradas utilizando `ValidationException`.

### Dependências
- Inclusão de serviços necessários:
  - `partnerService`
  - `eventService`

## Criando o Caso de Uso: Comprar Ticket

### Estrutura Inicial
- Extensão da classe `UseCase`.
- Definição da entrada e saída.

### Parâmetros do Ticket
- **Entrada**:
  - `Long eventId`
  - `Long customerId`
  
- **Saída**:
  - `Long ticketId`
  - `String ticketStatus`

### Lógica de Implementação
- Validações para garantir que o evento e o cliente existam.
- Verificação se o ticket já foi comprado.
- Geração do ticket e adição à lista de tickets do evento.

### Dependências
- Inclusão de serviços necessários:
  - `eventService`
  - `customerService`

## Atualizações no Controller

### Implementação dos Casos de Uso
- Substituição das chamadas diretas por instâncias dos novos casos de uso.
- Validações para evitar `NullPointerException`.

### Exemplo de Uso
```java
final var useCase = new CreateEventUseCase(eventService, partnerService);
final var output = useCase.execute(new Input(dto.date, dto.name, dto.partner.getId(), dto.totalSpots));
```

## Testes e Validações
- Importância de rodar todos os testes da aplicação.
- Garantir que a extração de casos de uso não quebre funcionalidades existentes.

## Conclusão e Próximos Passos
- Finalização da extração dos casos de uso.
- Planejamento para implementar o GraphQL para eventos na próxima aula.
- Revisão das portas de saída do hexágono e melhoria das entidades.

## Observações Finais
- A estrutura do código foi aprimorada.
- Os casos de uso se tornaram mais semânticos e compreensíveis.
- Importância de manter todos os testes em verde após alterações.

**Espero que todos tenham gostado da aula! Vejo vocês na próxima!**



---

## modulo_9_11358.mp4

# Resumo da Aula: Extração de Casos de Uso e Controllers

## Introdução
Nesta aula, o foco é a extração dos casos de uso na aplicação, especialmente na criação do controller de eventos, visando reduzir o acoplamento e melhorar a legibilidade do código. O professor também menciona a importância de criar testes unitários para os casos de uso.

## Objetivos da Aula
- Extrair e simplificar o controller de eventos.
- Garantir uma cobertura de testes adequada.
- Implementar os casos de uso para:
  - Criar um evento
  - Comprar um ingresso

## Estrutura do Controller

### 1. Criar Evento
- **Casos de uso:**
  - `create event`
- **Componentes:**
  - Input: `date`, `name`, `totalSpots`, `partnerId`
  - Output: Retorna uma cópia simplificada do evento.
- **Implementação:**
  - Utilizar o padrão *public record input*.
  - Manter o input como `string` para a data, permitindo flexibilidade na formatação.
  - Retorno simplificado do evento, incluindo atributos essenciais.

### 2. Comprar Ingresso
- **Casos de uso:**
  - `buy ticket`
- **Componentes:**
  - Input: `eventId`, `customerId`
  - Output: Retorna o `ticketId` e o `ticketStatus`.
- **Implementação:**
  - Verificação de validade do evento e do cliente.
  - Verificação de disponibilidade de ingressos (sold out).
  - Gerar o ticket e retornar os dados necessários.

## Melhoria do Código
- **Redução de Acoplamento:**
  - Remover dependências desnecessárias dos controllers para manter o código limpo.
- **Tratamento de Exceções:**
  - Utilizar `ValidationException` para tratar erros de validação.
  - Implementar mensagens de erro apropriadas para o usuário.

## Testes
- A importância de realizar testes unitários para todos os casos de uso implementados.
- Garantir que todos os testes da aplicação estejam passando após as alterações no código.

## Conclusão
- Os controllers foram simplificados e a lógica de negócio foi isolada em casos de uso, tornando o código mais semântico.
- Na próxima aula, serão abordados:
  - Implementação do GraphQL para eventos.
  - Criação de testes unitários para os novos casos de uso.

### Observações Finais
- O professor destaca a importância de manter a legibilidade do código e a necessidade de revisitar a arquitetura hexagonal para melhorar ainda mais a estrutura da aplicação.

## Tópicos para Estudo
1. **Casos de Uso**
   - Definição e importância na arquitetura de software.
2. **Padrões de Design**
   - Padrão *public record* e sua aplicação em Java.
3. **Tratamento de Exceções**
   - Como implementar e manejar exceções customizadas.
4. **Testes Unitários**
   - Estratégias para garantir a cobertura de testes em casos de uso.
5. **Arquitetura Hexagonal**
   - Conceitos e benefícios da arquitetura hexagonal em aplicações.

## Dicas
- Pratique a implementação dos casos de uso em projetos pessoais.
- Experimente escrever testes unitários para os seus métodos.
- Estude sobre a arquitetura hexagonal para entender melhor a separação de responsabilidades.



---

## modulo_9_11359.mp4

# Resumo da Aula sobre Domínio no Hexágono

## Introdução
- A aula foca na criação das entidades de domínio dentro do hexágono.
- Objetivo: Trabalhar em entidades de domínio e criar a interface de repositório.

## Entidades de Domínio
- **Diferença entre Caso de Uso e Domínio**:
  - Casos de uso, como `createCustomer`, não representam o domínio real, mas sim tabelas de banco de dados.
  - O foco deve ser em um domínio que faça sentido, não apenas em tabelas.

### Conceito de Agregado
- O conceito de **agregado** é central no DDD (Domain-Driven Design).
- Um agregado é:
  - Um limite transacional que agrupa várias entidades.
  - Identificado por um ID (não por propriedades, como objetos de valor).
  - Deve garantir a integridade e invariantes das entidades que contém.
- Persistência de dados deve ser feita de forma atômica dentro de um único agregado.

## Estrutura do Hexágono
- A estrutura de pacotes é genérica e pode variar entre projetos.
- Recomenda-se a criação de um pacote **Entities** dentro do hexágono:
  - Pode ser considerado como um pacote de **Domain** em outras arquiteturas, como na **Clean Architecture**.

## Criação da Entidade `Customer`
- **Definição da Entidade**:
  - Criação de `Customer` com um objeto de valor `CustomerId`.
  - O `CustomerId` é um identificador único, representado por um `ID long`.
  
### Implementação do `CustomerId`
- Criação de métodos de fábrica:
  - `Unique`: gera um novo `CustomerId`.
  - `If`: recebe uma string e converte para `CustomerId`, com validação.
  
### Propriedades do `Customer`
- Propriedades da entidade `Customer` incluem:
  - `Name`
  - `CPF`
  - `Email`
  
### Validações
- As validações são aplicadas no construtor da entidade:
  - Verificações para garantir que `CustomerId`, `Name`, `CPF`, e `Email` não são nulos.
  - Validações adicionais para CPF e Email usando expressões regulares.

## Interface de Repositório
- A interface `CustomerRepository` é criada para expor métodos de persistência:
  - `CustomerOfId(CustomerId)`: retorna um `Customer`.
  - `CustomerOfCPF(String)`: busca um `Customer` pelo CPF.
  - `CustomerOfEmail(String)`: busca um `Customer` pelo Email.
  - `Save(Customer)`: método para salvar um `Customer`.

## Atualização do Caso de Uso
- O caso de uso `CreateCustomer` é atualizado para utilizar a nova estrutura de domínio.
- O fluxo de criação do `Customer` é simplificado, delegando a lógica para a entidade.

## Testes
- Após as mudanças, os testes unitários são ajustados para a nova estrutura.
- Implementação de um repositório em memória (`InMemory.CustomerRepository`) para facilitar os testes.

## Conclusão
- A aula abordou a importância de trazer regras de negócio para o domínio.
- As dependências externas foram removidas dos casos de uso, permitindo maior encapsulamento.
- Progresso significativo foi feito na criação de uma arquitetura centrada no domínio.

## Próximos Passos
- Continuar a evolução do domínio e a validação das entidades.
- Abordar a interface de gateways na próxima aula.

### Dicas de Estudo
- **Revisar o conceito de DDD** e como ele se aplica na criação de entidades.
- **Praticar a implementação de métodos de fábrica** e validações para entidades de domínio.
- **Estudar a estrutura do hexágono** e como ela organiza a lógica de aplicação e infraestrutura.



---

## modulo_9_11360.mp4

# Aula sobre Entidades de Domínio e Arquitetura Hexagonal

## Introdução
- Nesta aula, o foco é na criação de entidades de domínio dentro do hexágono.
- O objetivo é desenvolver a interface de repositório e finalizar os componentes do hexágono.

## Conceitos Fundamentais

### O que é Domínio?
- Domínio refere-se ao contexto e regras de negócio que a aplicação deve seguir.
- Um caso de uso, como `createCustomer`, deve interagir com o domínio, não apenas com a infraestrutura (como tabelas de banco de dados).

### DDD (Domain-Driven Design)
- O conceito de **agregado** é crucial no DDD.
  - Um agregado é uma entidade que pode conter outras entidades e é identificado por um ID.
  - Deve garantir a integridade e as invariantes das entidades que agrupa.

### Estrutura do Hexágono
- A estrutura do hexágono protege a lógica de negócio das interações externas (drivers e driven actors).
- Sugestão de estrutura de pacotes:
  - **Application**
  - **Infrastructure**
  - **Entities** (ou **Domain**)

## Criação da Entidade Customer

### Exemplo de Implementação
- A entidade `Customer` é criada com os seguintes atributos:
  - **CustomerId**: um objeto de valor que representa o identificador do cliente.
  - **Name**: nome do cliente.
  - **CPF**: Cadastro de Pessoa Física.
  - **Email**: e-mail do cliente.

### Validações
- O construtor da entidade deve validar os parâmetros:
  - `CustomerId` não pode ser nulo.
  - `Name`, `CPF` e `Email` não podem ser nulos.
  - Validações adicionais para CPF e Email usando expressões regulares.

### Métodos de Fábrica
- Implementação de métodos de fábrica para criar instâncias de `Customer`:
  - **Unique**: gera um novo ID único.
  - **If**: cria um `CustomerId` a partir de uma string, com tratamento para valores inválidos.

## Interface de Repositório

### Criação do Repositório
- Uma interface `CustomerRepository` deve ser criada para gerenciar a persistência do agregado `Customer`.
- Métodos a serem implementados:
  - `CustomerOfId(CustomerId id)`: retorna um `Optional<Customer>`.
  - `CustomerOfCPF(String cpf)`: busca um cliente pelo CPF.
  - `CustomerOfEmail(String email)`: busca um cliente pelo email.
  - `Save(Customer customer)`: persiste um cliente.

### Ajustes nos Casos de Uso
- Ajustes nos métodos de casos de uso para utilizar a nova interface de repositório.
- Redução da lógica diretamente no controlador, distribuindo-a entre o caso de uso e a entidade.

## Testes e Validações

### Implementação de Testes
- Criação de uma implementação em memória de `CustomerRepository` para testes.
- Testes devem garantir que:
  - Não é possível criar um cliente com CPF duplicado.
  - Validações como CPF inválido e e-mail inválido sejam testadas adequadamente.

### Resultados dos Testes
- A maioria dos testes deve passar após as implementações, exceto testes integrados que podem falhar devido a dependências externas.

## Conclusão
- A aula demonstrou como trabalhar com entidades de domínio e implementar a arquitetura hexagonal.
- A lógica de negócio foi integrada ao domínio, e as dependências externas foram minimizadas.
- Espera-se que os alunos tenham compreendido os conceitos e as práticas apresentadas.

## Próximos Passos
- Continuar a implementação de outras entidades e casos de uso.
- Refinar validações e explorar outras interações dentro do hexágono.

**Nota:** Certifique-se de revisar as expressões regulares e as validações aplicadas para garantir que atendam aos requisitos específicos do projeto.



---

## modulo_9_11361.mp4

# Aula sobre Domínio e Arquitetura Hexagonal

## Introdução
- A aula foca na criação de domínios dentro do hexágono.
- Objetivo: entender entidades de domínio, especialmente a entidade `Customer`.

## Conceitos Fundamentais

### Entidades de Domínio
- Diferenciação entre *casos de uso* e *entidades de domínio*.
- O caso de uso `createCustomer` utiliza a tabela de infraestrutura, não o domínio.

### DDD (Domain-Driven Design)
- Importância do conceito de *agregado*.
  - Agregados são limites transacionais que agrupam entidades.
  - Não é necessário ter uma interface de repositório para cada entidade.

### Estrutura do Hexágono
- O hexágono deve ser protegido de *drivers* e *driven actors*.
- Criação de um pacote chamado `Entities` dentro do hexágono, que pode ser considerado como o *Domain*.

## Implementação da Entidade Customer

### Criação da Classe Customer
- Atributos iniciais:
  - `CustomerId`, `Name`, `CPF`, `Email`.
- Utilização de *objetos de valor* e *métodos de fábrica* para criar a entidade.

#### Estrutura da Classe Customer
1. **Identificador**
   - `CustomerId` é um objeto de valor.
   - Propriedades imutáveis e identificadas pelo seu valor.
2. **Validações**
   - Validações no construtor para evitar valores inválidos.
   - Uso de *expressões regulares* para validar CPF e Email.
3. **Métodos de Fábrica**
   - `Unique` e `If` para criação de `CustomerId`.

### Implementação do Repositório
- Criação da interface `CustomerRepository`.
  - Métodos: `CustomerOfId`, `CustomerOfCPF`, `CustomerOfEmail`, `Save`.
- O repositório deve gerenciar a persistência do agregado, não apenas tabelas.

## Alterações nos Casos de Uso

### Modificações no Caso de Uso createCustomer
- Substituição de dependências para utilizar o novo `CustomerRepository`.
- Melhoria na lógica de criação e validação de `Customer`.

### Exemplo de Código
- Ajustes em métodos de entrada e saída para refletir mudanças na estrutura de dados.
  
## Testes
- Criação de uma implementação fake `InMemory.CustomerRepository` para testes.
- Manutenção de testes unitários e correção de falhas relacionadas a dependências externas.

## Conclusão
- A aula proporcionou um avanço significativo na construção do domínio.
- Validações de CPF e Email foram implementadas.
- Todas as dependências externas foram removidas dos casos de uso, resultando em um domínio mais robusto.

## Próximos Passos
- Continuação do desenvolvimento da arquitetura hexagonal.
- Implementação de mais regras de negócios e validações. 

### Observações Finais
- A importância de manter o código organizado e focado no domínio.
- A prática de criar implementações em memória para facilitar testes.



---

## modulo_9_11362.mp4

# Resumo da Aula: Trabalhando com o Domínio do Hexágono

## Introdução
- A aula foca na criação de domínios dentro do hexágono.
- Serão discutidas entidades de domínio e a interface de repositório.

## Conceitos Fundamentais

### Domínio vs. Infraestrutura
- Os casos de uso (ex: `createCustomer`) não devem se concentrar apenas em tabelas de banco de dados.
- O objetivo é criar um domínio que faça sentido, não apenas uma representação de dados.

### DDD (Domain-Driven Design)
- O conceito de **agregado** é fundamental:
  - Um agregado é um limite transacional que contém várias entidades.
  - A integridade do agregado deve ser mantida, garantindo que suas invariantes não sejam quebradas.

## Estrutura do Hexágono
- O hexágono deve ser protegido de drivers e atores:
  - O Alistair Cockburn não especifica detalhes sobre pacotes ou estrutura de pastas.
  - Recomenda-se criar um pacote chamado **Entities** dentro do hexágono.

## Criação da Entidade `Customer`
- **Identificador**: Criar um `CustomerId` como objeto de valor.
  - O `CustomerId` será imutável e representará um ID.
  - Utilizar **Factory Methods** para a construção do objeto.

### Propriedades do `Customer`
- Propriedades a serem implementadas:
  - `Name`
  - `CPF`
  - `Email`
- O construtor deve validar as propriedades:
  - Se `CustomerId`, `Name`, `CPF` ou `Email` forem nulos, lançar uma `ValidationException`.
  - Implementar validações básicas de CPF e Email usando regex.

## Interface de Repositório
- A interface `CustomerRepository` deve expor métodos para gerenciar a persistência do agregado:
  - `CustomerOfId(CustomerId)`: Retorna um `Optional<Customer>`.
  - `CustomerOfCPF(String)`: Retorna um `Customer`.
  - `CustomerOfEmail(String)`: Retorna um `Customer`.
  - `Save(Customer)`: Salva o cliente.

## Atualizações no Caso de Uso `CreateCustomer`
- Refatorar o caso de uso para utilizar a nova estrutura de entidades e repositórios.
- O código deve se tornar mais conciso, utilizando o **Factory Method** para criar `Customer`.

## Validações e Testes
- Implementação de testes unitários para garantir que as validações funcionem corretamente.
- Criar uma classe `InMemoryCustomerRepository` para facilitar os testes, sem depender de uma infraestrutura externa.
- Garantir que as exceções sejam lançadas corretamente em caso de entradas inválidas.

## Conclusão
- O domínio está sendo enriquecido com regras de negócio.
- A dependência externa do hexágono foi removida dos casos de uso, centralizando a lógica dentro do domínio.
- A evolução do código demonstrou a importância de manter a integridade e a validação das entidades.

## Próximos Passos
- Continuar a implementação das demais entidades e repositórios.
- Fazer ajustes e melhorias baseadas nas práticas aprendidas durante a aula.



---

## modulo_9_11363.mp4

# Resumo da Aula: Consolidação de Entidades de Domínio e Casos de Uso

## Introdução
Nesta aula, o objetivo é consolidar o que foi aprendido sobre entidades de domínio e casos de uso. Serão feitas considerações finais e apontados pontos em aberto para aulas futuras.

## Estruturação de Pacotes
- **Organização de Pacotes**:
  - Criar pacotes para **Customer**, **Partner**, **Event**, e **Ticket**.
  - Mover classes relevantes para os pacotes correspondentes.
  
### Pacotes Criados:
1. **Customer**:
   - Classes relacionadas a clientes.
2. **Partner**:
   - Classes relacionadas a parceiros.
3. **Event**:
   - Classes relacionadas a eventos.
4. **Ticket**:
   - Classes relacionadas a ingressos.
  
### Objetos de Valor
- Quatro objetos de valor foram identificados que pertencem a uma pessoa física e jurídica.
- Nome é considerado genérico e não foi incluído como um objeto de valor.

## Casos de Uso
- Separação dos casos de uso em pacotes:
  - Pacote **Customer**: Métodos relacionados a clientes.
  - Pacote **Partner**: Métodos para criar e obter parceiros.
  - Pacote **Event**: Métodos para criar eventos e inscrever clientes em eventos.
  
## Testes e Refatoração
- Importância dos testes:
  - Validar cada validação em um escopo menor para facilitar o diagnóstico de problemas.
  
### Exemplos de Testes:
- **Customer**:
  - Não deve permitir instanciar um cliente com:
    - E-mail duplicado.
    - CPF inválido.
    - Nome inválido.
  
- **Partner**:
  - Não deve permitir instanciar um parceiro com:
    - CNPJ inválido.
    - Nome inválido.
    
- **Event**:
  - Testes para garantir que eventos são criados corretamente e que não podem ser criados com dados inválidos (nome, data, total de vagas).
  - Implementação de testes para o método **ReserveTicket**:
    - Deve reservar um ticket quando possível.
    - Não deve permitir reserva de ticket quando o evento está esgotado.

## Validações e Exceções
- Exceções devem ser tratadas adequadamente para garantir a robustez do sistema.
- Implementação de mensagens de erro claras para validações falhadas.

## Conclusão
- A aula concluiu com a criação de uma estrutura robusta de testes que garante a funcionalidade correta das entidades de domínio.
- Importância dos testes foi enfatizada para a segurança do código.

## Próximos Passos
- Continuar a explorar e implementar testes para outras entidades e cenários.
- Revisar e expandir os pacotes conforme necessário.

## Dicas para Estudo
- **Revise** a estrutura de pacotes e como as classes estão organizadas.
- **Pratique** a implementação de testes para diferentes cenários.
- **Entenda** a importância da validação e como as exceções são tratadas no código.

Esta aula proporciona uma base sólida para a compreensão de entidades de domínio e casos de uso, assim como a importância de testes no desenvolvimento de software.



---

## modulo_9_11364.mp4

# Resumo da Aula: Consolidação de Entidades de Domínio e Casos de Uso

## Objetivos da Aula
- Consolidar o entendimento sobre entidades de domínio e casos de uso.
- Realizar considerações finais sobre o material estudado.
- Organizar o código em pacotes adequados.

## Estrutura do Código
### Organização em Pacotes
- Criar pacotes para organizar melhor as entidades:
  - **Customer**: Contém entidades e casos de uso relacionados a clientes.
  - **Partner**: Contém entidades e casos de uso relacionadas a parceiros.
  - **Event**: Contém entidades e casos de uso relacionadas a eventos.
  - **Ticket**: Contém entidades e casos de uso relacionadas a ingressos.
  - **Value Objects**: Informações sobre pessoas (físicas e jurídicas).

### Casos de Uso
- Separar casos de uso em pacotes:
  - **Customer**: `Create Customer`, `Get Customer`.
  - **Partner**: `Create Partner`, `Get Partner`.
  - **Event**: `Create Event`, `Subscribe Customer to Event`.

## Importância dos Testes
- Testes são cruciais para validar a funcionalidade de cada parte do código:
  - **Validação de Dados**: Garantir que dados inválidos não sejam aceitos.
  - **Escopo Menor**: Testes menores ajudam a identificar problemas rapidamente.
  
### Exemplos de Testes
1. **Teste de Cadastro de Cliente**:
   - Verificar se um cliente pode ser cadastrado com e-mail duplicado.
   - Certificar que um cliente não pode ser criado com CPF inválido.
  
2. **Teste de Cadastro de Parceiro**:
   - Garantir que não é possível cadastrar um parceiro com CNPJ inválido.

3. **Teste de Eventos**:
   - Verificar se um evento pode ser criado com dados válidos.
   - Garantir que o cadastro de um evento com nome inválido resulta em erro.

## Métodos e Validações
### Métodos Importantes
- **ReserveTicket**: Método responsável por reservar um ingresso para um evento.
  - Deve garantir que a reserva só ocorra se houver disponibilidade.
  - Testes devem validar cenários onde a reserva é possível e onde falha.

### Validações Realizadas
- Verificações de nome, data e outros atributos de eventos e parceiros.
- Mensagens de erro claras para cada tipo de validação que falha.

## Conclusões
- A estruturação correta do código em pacotes facilita a manutenção e a escalabilidade do projeto.
- A realização de testes abrangentes garante que o sistema funcione conforme esperado, prevenindo problemas futuros.
- A organização e a validação efetiva são fundamentais para o sucesso em projetos de desenvolvimento de software.

## Pontos em Aberto
- Discussão sobre a modelagem mais profunda de DDD (Domain-Driven Design).
- Análise de como os casos de uso podem ser otimizados e integrados em um fluxo contínuo de desenvolvimento.

## Próximos Passos
- Continuar a estruturação e validação das entidades e casos de uso.
- Explorar mais sobre DDD e suas aplicações em projetos de software. 

**Nota**: Mantenha a prática constante de testes e revisões para garantir a qualidade do código e o entendimento dos conceitos abordados.



---

## modulo_9_11365.mp4

# Resumo da Aula: Consolidação de Entidades de Domínio e Casos de Uso

## Introdução
- A aula tem como objetivo consolidar o conteúdo anterior.
- Serão feitas considerações finais e comentários sobre pontos em aberto para próximas aulas.

## Organização de Pacotes
- **Estrutura de Pacotes**:
  - Criar pacotes para organizar melhor as entidades.
    - **Pacote Customer**:
      - Incluir as entidades relevantes.
    - **Pacote Partner**:
      - Incluir as entidades relevantes.
    - **Pacote Event**:
      - Incluir as entidades relevantes.
    - **Pacote Ticket**:
      - Incluir as entidades relevantes.
  
## Entidades de Domínio e Casos de Uso
- **Entidades de Domínio**:
  - *Value Objects* que representam informações de pessoas físicas e jurídicas.
  - Identificar e organizar entidades como:
    - **Person**: Informações de pessoas (exceto o nome que é genérico).
  
- **Casos de Uso**:
  - Separar casos de uso em pacotes:
    - **Pacote Customer**: Casos relacionados ao cliente.
    - **Pacote Partner**: Criar e obter parceiros.
    - **Pacote Event**: Criar eventos e inscrever clientes.

## Modelagem
- A modelagem deve ser revisada com base nos princípios de *Domain-Driven Design (DDD)*.
- Relacionamentos entre entidades devem ser claros (ex: Event possui Tickets).

## Testes e Validações
- Importância dos testes:
  - Validar cada aspecto individualmente em um escopo menor.
  - Garantir que mudanças em validações específicas não quebrem a lógica geral.

### Exemplos de Testes
- **Testes para Customer**:
  - Não deve permitir cadastro com e-mail duplicado.
  - Deve validar CPF e nome.
  
- **Testes para Partner**:
  - Similar aos testes de Customer, mas com validações de CNPJ.

- **Testes para Event**:
  - Criar eventos deve respeitar validações como nome, data e total de lugares.
  - Testar a reserva de Tickets.
  
### Cenários de Teste
1. **Cenário Feliz**:
   - Reservar um ticket quando houver disponibilidade.
  
2. **Cenário Infeliz**:
   - Reservar um ticket quando o evento estiver esgotado.
   - Não permitir a reserva de tickets para o mesmo cliente mais de uma vez.

## Conclusão
- A cobertura de testes para as entidades de domínio está bem garantida.
- Os alunos devem replicar testes para outras entidades como CPF e e-mail.
- A aula termina com uma expectativa positiva para as próximas discussões.

## Próximos Passos
- Revisar e implementar os testes discutidos.
- Preparar-se para as próximas aulas que abordarão novos conceitos e aprofundamentos nas entidades e casos de uso.



---

## modulo_9_11366.mp4

# Resumo da Aula: Consolidação de Entidades de Domínio e Casos de Uso

## Introdução
- A aula tem como objetivo consolidar os conceitos abordados anteriormente.
- Serão feitas considerações finais sobre as entidades de domínio e casos de uso.
- Discussão sobre pontos em aberto a serem explorados nas próximas aulas.

## Estruturação de Pacotes
- **Organização de classes em pacotes**:
  - **Pacote Customer**: inclusão de classes relacionadas a clientes.
  - **Pacote Partner**: inclusão de classes relacionadas a parceiros.
  - **Pacote Event**: inclusão de classes relacionadas a eventos.
  - **Pacote Ticket**: inclusão de classes relacionadas a ingressos.
  - **Value Objects**: identificação de objetos de valor relacionados a pessoas físicas e jurídicas.

## Casos de Uso
- **Separação de casos de uso em pacotes**:
  - **Customer**: casos de uso relacionados a clientes.
  - **Partner**: criação e recuperação de parceiros.
  - **Event**: criação de eventos e inscrição de clientes em eventos.

## Modelagem e DDD
- **Domain-Driven Design (DDD)**:
  - Discussão sobre a modelagem e a estrutura de pacotes.
  - Necessidade de entender como as entidades interagem e se relacionam.

## Testes e Validações
- **Importância dos testes**:
  - Validação de cada funcionalidade em um escopo menor.
  - Garantia de que cada validação funciona corretamente.

### Exemplos de Testes Criados
1. **Testes para a entidade Customer**:
   - Não deve cadastrar um cliente com e-mail duplicado.
   - Não deve instanciar um cliente com CPF inválido.
   - Validação de nome e e-mail.

2. **Testes para a entidade Partner**:
   - Não deve instanciar um parceiro com CNPJ inválido.
   - Validação de nome e e-mail para parceiros.

3. **Testes para Event e Ticket**:
   - Criação de eventos e validação de entradas.
   - Testes para o método `ReserveTicket`:
     - Não deve reservar um ingresso se o evento estiver esgotado.
     - Não deve permitir a reserva de múltiplos ingressos para o mesmo cliente.

## Estrutura de Testes
- **Organização dos testes em pacotes**:
  - **Pacote Customer**: testes relacionados a clientes.
  - **Pacote Partner**: testes relacionados a parceiros.
  - **Pacote Event**: testes relacionados a eventos.

## Conclusão
- **Cobertura de testes**: A cobertura de testes foi considerada excelente, garantindo a segurança das funcionalidades.
- **Próximos passos**: Preparação para as próximas aulas e discussões sobre novos temas.

## Considerações Finais
- Importância da validação e da estruturação correta das entidades de domínio.
- Enfoque contínuo em garantir a qualidade do código através de testes rigorosos.



---

## modulo_9_11367.mp4

# Resumo da Aula sobre Arquitetura Hexagonal

## Introdução
Nesta aula, foram feitas considerações finais sobre o módulo de Arquitetura Hexagonal, com dicas para aprofundamento e revisão dos conceitos abordados.

## Recapitulação da Estrutura da Aplicação
- **Mudança do Código**: A aplicação foi reorganizada, saindo de uma estrutura com *spaghetti code* para uma arquitetura mais limpa.
- **Pacotes Criados**:
  - **Application**: Contém casos de uso, repositórios e o domínio.
  - **Infrastructure**: Abrange a parte externa do hexágono, incluindo:
    - *Interface Adapters*
    - *Drivers*
    - *Driven Actors*

## Controllers e Adaptadores
- Os antigos controllers foram transformados em **REST Controllers** e **GraphQL**.
- Cada controller agora é um adaptador que implementa casos de uso específicos.
- **DTOs**:
  - Compartilhadas entre REST e GraphQL.
  - Necessidade de cuidado para evitar dependências indesejadas entre eles.

## Casos de Uso e Configurações
- Casos de uso foram organizados em uma classe de **Configurações**.
- Discussão sobre a possibilidade de usar CDI do Java para configuração automática.
- **Repositórios**:
  - Interfaces adaptadoras que não são implementações JPA.
  
## Manipulação de Agregados e Eventos de Domínio
- Discussão sobre a necessidade de manipular agregados corretamente.
- Introdução ao conceito de **Eventos de Domínio**:
  - Permitem a manipulação de um agregado, disparando reações em outros casos de uso.
  - Sugestão de implementar um sistema de reservas de eventos, mantendo a integridade dos dados.

## Criação de Domínios Ricos
- Definição de um agregado como uma entidade identificada por um ID imutável.
- Uso de **Factory Methods** para facilitar a construção de objetos.
- Criação de objetos de valor (ex: CNPJ, CPF, Email) que encapsulam validações.

## Testes
- Abordagem de testes integrados e unitários.
- Importância de manter os testes rápidos e independentes.
- Discussão sobre a *Pirâmide Prática de Testes* de Martin Fowler.

## Dicas e Recomendações
1. **Sub-Módulos do Gradle**:
   - Recomenda-se a criação de sub-módulos para separar a camada de aplicação da infraestrutura.
   - Isso ajuda a evitar acoplamentos indesejados entre frameworks e regras de negócio.
2. **Uso de ArcUnit**:
   - Para testar a arquitetura da aplicação, garantindo que pacotes e classes estejam coerentes.

## Conclusão
- A aula finalizou com um convite aos alunos para implementarem as sugestões discutidas, especialmente em relação a eventos de domínio e arquitetura limpa.

## Próximos Passos
- Implementação de conceitos de **Clean Architecture** nas próximas aulas.

### Observações Finais
- A prática e a implementação dos conceitos discutidos serão cruciais para o entendimento e aplicação da Arquitetura Hexagonal e princípios de DDD.



---

## modulo_9_11371.mp4

# Resumo da Aula sobre Padrões DDD

## Introdução
Nesta aula, foi feita uma revisão dos padrões de DDD (Domain-Driven Design), focando principalmente na modelagem tática. Os conceitos abordados incluem:

- *Value Objects* (Objetos de Valor)
- *Entities* (Entidades)
- *Aggregates* (Agregados)
- *Domain Events* (Eventos de Domínio)

## 1. Value Objects (Objetos de Valor)
- **Definição**: Objetos que são identificados por seus valores, não por um identificador único.
- **Exemplos**:
  - *CNPJ*: sua identificação é o número do CNPJ.
  - *Endereço*: identificação através dos atributos (rua, número, complemento), não possui um ID próprio.
- **Características**:
  - Não devem ser alterados; se seus valores mudam, um novo objeto deve ser criado.

## 2. Entities (Entidades)
- **Definição**: Objetos que possuem uma identidade única (ID) e podem ter seus atributos alterados ao longo do tempo.
- **Exemplo**: 
  - *Customer*: um cliente tem um ID único que o identifica, mesmo que outros atributos (como nome) mudem.
- **Características**:
  - O ID permanece constante após a criação.
  - Exemplos de identificação: CPF para pessoas no contexto governamental.

## 3. Aggregates (Agregados)
- **Definição**: Um cluster de entidades e objetos de valor que são tratados como uma única unidade.
- **Aggregate Root (Raiz de Agregação)**:
  - É a entidade principal do agregado que expõe métodos públicos e controla o comportamento do agregado.
  - **Características**:
    - Todo Aggregate Root é uma entidade com um identificador.
    - Nem toda entidade é um Aggregate Root.
- **Importância**:
  - Representa o limite transacional entre as classes e objetos de valor dentro do domínio.

## 4. Domain Events (Eventos de Domínio)
- **Definição**: Eventos que são gerados a partir de mutações em um agregado.
- **Uso**:
  - Permitem notificar outros sistemas ou pacotes sobre mudanças sem gerar acoplamento.
  - Auxiliam na interação entre diferentes agregados e casos de uso.
- **Consistência Eventual**: A abordagem de garantir que, eventualmente, todos os sistemas estejam atualizados.

## Conclusão
A aula fez uma rápida revisão dos principais padrões de DDD e enfatizou a importância de compreender cada um deles para aplicar corretamente a modelagem tática. Na próxima aula, será abordado o tema dos *Domain Events* com mais profundidade, incluindo a sua utilização dentro da arquitetura limpa (CleanArc). 

## Próximos Passos
- **Próxima Aula**: Estudo detalhado sobre *Domain Events* e como integrá-los na implementação do CleanArc.
- **Preparação**: Revisar os conceitos apresentados e refletir sobre como eles podem ser aplicados em projetos reais.



---

## modulo_9_11372.mp4

# Resumo da Aula sobre Padrões DDD

## Introdução
Na aula de hoje, foram abordados os padrões de DDD (Domain-Driven Design), focando principalmente na *modelagem tática*. A seguir, estão os principais conceitos discutidos.

## 1. Objetos de Valor (Value Objects)
- **Definição**: Objetos que são identificados por seus valores.
- **Exemplos**:
  - **CNPJ**: A identificação é o número do CNPJ.
  - **Endereço**: Não possui um ID, sua identidade é definida por atributos como rua, número e complemento.

## 2. Entidades
- **Definição**: Objetos que têm uma identidade única e seus atributos podem ser alterados.
- **Características**:
  - Identificação através de um ID único.
  - Permanência do ID mesmo com alterações nos atributos.
- **Exemplo**:
  - **Customer**: A entidade é identificada por um ID mesmo que seus atributos, como nome ou documento, mudem.

## 3. Agregado (Aggregate)
- **Definição**: Um cluster de entidades e objetos de valor que são tratados como uma única unidade.
- **Conceitos-chave**:
  - **Limite Transacional**: Representa o conjunto que deve ser persistido junto de forma atômica.
  - **Aggregate Root**: 
    - A classe que representa o agregado e expõe métodos que manipulam seu comportamento.
    - **Características**:
      - Todo Aggregate Root é uma entidade com um identificador.
      - Nem toda entidade é um Aggregate Root.

## 4. Eventos de Domínio (Domain Events)
- **Definição**: Eventos gerados a partir de mutações em um agregado.
- **Função**: Permitem a notificação e interação entre agregados e outros casos de uso sem gerar acoplamento.
- **Consistência Eventual**: Os eventos são propagados para outros sistemas, garantindo a integridade sem dependências diretas.

## Conclusão
- A aula revisou rapidamente os *padrões DDD* com foco na *modelagem tática*.
- Na próxima aula, serão abordados os *Eventos de Domínio* com mais profundidade, incluindo sua produção e integração na arquitetura limpa (CleanArc).

## Próximos Passos
- Estudar mais sobre Eventos de Domínio e sua aplicação no CleanArc.
- Preparar perguntas para discussão na próxima aula.

---

Esses pontos fornecem uma base sólida sobre os padrões de DDD discutidos, facilitando a revisão e o entendimento dos conceitos centrais.



---

## modulo_9_11374.mp4

# Resumo da Aula sobre Padrões DDD (Domain-Driven Design)

## Introdução
Nesta aula, foi realizada uma revisão rápida sobre os padrões de DDD, focando especialmente na modelagem tática. Os conceitos revisados incluem:

- **Value Objects (Objetos de Valor)**
- **Entidades**
- **Agregados**
- **Eventos de Domínio**

---

## 1. Value Objects (Objetos de Valor)
- **Definição**: Objetos cuja identificação é feita através de seus valores.
- **Exemplos**:
  - **CNPJ**: Identificado pelo seu número.
  - **Endereço**: Não faz sentido ter um ID. Identificado por seus atributos (rua, número, complemento).

---

## 2. Entidades
- **Definição**: Objetos que possuem um identificador único (ID) e cujos atributos podem mudar ao longo do tempo.
- **Características**:
  - Um ID único é atribuído na criação da entidade.
  - Por exemplo, um cliente (Customer) é uma entidade; mesmo que suas informações mudem, ele mantém o mesmo identificador.
- **Exemplo**:
  - **CPF**: Identificador de uma pessoa no contexto governamental.

---

## 3. Agregados
- **Definição**: Um *Aggregate* é um cluster de entidades e objetos de valor que devem ser persistidos juntos de forma atômica.
- **Conceitos**:
  - **Aggregate Root (Raiz do Agregado)**: A classe principal do agregado que expõe métodos públicos e manipula o comportamento do mesmo.
  - Todo Aggregate Root é uma entidade, mas nem toda entidade é um Aggregate Root.

---

## 4. Eventos de Domínio
- **Definição**: Eventos gerados a partir de mutações em um agregado.
- **Função**:
  - Permitem a interação com outros sistemas e agregados sem acoplamento.
  - Proporcionam consistência eventual.
- **Próxima Aula**: Será aprofundado o tema dos eventos de domínio e como utilizá-los na arquitetura limpa (CleanArc).

---

## Conclusão
A aula revisou rapidamente os principais conceitos dos padrões de DDD, preparando os alunos para o aprofundamento em eventos de domínio nas próximas aulas. O entendimento desses padrões é fundamental para a construção de sistemas robustos e bem estruturados.

---

## Pontos Importantes para Estudo
- **Revisar os conceitos de Value Objects e Entidades**.
- **Entender a diferença entre Aggregate e Aggregate Root**.
- **Familiarizar-se com o conceito de Eventos de Domínio e sua aplicação**.
- Preparar-se para discutir como integrar eventos na arquitetura CleanArc na próxima aula.



---

## modulo_9_11375.mp4

# Resumo da Aula sobre DDD Patterns

## Introdução
Na aula de hoje, revisamos rapidamente os *padrões de DDD* (Domain-Driven Design), com foco na *modelagem tática*. A seguir, abordaremos os principais conceitos discutidos.

## 1. Value Objects (Objetos de Valor)
- **Definição**: Objetos cuja identificação é feita através de seus valores.
- **Exemplos**:
  - *CNPJ*: A identificação é o número do CNPJ.
  - *Endereço*: Identificado por seus atributos como rua, número e complemento, não possui um ID exclusivo.

## 2. Entidades
- **Definição**: Objetos que possuem um identificador único (ID).
- **Características**:
  - Os atributos podem ser alterados conforme as regras de negócio, mas o ID permanece constante.
- **Exemplo**: 
  - *Customer*: Um cliente é identificado por um ID único, como um CPF. Mudanças em atributos como nome ou documento não alteram sua identidade.

## 3. Agregado (Aggregate)
- **Definição**: Um conjunto de entidades e objetos de valor que representam um conceito no domínio.
- **Características**:
  - Define um limite transacional, ou seja, as operações dentro do agregado devem ser realizadas de forma atômica.
  
### 3.1. Aggregate Root (Raiz de Agregação)
- **Definição**: A entidade principal do agregado que expõe métodos públicos para manipulação do seu comportamento.
- **Importante**: 
  - Todo Aggregate Root é uma entidade com um identificador único, mas nem toda entidade é um Aggregate Root.

## 4. Domain Events (Eventos de Domínio)
- **Definição**: Eventos gerados a partir de mutações em um agregado.
- **Função**:
  - Propagar informações para outros sistemas ou pacotes, permitindo a interação entre agregados sem acoplamento.
- **Consistência**: A transmissão de eventos ocorre com consistência eventual.

## Conclusão
Na aula, revisamos os principais conceitos dos *padrões de DDD* e sua aplicação na modelagem tática. Na próxima aula, vamos aprofundar no tema dos *Domain Events*, sua produção e integração na arquitetura *CleanArc*.

## Próximos Passos
- **Próxima Aula**: Estudo detalhado sobre *Domain Events* e sua utilização na arquitetura limpa, especialmente no contexto de "Subscribe Customer to Events".



---

## modulo_9_11376.mp4

# Resumo da Aula: Aplicação do Padrão Presenter na Arquitetura

## Introdução
- Apresentação e boas-vindas.
- Tema da aula: *Presenter* na arquitetura de software.
- Importância do uso do *Presenter* em casos de uso específicos.

## Estrutura do Presenter
### Definição da Interface Presenter
- Criação da interface chamada **Presenter** na aplicação:
  - Dois parâmetros: *IN* e *OUT*.
  - *OUT* deve conter métodos como *PRESENT* e *INPUT*.
  - Possibilidade de incluir um parâmetro que recebe *THROWABLE* para tratamento de erros.

### Implementação do Presenter
1. **Método Dinâmico**:
   - Adicionar um segundo método no caso de uso que retorna um tipo dinâmico.
   - O *PRESENTER* deve ser passado como argumento.
   - Tratamento de erros usando *TRY, CATCH*.

2. **Casos Especiais**:
   - O caso *NULLARY* não tem parâmetro, mas possui *OUTPUT*.
   - O caso *UNIT* é *VOID* e não faz sentido usar *PRESENTER*.

## Exemplo Prático
### Criando o Presenter para o Customer
- Criação de uma nova pasta chamada **PRESENTERS**:
  - Implementação do Presenter: `GETCUSTOMER.OUTPUT.BYID.HTTP.RESPONSEENTITY`.
  - Uso de *OPTIONAL* para retorno quando necessário.

### Lógica de Retorno
- Definição do retorno em caso de erro:
  - Utilização de `RESPONSE NOT FOUND`.
- Uso de *LOGGER* para registrar erros.

### Cenário de Uso
- Demonstração de teste integrado:
  - Adição de um teste para obter cliente por ID.
  - Implementação de diferentes respostas com base no cabeçalho *xpublic*.

## Flexibilidade do Padrão Presenter
- Possibilidade de criar diferentes implementações do Presenter:
  - Um que retorna *RESPONSEENTITY* e outro que retorna *STRING*.
- Customização da resposta do endpoint conforme a necessidade.

## Considerações sobre o Spring Framework
- O Spring cobre *CONTENT NEGOTIATION*:
  - Respostas diferentes com base em *ACCEPT* headers.
- Comparação com o padrão de *INTERFACE ADAPTER*:
  - O Controller do Spring já implementa esse padrão.

## Conclusão
- O padrão *Presenter* é flexível e permite customização das respostas sem alterar o Controller ou o caso de uso.
- Importância de manter a arquitetura limpa e organizada conforme as diretrizes do Uncle Bob.

## Pontos Finais
- A aplicação do padrão *Presenter* proporciona:
  - Flexibilidade na apresentação dos resultados.
  - Redução do acoplamento entre componentes.
  - Facilidade de manutenção e evolução do código.

---

Espero que este resumo ajude nos seus estudos sobre a aplicação do padrão Presenter na arquitetura de software!



---

## modulo_9_11458.mp4

# Resumo da Aula: Aplicando o Presenter na Arquitetura

## Introdução
- O foco da aula é a aplicação do padrão *Presenter* na arquitetura de software.
- A abordagem que será apresentada é utilizada no Mercado Livre.
- Discussão sobre o uso de *Presenters* em conjunto com o Spring será feita ao final.

## Conceito de Presenter
- O *Presenter* é uma interface que possui dois parâmetros: *IN* e *OUT*.
- **Parâmetros**:
  - *IN*: entrada do caso de uso.
  - *OUT*: saída do caso de uso.
- O *Presenter* pode ser configurado para lidar com erros (exemplo: *THROWABLE*).

## Implementação do Presenter
1. **Criação da Interface Presenter**:
   - Criar uma nova interface chamada `Presenter` na aplicação.
   - Definir métodos que manipulam *IN* e *OUT*.

2. **Modificação no Caso de Uso**:
   - Criar um segundo método no caso de uso que aceita um *Presenter* como parâmetro.
   - O método deve retornar um tipo dinâmico, permitindo flexibilidade.

3. **Tratamento de Erros**:
   - Implementar lógica de *TRY-CATCH* para gerenciar erros no caso de uso.
   - Retornar o resultado esperado se não houver erros.

## Cenário Prático: GET CUSTOMER
- Criar uma nova pasta chamada `PRESENTERS` no módulo REST.
- Implementar o *Presenter* para o caso de uso `GETCUSTOMER`.

### Exemplo de Implementação
- Criar `GETCUSTOMER.OUTPUT.BYID.HTTP.RESPONSEENTITY` que implementa o *Presenter*.
- Usar *OPTIONAL* para gerenciar a ausência de valores retornados.
- Implementar o método `PRESENT` para gerar a resposta.

### Benefícios do Padrão Presenter
- Flexibilidade para alterar a resposta do caso de uso sem impactar o controlador.
- Possibilidade de retornar diferentes tipos de resposta (ex: *STRING*, *RESPONSEENTITY*).

## Testes Integrados
- Criar e executar testes integrados para validar a implementação.
- Testar diferentes cenários, incluindo a manipulação de cabeçalhos de requisição.

## Injeção de Dependências
- Discutir a possibilidade de injetar *Presenters* no controlador.
- A injeção de dependências deve ser feita de forma a manter a flexibilidade.

## Considerações sobre o Spring
- O Spring suporta *Content Negotiation* que pode facilitar a implementação de *Presenters*.
- O uso de *Content-Type* e *Accept* para personalizar as respostas.

## Recapitulando
- O padrão *Presenter* foi adicionado como um parâmetro no caso de uso, permitindo a modificação flexível da resposta.
- O *Controller* não deve conhecer a implementação do *Presenter*, apenas a interface.

## Conclusão
- O padrão *Presenter* oferece uma maneira eficaz de separar a lógica de apresentação da lógica de negócios.
- Sua implementação permite a adaptação do formato de resposta sem alterar outros componentes da arquitetura.

## Dicas para Estudo
- **Revisar conceitos**: Entender bem o que é um *Presenter* e como ele se encaixa na arquitetura limpa.
- **Praticar**: Implementar cenários de teste e brincar com diferentes implementações de *Presenters*.
- **Explorar o Spring**: Ver como o Spring pode ser usado para gerenciar *Presenters* e outras dependências.



---

## modulo_9_11459.mp4

# Resumo da Aula sobre o Padrão Presenter

## Introdução
- O padrão Presenter é uma abordagem interessante no desenvolvimento de aplicações, especialmente em arquiteturas que utilizam casos de uso.
- O foco da aula é demonstrar como implementar o Presenter na arquitetura, além de discutir seu uso em conjunto com o Spring.

## Estrutura do Presenter
### Criação da Interface Presenter
1. Navegar até a camada de **Application**, no **Search Main**.
2. Criar uma nova interface chamada **Presenter** com dois parâmetros: **IN** e **OUT**.
   - **OUT**: Representa o resultado a ser apresentado.
   - **INPUT**: Representa a entrada para o Presenter.
   - É possível incluir um terceiro parâmetro para tratamento de erros: **THROWABLE**.

### Aplicação do Presenter
- Criar um segundo método no caso de uso que receba um **PRESENTER**.
  - O **IN** do Presenter será o **OUTPUT** do caso de uso.
  - O **OUTPUT** do Presenter será dinâmico.
- Utilizar sobrecargas para facilitar a implementação:
  - Exemplo: `PRESENTER.PRESENTOUTPUT.EXECUTEINPUT`.

### Tratamento de Erros
- Implementar a lógica de tratamento de erros com `TRY`, `CATCH`, e `THROWABLE`.
- Retornar o resultado esperado ou um erro apropriado.

## Implementação Prática
### Cenário com o Customer
1. Criar uma nova pasta chamada **PRESENTERS** na camada de **REST**.
2. Criar uma classe chamada **GETCUSTOMER** que implementa o Presenter.
   - A classe deve retornar um **RESPONSEENTITY**.
   - Utilizar **OPTIONAL** para o retorno, já que o método pode não encontrar o cliente.

### Mapeamento de Respostas
- Implementar o mapeamento de respostas com base nos dados retornados pelo caso de uso.
- Exemplo de resposta: se o cliente não for encontrado, retornar `RESPONSE NOT FOUND`.

## Vantagens do Padrão Presenter
- Flexibilidade na modificação das respostas sem alterar o controlador ou o caso de uso.
- Possibilidade de retornar diferentes tipos de dados (ex: `STRING`, `HTTP RESPONSE`).
- Implementação de critérios dinâmicos através de parâmetros de entrada.

## Injeção de Dependências e Spring
- O Presenter pode ser injetado dentro do controlador, mantendo a flexibilidade.
- Discussão sobre a utilização do Spring como framework que já implementa conceitos de *content negotiation*.
  - O Spring lida com diferentes tipos de resposta baseando-se no cabeçalho da requisição.

## Observações Finais
- A importância de manter a responsabilidade única (Single Responsibility Principle) nas implementações.
- O Presenter deve ser utilizado para apresentar resultados de maneira flexível e adaptativa, sem acoplamento excessivo ao framework utilizado.
- O padrão é eficaz para customizar retornos de métodos sem a necessidade de alterar o controlador ou o caso de uso.

## Conclusão
- A implementação do padrão Presenter oferece uma maneira flexível e organizada de lidar com a apresentação de dados em aplicações.
- Encerramento da aula com a expectativa de que os alunos tenham compreendido a importância e a aplicação do Presenter na arquitetura de software.



---

## modulo_9_11460.mp4

# Resumo da Aula sobre o Padrão Presenter

## Introdução
Na aula de hoje, foi abordado o uso do padrão *Presenter* na arquitetura de software, com foco em como aplicá-lo em casos de uso. O instrutor também mencionou a relação entre *Presenters* e o framework *Spring*.

## Objetivos da Aula
- Apresentar o conceito e a implementação do padrão *Presenter*.
- Discutir a aplicação do *Presenter* em casos de uso.
- Explorar a integração com o *Spring*.

## O Padrão Presenter

### Criação da Interface Presenter
- Criar uma nova interface chamada **Presenter** na camada de aplicação.
- A interface terá dois parâmetros:
  - **IN**: Entrada do Presenter.
  - **OUT**: Saída do Presenter.
- Estrutura básica:
  - `OUT PRESENT`
  - `INPUT`

### Implementação do Presenter
1. **Métodos do Presenter**:
   - Criar métodos que recebem um *Presenter* como parâmetro.
   - O *Presenter* deve manipular a saída do caso de uso.
2. **Tratamento de Erros**:
   - Integrar o tratamento de erros utilizando `TRY`, `CATCH` e `THROWABLE`.
   - Retornar a saída do *Presenter* em caso de sucesso ou erro.

### Exemplo Prático
- Criar um *Presenter* para o uso do caso de **GETCUSTOMER**.
- Implementar o retorno de um **RESPONSEENTITY**.
- Adicionar lógica para retornar diferentes tipos de resposta (ex: JSON ou String) com base em cabeçalhos de requisição.

## Vantagens do Padrão Presenter
- Flexibilidade na modificação da resposta do caso de uso sem alterar o controlador.
- Possibilidade de retornar diferentes formatos de resposta, como:
  - **HTML**
  - **JSON**
  - **Strings**
- Separação de preocupações, respeitando o princípio da *Single Responsibility*.

## Integração com o Spring
- O *Spring* já implementa muitos conceitos que podem ser utilizados em conjunto com o padrão *Presenter*.
- O *Spring* oferece suporte a *Content Negotiation*, permitindo a negociação do tipo de resposta com base nos cabeçalhos da requisição.
- **Considerações**:
  - O acoplamento ao framework pode ser um desafio ao implementar *Presenters*.

## Considerações Finais
- O padrão *Presenter* permite que diferentes formatos de resposta sejam manipulados sem impactar o controlador ou os casos de uso.
- A implementação do *Presenter* pode ser feita de forma a garantir que a lógica de apresentação esteja separada da lógica de negócio.
- O uso do *Spring* pode facilitar a implementação, mas é importante estar atento ao nível de acoplamento.

## Conclusão
O instrutor enfatizou a importância da flexibilidade e da separação de preocupações na arquitetura de software, destacando como o padrão *Presenter* pode contribuir para isso. A aula foi encerrada com um convite para a próxima sessão.



---

## modulo_9_11461.mp4

# Resumo da Aula sobre Clean Architecture e Gateways

## Introdução
- A aula aborda o conceito de **gateways** dentro do contexto da **Clean Architecture**.
- O palestrante menciona a relação entre Clean Architecture e **Domain-Driven Design (DDD)**.

## Conceitos Principais

### O Que São Gateways?
- Gateways representam a **porta de saída do núcleo da aplicação**.
- Eles são utilizados para acessar recursos externos, como:
  - Sistemas de arquivos
  - Processos remotos
  - Bancos de dados

### Diferença entre Repository e Gateway
- O padrão **Repository** é frequentemente associado ao modelo de domínio (domain model).
- A nomenclatura muda de `CustomerRepository` para `CustomerGateway` quando se utiliza o padrão gateway.
- Gateways podem ser usados em diferentes contextos:
  - Acesso a dados
  - Interação com serviços externos

## Padrões Relacionados
- **Data Mapper**: Um padrão para mapear objetos de domínio para banco de dados.
- **Table Data Gateway**: Um objeto que atua como um gateway para uma base de dados.

## Aplicações de Gateways
- Exemplo de uso de gateways na camada de aplicação:
  - Acesso a um sistema de cache.
  - Implementação de métodos como `evict`, `put` e `get` em um gateway de cache.
  
### Exemplos de Métodos de Gateway
- `isPartnerEligibleToSomething`
- `execute`
- Métodos que indicam claramente a funcionalidade de um gateway.

## Vantagens da Clean Architecture
- Permite mudar a camada de persistência sem alterar o núcleo da aplicação.
- Exemplo: Mudar de MySQL para um banco de documentos apenas alterando a implementação do gateway.

## Desafios com Frameworks
- A utilização de frameworks como **Spring** pode obscurecer o valor dos **Interface Adapters**.
- A abstração do framework permite mudar componentes, como o **HTTP Router**, sem reescrever a aplicação.

## Considerações Finais
- O palestrante destaca a flexibilidade da Clean Architecture na proteção das **Application Business Rules** e **Enterprise Business Rules**.
- O código fonte dos exemplos abordados na aula estará disponível no repositório do GitHub.

## Contato e Recursos
- O palestrante se coloca à disposição para dúvidas e sugestões, mencionando seu Instagram e LinkedIn.
- Link do repositório do GitHub: `github.dev/devfullcycle/mba-hexagonal-architecture`.

## Conclusão
- A aula conclui que tanto o padrão **Gateway** quanto o **Repository** são válidos e podem ser utilizados conforme a necessidade do projeto. 
- A flexibilidade e a separação de preocupações são essenciais na arquitetura de software.

---

### Dicas para Estudo
- **Rever a documentação** sobre Clean Architecture e DDD.
- **Praticar a implementação** de gateways em projetos pequenos.
- **Explorar alternativas** a frameworks populares para entender melhor a abstração.



---

## modulo_9_11462.mp4

# Resumo da Aula sobre Gateways em Clean Architecture

## Introdução
Nesta aula, o professor aborda a última peça do Clean Architecture, focando especificamente nos *gateways*. Ele relaciona a importância dos gateways com o *Domain-Driven Design* (DDD) e discute como eles são utilizados na arquitetura de software.

## Conceitos Principais

### O que são Gateways?
- **Gateways** servem como a porta de saída do núcleo da aplicação, permitindo que a camada de Application Business Rules acesse recursos externos.
- O padrão **repository** é mencionado, mas o uso de **gateways** é enfatizado, especialmente em contextos onde o *domain model* não é amplamente utilizado.

### Diferença entre Repository e Gateway
- **CustomerRepository** é substituído por **CustomerGateway**, refletindo uma mudança de foco.
- Gateways podem acessar recursos fora da aplicação, como:
  - Sistemas de arquivos
  - Processos remotos
  - Acesso a bancos de dados (ex: *Table Data Gateway*)

## Exemplos de Uso de Gateways
- Os gateways podem ser usados dentro da camada de aplicação para acessar diferentes tipos de armazenamento, como:
  - **Cache**: Implementações de métodos como `get`, `put` e `evict`.
  - **Verificações de elegibilidade**: Exemplo de método `isPartnerEligibleToSomething`.

### Integração com Frameworks
- Os gateways oferecem uma interface que pode estar acoplada ou não ao framework utilizado, permitindo flexibilidade na implementação.
- O professor menciona a dificuldade de observar o valor dos adapters de interface no Spring, onde a integração é mais rígida.

## Benefícios do Clean Architecture
- Permite a mudança da camada de persistência (ex: de MySQL para um banco de documentos) sem alterar o núcleo da aplicação, apenas mudando a implementação do gateway.
- Facilita a adaptação a diferentes frameworks e tecnologias sem a necessidade de refatoração extensa.

## Considerações Finais
- O professor destaca a relevância dos gateways e como eles podem ser utilizados em conjunto com o DDD ou como uma alternativa ao padrão repository.
- Ele convida os alunos a explorar o código fonte disponível no GitHub e se disponibiliza para esclarecer dúvidas.

## Recursos Adicionais
- Código fonte disponível em: [GitHub - mba hexagonal architecture](https://github.com/devfullcycle/mba-hexagonal-architecture)
- Contato: Instagram [@deploy_dc](https://instagram.com/deploy_dc) e LinkedIn.

## Conclusão
A aula foi uma introdução aos gateways no contexto do Clean Architecture, discutindo suas aplicações e benefícios, além de fornecer exemplos práticos e recomendações sobre como utilizá-los efetivamente em projetos de software.



---

## modulo_9_11463.mp4

# Resumo da Aula sobre Gateways no Clean Architecture

## Introdução
- A aula aborda a última parte do Clean Architecture: os *gateways*.
- O *Domain-Driven Design* (DDD) já existia antes da proposta do Clean Architecture, mas não foi mencionado por Uncle Bob.

## O que são Gateways?
- **Definição**: Os gateways representam a *porta de saída* do núcleo da aplicação, especificamente da camada de *Application Business Rules*.
- **Padrão Utilizado**: O padrão *repository* é mencionado, mas o foco está no padrão *gateway*.

### Comparação entre Repository e Gateway
- **Repository**: Nomeado como `CustomerRepository`.
- **Gateway**: Nomeado como `CustomerGateway`.
- **Diferença Principal**: O gateway é uma forma de acessar recursos externos ou sistemas, enquanto o repositório lida com a persistência de dados.

## Importância dos Gateways
- Os gateways permitem o acesso a qualquer recurso fora da aplicação, como:
  - Sistema de arquivos
  - Processos remotos
  - Outros sistemas externos

## Exemplos de Uso de Gateways
- **Exemplo em MercadoLivre**: Utilização do padrão gateway em vez do padrão repository, especialmente em equipes que não usam muito o DDD.
- **Exemplo de Implementação**:
  - `subscribeCustomerToEvent`
  - `getPartnerPorId`
- **Uso em Cache**: Implementação de um gateway para acesso a uma camada de cache, com métodos como:
  - `get`
  - `put`
  - `evict`

## Aplicações dos Gateways
- Os gateways são usados para:
  - Acesso a sistemas de armazenamento (cache, file system)
  - Determinação de elegibilidade, como `isPartnerEligibleToSomething`.

## Integração com Clean Architecture
- Os gateways podem ser usados como interfaces dentro da camada de aplicação.
- É possível trabalhar apenas com gateways, sem utilizar repositórios.

### Flexibilidade do Clean Architecture
- *Mudança de Persistência*: Alterar a camada de persistência (ex: de MySQL para um banco de documentos) sem modificar o núcleo da aplicação.
- *Abstração do Framework*: Mudanças em frameworks (ex: Spring para Quarkus) podem ser feitas criando novos adaptadores para o HTTP Router.

## Considerações Finais
- O Clean Architecture protege as *Application Business Rules* e *Enterprise Business Rules* das *Interface Adapters* e dos *Frameworks and Drivers*.
- O material de código estará disponível no repositório do GitHub.

## Contato e Recursos
- Para dúvidas ou sugestões, os alunos podem entrar em contato pelo Instagram (@deploy_dc) ou LinkedIn.
- Todos os códigos e materiais adicionais estão disponíveis no repositório GitHub: `mba hexagonal architecture`.

## Conclusão
- A aula conclui a série sobre Clean Architecture, enfatizando a importância e a flexibilidade dos gateways na arquitetura de software.



---

## modulo_9_11464.mp4

# Resumo da Aula sobre Gateways na Clean Architecture

## Introdução
- A aula aborda a última peça do Clean Architecture: **gateways**.
- O conceito de **Domain-Driven Design (DDD)** é mencionado, embora não tenha sido destacado por Uncle Bob no livro.

## O que são Gateways?
- **Gateways** são a *porta de saída* do núcleo da aplicação, especificamente da camada de **Application Business Rules**.
- Exemplos de uso incluem acesso a recursos externos como sistemas de arquivos ou processos remotos.

### Comparação com Repository
- No contexto de DDD, o termo **CustomerRepository** pode ser substituído por **CustomerGateway**.
- A principal diferença é a terminologia, e a abordagem pode variar dependendo da equipe e da aplicação.

## Padrões Relacionados
- **Patterns of Enterprise Application Architecture**:
  - O livro discute o padrão gateway como meio de acessar recursos fora da aplicação.
  - Dois padrões mencionados:
    - **Data Mapper**
    - **Table Data Gateway**
  
### Como Usar Gateways
- Gateways podem ser utilizados em diversas camadas, incluindo a camada de **application**.
- Exemplo prático: uso de um gateway para gerenciar acesso a um cache.
  - Métodos sugeridos: `evict`, `put` e `get`.

## Exemplos de Aplicação
- **isPartnerEligibleToSomething**: um exemplo de nome de gateway que poderia ser utilizado.
- A flexibilidade de usar gateways permite acessar diferentes tipos de armazenamento sem acoplar a lógica ao repositório.

## Estrutura do Código
- A estrutura pode ser organizada em pacotes, onde apenas as interfaces são expostas, mantendo o núcleo desacoplado.
- A implementação pode ser feita de forma a não depender do framework utilizado.

## Vantagens da Clean Architecture
- Permite mudanças na camada de persistência sem alterar o núcleo da aplicação.
- Exemplos de mudanças que podem ser feitas:
  - Trocar de MySQL para um banco de documentos.
  - Utilizar um Key-Value Store (KVE) com simples alterações na implementação do gateway.

## Considerações Finais
- O valor do **Interface Adapter** pode não ser tão evidente no ecossistema do Spring devido à sua abordagem de ponta a ponta.
- Em outras bibliotecas ou configurações manuais, o valor se torna mais claro, permitindo que os desenvolvedores mudem a camada de roteamento sem reescrever a aplicação.

## Recursos e Contato
- Todo o código discutido está disponível no repositório do GitHub: 
  - `mba hexagonal architecture` (github.dev/devfullcycle/mba-hexagonal-architecture).
- Dúvidas e sugestões podem ser enviadas através:
  - Instagram: `@deploy_dc`
  - LinkedIn
  - Chat de suporte

## Conclusão
- A aula encerra com a expectativa de que os alunos tenham compreendido os conceitos abordados e a importância dos gateways na Clean Architecture.



---

## modulo_9_11552.mp4

# Resumo da Aula sobre Arquitetura Hexagonal

## Introdução
- A aula é uma conclusão do módulo sobre *Arquitetura Hexagonal*.
- O foco é compartilhar considerações finais e dicas para aprofundamento.

## Recapitulação do Conteúdo
- **Transição do Código Espaguete**: 
  - O projeto inicial tinha *spaghetti code* e acoplamentos excessivos.
  - A aplicação foi reorganizada em dois pacotes principais:
    - **Application**: Contém casos de uso e repositórios.
    - **Infrastructure**: Inclui interfaces, adaptadores e atores.

### Estrutura do Projeto
- **Controladores**:
  - Foram transformados em adaptadores REST, como:
    - `CustomerController`
    - `EventController`
    - `PartnerController`
  - Cada controlador agora possui seu próprio caso de uso, evitando acoplamentos desnecessários.

- **Drivers e Atores**:
  - Adição do *GraphQL* como um novo driver.
  - Reuso de casos de uso entre REST e GraphQL para maior eficiência.

- **DTOs (Data Transfer Objects)**:
  - Compartilhamento de DTOs entre REST e GraphQL.
  - Atenção necessária para evitar problemas de acoplamento entre as duas camadas.

## Configurações e Casos de Uso
- **Configurações**:
  - Casos de uso configurados manualmente na camada de Application.
  - Possibilidade de utilizar CDI do Java para configuração automática.

- **Repositórios**:
  - Diferentes dos repositórios JPA, são interfaces que se comunicam com um *Data Mapper*.

### Anatomia dos Casos de Uso
- Estrutura dos casos de uso dividida em:
  - **Customer**
  - **Partner**
  - **Event**

## Considerações sobre Eventos de Domínio
- Discussão sobre a manipulação de agregados usando *Domain Events*.
- Importância da manipulação correta de IDs para garantir a integridade de dados.

## DDD (Domain-Driven Design)
- Introdução a conceitos de DDD:
  - Agregados, Value Objects e Entidades.
  - Distribuição da complexidade entre classes para um melhor design.

### Exemplos de Implementação
- Uso de *Factory Methods* para simplificar a criação de objetos complexos.
- Validações encapsuladas em objetos de valor, como CPF e CNPJ.

## Testes
- Criação de uma abstração para testes de integração e unitários.
- Importância de testes rápidos e independentes.
- Estratégias de teste conforme a pirâmide de Martin Fowler:
  - **Testes Unitários**
  - **Testes de Integração**
  - **Testes End-to-End**

## Dicas Finais
- Recomendação de dividir o projeto em sub-módulos no Gradle:
  - **Application**: Sem dependências externas.
  - **Infrastructure**: Com dependências necessárias.
- Utilização de ferramentas, como *ArcUnit*, para garantir a conformidade da arquitetura.

## Conclusão
- A aula conclui o módulo e prepara os alunos para futuras discussões sobre *Clean Architecture*.
- Importância de seguir boas práticas para evitar acoplamentos indesejados e manter a arquitetura limpa.

---

### Observações Finais
- Implementar as mudanças sugeridas pode melhorar a robustez da aplicação.
- Praticar os conceitos discutidos é essencial para a aplicação prática da *Arquitetura Hexagonal*.



---

## modulo_9_11553.mp4

# Resumo da Aula sobre Arquitetura Hexagonal

## Introdução
- Finalização do módulo de arquitetura hexagonal.
- Recapitulação do que foi abordado nas aulas anteriores.

## Estrutura da Aplicação
1. **Divisão em Pacotes**
   - **Pacote `application`**:
     - Casos de uso.
     - Repositórios.
     - Domínio.
   - **Pacote `infrastructure`**:
     - Adaptadores de interface.
     - Drivers e atores dirigidos.

2. **Controllers como Adaptadores**
   - Transformação dos controllers em adaptadores REST.
   - Exemplos de controllers adaptadores: `customer controller`, `event controller`, `partner controller`.
   - Cada adaptador possui casos de uso específicos, sem acoplamento ou regras de negócio.

3. **Integração com GraphQL**
   - Implementação de GraphQL para evitar duplicação de regras de negócio na camada de controller.
   - Compartilhamento de DTOs entre as camadas REST e GraphQL, com cautela sobre possíveis alterações.

## Casos de Uso e Configuração
- **Configuração Manual**:
  - Casos de uso configurados manualmente.
  - Possibilidade de usar CDI do Java para injeção de dependências.
  
- **Repositórios**:
  - Interfaces de repositórios não são JPA, são adaptadores que levam a um Data Mapper ou ORM.

## DDD e Eventos de Domínio
- Discussão sobre a manipulação de agregados e a necessidade de aplicar *Domain Events*.
- Importância de manter as validações e a estrutura adequada dos casos de uso.

### Agregados e Objetos de Valor
- Definição de um agregado como uma entidade imutável identificada por um ID.
- Uso de *Factory Methods* para facilitar a construção de objetos de valor.
- Encapsulamento de validações nos objetos de valor.

### Exceções
- Criação de uma exceção performática com parâmetros específicos para melhorar a performance do sistema.

## Testes
1. **Abstrações de Teste**:
   - Criação de uma abstração de `IntegrationTest`.
   - Importância dos testes unitários e integrados.

2. **Classificação de Testes**:
   - Definição de testes unitários e integrados.
   - Exemplo de testes end-to-end.

## Dicas e Recomendações
- **Sub-módulos no Gradle**:
  - Criação de sub-módulos para `application` e `infrastructure` para evitar acoplamentos indesejados.
  
- **Uso de ArcUnit**:
  - Testes de arquitetura para garantir a conformidade com a estrutura do projeto.

## Conclusão
- Encorajamento para aplicar o que foi aprendido na prática.
- Expectativa de continuar o aprendizado na próxima aula.



---

## modulo_9_11554.mp4

# Resumo da Aula sobre Arquitetura Hexagonal

## Introdução
- O objetivo da aula é fazer considerações finais sobre o módulo de arquitetura hexagonal.
- Recapitulação das práticas realizadas na branch chamada *hexagonal arc*.

## Recapitulando a Estrutura da Aplicação
- A aplicação foi dividida em dois pacotes principais:
  - **Application**: Contém casos de uso, repositórios e o domínio.
  - **Infrastructure**: Abrange toda a parte externa do hexágono, incluindo:
    - Interface adapters
    - Drivers
    - Driven actors

### Mudanças Realizadas
- **Controllers** foram transformados em REST:
  - Exemplo: `customer controller`, `event controller`, `partner controller`.
- Cada controller agora possui um caso de uso específico, eliminando o acoplamento e as regras de negócio.
- Introdução de **GraphQL** como um novo driver, facilitando a reutilização de casos de uso.

## Considerações sobre DTOs
- As DTOs (Data Transfer Objects) estão sendo compartilhadas entre REST e GraphQL.
- Recomenda-se cuidado ao adicionar campos a DTOs, pois mudanças em um podem impactar o outro.
- Sugestão: Criar DTOs separados para REST e GraphQL para evitar problemas.

## Configuração dos Casos de Uso
- Os casos de uso estão configurados manualmente.
- Alternativa: Usar a especificação de CDI do Java (Jakarta ou Javax Inject) para configuração automática.

## Repositórios
- Os repositórios não são JPA, mas implementações expostas na camada de *application*.
- Exemplo: `CustomerDatabaseRepository`, que é um interface adapter.

## Casos de Uso
- Casos de uso foram definidos, por exemplo:
  - Customer
  - Partner
  - Event
- Discussão sobre a manipulação de agregados e a implementação de *Domain Events* para melhorar a interação entre casos de uso.

## Fatores Importantes a Considerar
- A manipulação de agregados deve ser feita de forma isolada, utilizando eventos de domínio para disparar reações em outros casos de uso.
- A estrutura do agregado deve ser bem definida:
  - Identificação por um **ID** imutável.
  - Utilização de *factory methods* para facilitar a construção de objetos.

## Testes
- Foi criada uma abstração para testes de integração e testes unitários.
- Importante distinguir entre:
  - Testes **unitários**: Focam em uma única unidade (caso de uso).
  - Testes **integrados**: Envolvem múltiplos componentes, podendo ser mais amplos ou mais restritos.
  
### Pirâmide de Testes
- Referência ao artigo de Martin Fowler sobre a pirâmide prática de testes.
- Dicas sobre a execução eficiente de testes e a importância de manter a unidade dos testes.

## Dicas Finais
- Para o próximo módulo (Clean Architecture):
  - Implementar sub-módulos no Gradle para organizar melhor a estrutura.
  - **Application**: Deve ser puro, sem bibliotecas ou frameworks.
  - **Infrastructure**: Pode incluir bibliotecas e frameworks, mas deve referenciar a camada de *application*.
- Utilizar ferramentas como ArcUnit para garantir a coerência entre pacotes e classes.

## Conclusão
- A aula abordou a importância da arquitetura hexagonal e práticas para otimizar a estrutura do código.
- A próxima aula continuará a construção sobre esses conceitos.

Espero que este resumo ajude no seu estudo sobre arquitetura hexagonal!

