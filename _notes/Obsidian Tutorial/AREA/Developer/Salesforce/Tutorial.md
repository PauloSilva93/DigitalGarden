# Salesforce Certified Platform Developer I
- [Salesforce Certified Platform Developer I](#salesforce-certified-platform-developer-i)
  - [Salesforce Fundamentals](#salesforce-fundamentals)
    - [MVC Pattern](#mvc-pattern)
    - [Core/Standard CRM Objects](#corestandard-crm-objects)
    - [AppExchange](#appexchange)
    - [Packages](#packages)
    - [Declarative customization:](#declarative-customization)
      - [Fields and validations rules](#fields-and-validations-rules)
      - [Declarative Automation Tools](#declarative-automation-tools)
  - [Data Modeling and Management](#data-modeling-and-management)
    - [Terminologia Salesforce](#terminologia-salesforce)
    - [Tipos de associações e relacionamentos](#tipos-de-associações-e-relacionamentos)
    - [Schema Builder](#schema-builder)
    - [Importing Data](#importing-data)
    - [Exporting Data](#exporting-data)
    - [More about Formula Fields](#more-about-formula-fields)
    - [More about Rollup Sumary Fields](#more-about-rollup-sumary-fields)
  - [Process Automation and Logic](#process-automation-and-logic)
    - [Workflow Rules](#workflow-rules)
    - [Process Builder](#process-builder)
      - [Flow Builder](#flow-builder)
    - [Approval Process](#approval-process)
    - [Visual Flows](#visual-flows)
    - [Apex: Variables, Constants, Methods and Expressions](#apex-variables-constants-methods-and-expressions)
    - [Apex: Flow Control Statements](#apex-flow-control-statements)
    - [Operadores lógicos](#operadores-lógicos)
    - [Copy/Pass by Reference/Value](#copypass-by-referencevalue)
    - [Clonando objetos](#clonando-objetos)
    - [Apex Classes and Interfaces: OOP and Access Modifiers](#apex-classes-and-interfaces-oop-and-access-modifiers)
    - [SOQL](#soql)
      - [Introdução](#introdução)
      - [WHERE](#where)
      - [Expressões após WHERE](#expressões-após-where)
      - [Aggregate functions](#aggregate-functions)
      - [Pseudônimo](#pseudônimo)
      - [Retorno de SOQL queries](#retorno-de-soql-queries)
        - [Mais sobre aggregate functions](#mais-sobre-aggregate-functions)
      - [Acessando objetos relacionados via SOQL](#acessando-objetos-relacionados-via-soql)
      - [Semi-joins e Anti-joins](#semi-joins-e-anti-joins)
      - [SOQL Dinâmico](#soql-dinâmico)
    - [SOSL](#sosl)
      - [Introdução](#introdução-1)
      - [Diferenças de SOQL e SOSL](#diferenças-de-soql-e-sosl)
    - [DML](#dml)
      - [Introdução](#introdução-2)
      - [Mais sobre a classe Database](#mais-sobre-a-classe-database)
    - [Savepoint e Rollback](#savepoint-e-rollback)
    - [Apex Triggers](#apex-triggers)
      - [Introdução](#introdução-3)
      - [Trigger Context Variables](#trigger-context-variables)
      - [Método addError()](#método-adderror)
    - [Melhores práticas com Apex triggers](#melhores-práticas-com-apex-triggers)
    - [Limites de Governança](#limites-de-governança)
    - [Ordem de execução](#ordem-de-execução)
    - [Lidando com exceptions](#lidando-com-exceptions)
      - [Throw exceptions e Custom Exception Class](#throw-exceptions-e-custom-exception-class)
    - [Segurança em Apex](#segurança-em-apex)
      - [Segurança de registros](#segurança-de-registros)
      - [Segurança de classes](#segurança-de-classes)
    - [Impacto do Apex em mudanças declarativas](#impacto-do-apex-em-mudanças-declarativas)
    - [Técnicas programáticas para prevenir vulnerabilidades de segurança](#técnicas-programáticas-para-prevenir-vulnerabilidades-de-segurança)
    - [Usando ferramentas declarativas e Apex juntos](#usando-ferramentas-declarativas-e-apex-juntos)
      - [Executando Apex a partir de um Flow e Process](#executando-apex-a-partir-de-um-flow-e-process)
      - [Invocable variables](#invocable-variables)
      - [Executando Flows a partir do Apex](#executando-flows-a-partir-do-apex)
    - [Platform Events](#platform-events)
      - [Introdução](#introdução-4)
      - [Como um platform event funciona?](#como-um-platform-event-funciona)
  - [User Interface](#user-interface)
    - [Visualforce](#visualforce)
      - [Introdução](#introdução-5)
      - [Trabalhando com dados do Salesforce na VF](#trabalhando-com-dados-do-salesforce-na-vf)
      - [Apex Properties](#apex-properties)
      - [Standard Controller vs Custom Controller vs Controller Extension](#standard-controller-vs-custom-controller-vs-controller-extension)
      - [Usando recursos estáticos em VF](#usando-recursos-estáticos-em-vf)
      - [Incorporando páginas VF na plataforma Salesforce](#incorporando-páginas-vf-na-plataforma-salesforce)
    - [O framework Lightning Components e suas vantagens](#o-framework-lightning-components-e-suas-vantagens)
      - [Introdução](#introdução-6)
      - [Vantagens](#vantagens)
  - [Testing, Debbuging and Deployment](#testing-debbuging-and-deployment)
    - [Testing Deployment Requirement and Testing Framework](#testing-deployment-requirement-and-testing-framework)
    - [Escrevendo Testes unitários](#escrevendo-testes-unitários)
    - [Gerando dados de teste](#gerando-dados-de-teste)
    - [Executando Apex em Execute Anonymous](#executando-apex-em-execute-anonymous)
    - [Monitorar e Acessar Debug Logs](#monitorar-e-acessar-debug-logs)
    - [Workbench](#workbench)
    - [Deploying Metadata](#deploying-metadata)
      - [Change sets](#change-sets)
      - [Packages](#packages-1)
      - [Ant Migration Tool](#ant-migration-tool)
    - [Salesforce Environments e Sandboxes](#salesforce-environments-e-sandboxes)
    - [Sandbox](#sandbox)
      - [Básico do processamento assíncrono](#básico-do-processamento-assíncrono)
      - [Métodos futuros](#métodos-futuros)
        - [Introdução](#introdução-7)
        - [Sintaxe](#sintaxe)
        - [Exemplo de método futuro com callout](#exemplo-de-método-futuro-com-callout)
        - [Classes de teste](#classes-de-teste)
        - [Melhores práticas](#melhores-práticas)
        - [Pormenores](#pormenores)
      - [Apex de lote](#apex-de-lote)
        - [Introdução](#introdução-8)
        - [Sintaxe](#sintaxe-1)
        - [Exemplo de Apex de lote:](#exemplo-de-apex-de-lote)
        - [Classes de teste](#classes-de-teste-1)
        - [Melhores práticas](#melhores-práticas-1)
      - [Queueable Apex](#queueable-apex)
        - [Introdução](#introdução-9)
        - [Sintaxe](#sintaxe-2)
        - [Exemplo de queueable Apex](#exemplo-de-queueable-apex)
        - [Encadeando jobs](#encadeando-jobs)
        - [Callouts dentro do execute()](#callouts-dentro-do-execute)
      - [Scheduled Apex](#scheduled-apex)
        - [Introdução](#introdução-10)
        - [Sintaxe](#sintaxe-3)
        - [Exemplo](#exemplo)
        - [Classe de teste](#classe-de-teste)
        - [Criando Schedule Apex pela UI](#criando-schedule-apex-pela-ui)
        - [Importante](#importante)
      - [Monitorar Apex assíncrono](#monitorar-apex-assíncrono)
    - [Apex Integration Services](#apex-integration-services)
      - [Apex REST Callouts](#apex-rest-callouts)
        - [Introdução](#introdução-11)
        - [Autorizando um endpoint](#autorizando-um-endpoint)
        - [Métodos HTTP](#métodos-http)
        - [Sintaxe](#sintaxe-4)
        - [Exemplos](#exemplos)
          - [GET](#get)
          - [SET](#set)
        - [Testando Callouts](#testando-callouts)
        - [Exemplo final](#exemplo-final)
        - [Considerações finais](#considerações-finais)
      - [Apex Web Services](#apex-web-services)
        - [Introdução](#introdução-12)
    - [Leads e oportunidades para o Lightning Experience](#leads-e-oportunidades-para-o-lightning-experience)
      - [Criar e converter leads em clientes potenciais](#criar-e-converter-leads-em-clientes-potenciais)
  - [Process Automation Specialist](#process-automation-specialist)
      - [Approval Processes](#approval-processes)
      - [Escolha a ferramenta de automação certa](#escolha-a-ferramenta-de-automação-certa)
- [RESUMÃO DE COISAS QUE NÃO ME APROFUNDEI](#resumão-de-coisas-que-não-me-aprofundei)
  - [Custom Iterators](#custom-iterators)
  - [Classe Limits](#classe-limits)
  - [SFDX e SFDX CLI](#sfdx-e-sfdx-cli)
  - [Schema Class](#schema-class)
  - [Automation Tool Features](#automation-tool-features)
  - [Lightning Web Components (LWC)](#lightning-web-components-lwc)
    - [Criando um LWC:](#criando-um-lwc)

## Salesforce Fundamentals
1.	package.xml é um arquivo contendo metadados de componentes de uma ORG para uso por APIs.
2.	Este site https://packagebuilder.herokuapp.com/ permite gerar o arquivo package.xml de uma ORG específica.
3.	Definir componentes nesse arquivo segue uma estrutura padrão:
```
<types>
    <members>obj1</members>
    <members>obj2</members>
    <members>obj…</members>
    <name>typeName</name>
</types>
```
4.	Executar código em modo anônimo (como no Developer Console): Selecione um trecho de Código > CTRL + SHIFT + P > Execute Anonymous Apex
5.	Executar código SOQL: Selecione um trecho de Código > CTRL + SHIFT + P > Execute SOQL Query

7.	Salesforce – Instâncias vs Ambientes
    * Instâncias se referem a estruturas físicas e virtuais que compartilham os mesmos recursos para rodar o Salesforce (pense em servidores).
    * Org é o identificador que representa uma versão do Salesforce do cliente, contendo metadados e dados dentro de uma instância.
    * Ambiente é uma org usada para determinado propósito (sandbox, homologação, produção, etc).
![[dc.png]]
 
    * A instância e ID da org podem ser consultadas em Setup > Company Information. Exemplo:  
![[org-edition.png]]

### MVC Pattern

![[MVC.png]]

### Core/Standard CRM Objects
* Lead: Pessoas e empresas que foram identificadas como potenciais clientes.
* Account: Pessoas e empresas que estão envolvidas com seu negócio (clientes, concorrentes, parceiros)
* Contact: Pessoas que trabalham em Accounts. Cada Account tem pelo menos um Contact, e um Contact está relacionado a pelo menos um Account.
* Opportunity: Negócio com potencial receita que os representantes de venda monitoram até que o negócio tenha sido fechado (won ou lost).

### AppExchange
* Uma loja de aplicativos, components, serviços de consultoria, etc. disponíveis de forma gratuita ou paga, com demos para apps pagos.

### Packages
* São bundles de componentes de metadata que formam um App ou funcionalidade:
* Podem conter Objetos, Campos, código Apex, Layouts de páginas, template de email, etc.
* São privados, mas podem ser compartilhados via URL
* Para serem acessados publicamente, devem ser publicados no AppExchange ou distribuídos.
* Pacotes tem dois tipos: Managed (podemos entender como um pacote licenciado) e Unmanaged (podemos entender como um pacote open source).
    * **OBS**: Pacotes managed só podem ser criados em orgs Developer Edition.
* As diferenças entre managed packages e unmanaged packages são:

|Tópico|Unmanaged|Managed|
|:-:|:-:|:-:|
|Source code|Disponível para edição livre|Não disponível|
|Usado para|Distribuição freeware, projetos open-source|Vender aplicativos para clientes|
|Atualização|Não pode ser atualizado|Pode ser atualizado|
|Namespace|Não é usado|É obrigatório|
|Distribuição|Via link; Não pode ser controlada|É controlada pois o pacote não pode ser redistribuído|

### Declarative customization:
#### Fields and validations rules
* Formula field: Fórmula como no excel. Pode-se criar uma fórmula num objeto filho que referencie um campo no objeto pai, isso se chama **Cross Object formula**
* Rollup Summary Field: Um tipo de campo disponível apenas num objeto mestre de uma relação mestre-detalhe. Usado para calcular um valor numérico de registros de um campo do objeto filho. Os tipos de resumo são:
    * COUNT
    * SUM
    * MIN
    * MAX
* Validation Rules: Usadas para garantir que os dados atendam certos requisitos condicionais antes de serem criados/atualizados.
  *  São definidas usando uma fórmula que retorna true ou false (onde true quer dizer que um erro ocorreu e o registro não será salvo). Também pode incluir uma mensagem de erro caso retorne true.
  *  Impactam na criação/atualização de dados via API (Data Loader, web-to-lead, web-to-case).
  *  São criadas a partir do gerenciador de objetos do objeto em questão.

#### Declarative Automation Tools
* São 4 ferramentas para automação declarativa:
    * Workflow rules
    * Approval Process
    * Salesforce Flow (produto)
      * Process Builder 
      * Flow Builder (lightning)
    * Visual Workflow

## Data Modeling and Management

### Terminologia Salesforce
* Object: Como uma table num database. Pode ser standard (Account, Contact, Opportunity) ou custom.
* Field: Como uma coluna num database. Pode ser standard ou custom. Os standard fields se dividem em:
    * ID: Número único para cada registro
    * Name: Nome para cada registro
    * System fields: Se subdivivem em:
      * CreatedDate
      * CreatedByid
      * LastModifiedById
      * LastModifiedDate.
    * Relashionship fields: Em vez de primery key e foreign key para definir relacionamento entre objetos, o Force.com usa relashionship fields, que se dividem em 2 tipos:
      * Lookup, Master-Detail.
* Record: É como um registro de uma tabela ou uma linha da tabela.
* Org: Abreviação para organization, contém todos os dados e configurações do Salesforce.
* Force.com: Plataforma que consiste num conjunto de ferramentas, linguagens de programação e APIS nativas, usadas para customizar o Salesforce.
* App: Conjunto de objetos, campos, funcionalidade e configurações para suportar um processo de negócio.
* Tab: É como uma guia comum, mas se refere a um objeto.

### Tipos de associações e relacionamentos
* Existem 3 tipos de associação:  
	![[association-types.png]]

* E existem 2 tipos de relacionamento entre objetos:
  * Lookup
  * Master-detail

A principal diferença é que no lookup os objetos têm ligação fraca, e no master-detail, a ligação é forte. Numa ligação fraca, não existe dependência. Numa ligação forte, caso o objeto pai seja deletado por exemplo, o seu filho também será deletado.

* Para estabelecer um relacionamento do tipo lookup entre dois objetos, cria-se um campo do tipo lookup que aponta para outro objeto.
* Para criar um relacionamento do tipo master-detail, cria-se um campo do tipo master-detail no objeto filho, apontando para o pai do relacionamento (apenas disponível em objetos custom).

* Em relacionamentos do tipo many-to-many, a única forma de criar um relacionamento é através de um terceiro objeto chamado **Junction Object**. Este objeto deverá ser filho de ambos com o tipo master-detail.

* Outros tipos de relacionamento especiais são:
    * Hierarchical: Só disponível para o objeto User se relacionar com outro objeto User.
    * External lookup: Linka um objeto filho standard, custom ou externo à um objeto pai externo pelo seu campo de Id externo.
    * Indirect lookup: Linka um objeto um objeto pai standard ou custom a um objeto filho externo.
    * Self-relationship: Quando um objeto tem uma relação de lookup com ele mesmo.

**OBS:** Campos que referenciam campos de outros objetos poderão ser visíveis na aba `Details` do objeto.

### Schema Builder
* Ferramenta visual para criar e editar objetos, campos e relacionamentos, ao invés de usar o Object Manager:	![[schema-builder.png]]
* OBS: 
  * Campos adicionados pelo Schema Builder não são automaticamente adicionados ao layout da página.
  * Por padrão o nível de segurança de campos custom são definidos como visíveis para internal profiles.

### Importing Data
* Os data sources suportados pelo Salesforce são de formato CSV (comma separated values).  
* Há dois **métodos principais** para se importar dados para o Salesforce:  
  * Data Import Wizard (Setup > Integrations > Data Import Wizard)
    * Importa até 50 mil registros de uma vez
    * Pode detectar e evitar duplicatas
    * Suporta custom objects e alguns standard objects (Accounts, Contacts, Leads, Campaigns, Solutions)
    * Pode desativar o Workflow Rules
  * Data Loader (Setup > Integrations > Data Loader)
    * Importa até 5 milhões de registros de uma vez
    * Aplicação cliente (deve ser instalada)
    * Suporta UI e CLI (portanto pode ser automatizado)
    * Não detecta duplicatas
    * Suporta qualquer object
    * Não pode desativar o Workflow Rules
  
### Exporting Data
Podemos exportar dados para arquivos CSV usando dois **métodos principais**:  
* Salesforce Data Export (Setup > Data > Data Export)
  * Permite exportar dados manualmente (uma vez a cada 6 dias ou 28 dias)
  * E automaticamente (semanal ou mensalmente dependendo da edição)
  * Um email é enviado após o termino a exportação
* Data Loader
  * Não tem restrição na agenda de exportação

### More about Formula Fields
  * Um campo **read-only** calculado em tempo de leitura de página
  * Pode retornar: Checkbox, Currency, Date, Datetime, Number, Percent, Text
  * Pode referenciar campos do próprio Objeto ou do Objeto pai, e objetos relacionados em geral com até 10 níveis
  * Quando usa campos do pai se chama Cross Object formula
  * Pode conter no máximo 3900 caracteres e são calculados usando SOQL no backend
  * O SOQL gerado não pode ultrapassar os 5000 caracteres
  * **Não confundir** com rollup summary field
  * Campos referenciados em fórmulas não podem ser deletados até que as fórmulas sejam deletadas
  * Ao definir um tipo Number com 0 casas decimais com a fórmula `1`, cria-se um Power of One, que é capaz de contar objetos distintos em reports, etc.

### More about Rollup Sumary Fields
Vamos ver na prática como esse campo funciona:
* Account é pai de Opportunity (relacionamento master-detail), apesar do campo em Opportunity que faz referência a Account ser do tipo Lookup, o relacionamento é tratado como master-detail.
* Vamos supor que queremos exibir a quantidade em dinheiro de todas as Opportunities vinculadas a uma Account. Pra isso precisamos somar todos os valores do campo amount em Opportunity e exibir como um campo em Account:
  * Crie um novo campo `Opportunity Amount` em Account:
    * Setup > Object Manager > Account > Fields and Relationships > New > selecione Roll-Up Summary > Next > Field Label: Opportunity Amount > Next > Summarized Object: Opportunities > Select Roll-Up Type: SUM, Field to Aggregate: Amount > Next > Next > Save
* Após a criação do campo, ele aparece na aba Details de um objeto Account, exibindo a soma de todo os valores amount das Opportunities deste objeto:  
  ![[rollup-summary-field.png]]

## Process Automation and Logic

### Workflow Rules
* Workflow é a automatização de processos através de instruções executadas automaticamente.
* Workflow rule é um container para instruções de workflow
* Definidas em um objeto de cada vez
* São disparadas quando algum evento acontece
* São 4 passos para criar uma workflow rule:
1. Defina **o objeto** a qual a regra se aplica
2. Defina **quando** a regra será aplicada
   * Na criação de um registro
   * Na criação e edição de um registro
   * Na criação e quando a edição cumprir certas regras
3. Defina **a regra** a ser aplicada
4. Defina **as ações** da regra
  * As ações podem ser:
    * Criar tarefa
    * Enviar alerta de email
    * Atualizar o próprio registro ou registro vinculado numa relação master-detail
    * Enviar mensagens à sistemas externos
  * O tempo para executá-las pode ser:
    * Imediato
    * Agendado

* Para criar uma workflow rule: Setup > Process Automation > Workflow Rules

### Process Builder
* É uma ferramenta visual de workflow (como o workflow rules, mas com interface gráfica amigável, e muito mais recursos)
* É ativado quando um evento ocorre, assim como uma workflow rule
* Processos consistem em:
  * Regras que determinam quando executar grupos de ação
  * Ações imediatas a serem executadas
  * Ações agendadas a serem executadas
* As vantagens sobre o workflow rules são:
  *  Poder criar um processo inteiro no mesmo lugar em vez de criar várias workflow rules
  *  Múltiplas regras podem ser criadas, em vez de uma só
  *  Atualizar **qualquer registro relacionado**, não só o próprio registro e o registro do pai.
  *  Poder criar registros, quick actions para criar registros, atualizar registros, ou registrar uma chamada
  *  Chamar classes Apex
  *  Usar processos para disparar outros processos
  *  Executar um **Flow** (veremos mais sobre posteriormente)
  *  Postar no Chatter
  *  Enviar para aprovação

Um processo no Process Builder se parece com isto:  
![[process-builder.png]]

* O Process Builder está em: Setup > Process Automation > Process Builder

#### Flow Builder
* Ferramenta point-and-click para criar flows. A parte principal é o canvas:  
![[flow builder-canvas.png]]
* Um flow consiste em 3 blocos de construção
  1. Elementos (1): Aparecem no canvas e são adicionados pelo botão "+" e caem em 3 categorias:
     1. Interação: Usado como coletar dados, executar ações fora do flow e executar subflows. 
     2. Lógica: Usado para atribuições, decisões, loops, etc.
     3. Dados: Usado para CRUD de registros.
  2. Conectores (2): Conectam elementos e definem o caminho do fluxo.
  3. Recursos (3): Contêiners que representam valores como campos ou fórmulas. Esses valores podem vir do próprio flow ou de variáveis globais.

### Approval Process
Uma outra ferramenta de automação que permite definir:
* Regras para submeter ações em registros para aprovação (quais critérios um registro novo ou atualizado deve cumprir para ser enviado para aprovação?)
* Ações a serem submetidas para aprovação (quais alterações no registro devem ser feitas?)
* Passos para aprovação (quantas pessoas devem aprovar esse registro?)
* Ações finais após aprovação (o que será feito se o registro for aprovado?)
* Ações finais após rejeição (e se não for aprovado?)
* Ações de recall (e se foi quase aprovado, mas ainda precisa de algo?)

### Visual Flows
* 3 nomes relacionados a flow podem nos confundir, mas são coisas distintas: 
  * Visual Workflow: É um produto que engloba o processo de planejar, gerenciar e executar flows.
  * Flow Builder: Ferramenta point-and-click para criar flows
  * Flow: Aplicação que automatiza um processo de CRUD de dados no Salesforce.
Em resumo: Visual Workflow é o nome do produto cuja ferramenta é o Cloud Flow Designer, e flows são criados a partir dela.
* Ações de Visual Flows podem ser usadas no lugar do Process Builder, pois contém os mesmos recursos e um pouco mais.
* São úteis para casos onde é necessário coletar informação do usuário.
* Pode ser encontrado em: Setup > Process Automation > Flows

### Apex: Variables, Constants, Methods and Expressions
* Características da linguagem Apex:
  * Case insensitive
  * Fortemente tipada
  * Notação camel case é recomendada
* Os tipos de dados Apex são divididos em:  

  * Primitives:

    |Tipo|Exemplo|Observações|
    |-|-|-|
    |Blob|String myString = 'StringToBlob'; Blob myBlob = Blob.valueof(myString);|coleção de dados binários armazenados como um único objeto|
    |Boolean|Boolean myBool = true;|guarda true ou false|
    |Date|Date myDate = Date.newInstance(1993, 2, 19)|guarda apenas data (sem tempo). Permite operações com inteiros, retornando um Date|
    |Datetime|Datetime myDT = Datetime.newInstance(1993, 2, 19, 17, 30, 59)|guarda data e tempo. Permite operações com inteiros e double, retornando um Date.|
    |Decimal|Decimal PI = 3.1415;|32 bit (equivalente ao float). Campos de Currency são atribuídos para Decimal|
    |Double|Double n = 32.55;|64 bit|
    |ID|ID myId = valorDeUmCampoId|identificador de registro Force.com de 18 caracteres|
    |Integer|Integer n = 10;|32 bit|
    |Long|Long n = 10L;|64 bit|
    |sObject (specific)|Account acc = new Account();|objetos standard e custom|
    |sObject (generic)|sObject so = new Account(); Account a = (Account)so; // cast para specific|objetos standard e custom|
    |Object|Object obj = 10; Integer i = (Integer)obj;|representa qualquer tipo de dado do Apex (todos os dados herdam de Object)|
    |String|String name = 'Paulo'| valores devem estar entre aspas simples `'string'` somente. Use \ como caractere de escape. Suporta operadores de comparação|
    |Time|Time myTime = Time.newInstance(18, 30, 2, 20)|guarda apenas tempo. Diferente de Date e Datetime, não tem nenhum campo relacionado com esse tipo.|

    **OBS:** Cada tipo primitivo tem sua própria classe e métodos. Para mais detalhes, consulte: https://developer.salesforce.com/docs/atlas.en-us.apexcode.meta/apexcode/apex_dev_guide.htm

  * Collections: 

    |Tipo|Exemplo|Observações|
    |-|-|-|
    |List|List<type> myList = new List<type>();|armazena elementos **ordenados/indexados** e **não-únicos** (ON). Equivalente a arrays|
    |Set|Set<type> mySet = new Set<type>();|armazena elementos **não-ordenados** e **únicos** (UU)|
    |Map|Map<type,type> myMap = new Map<type,type>();|armazena pares (key,value), onde key é como um set e value é como uma list|

    **OBS:** Há várias formas de se declarar collections. Consulte o Apex Developer Guide para saber mais.

  * Enums:
  São usadas para definir conjuntos de valores cuja a ordem numérica não importa.

    **Exemplo:** 

    ```
    public enum Season {WINTER, SPRING, SUMMER, FALL} // declara enum Season
    Season current = Season.WINTER; // usa como um novo tipo de dado com valores limitados
    ```

  **OBS:** Variáveis declaradas sem valor retornam null.

* Constantes: São variáveis que só podem ser atribuídas uma vez, e são definidas com a palavra-chave **final**. Há apenas duas formas de se atribuir um valor nesse caso:
  * Na declaração: `final Double PI_NUMBER = 3.1415;` 
  * No construtor...
  <!-- * Através de um método inicializador static:
    ```
    public class myCls {
      static final Double PI_NUMBER;
      static {
        PI_NUMBER = 3.1415
      }
    }
    ``` -->

**OBS:** É uma boa prática que variáveis const sejam upper case e com notação usando _  

* Métodos são funções definidas na classe.
  * Sua sintaxe é:

    ```java
    [access modifier] [static] returnType name(params) {
      // body
    }
    ```
    * Onde:
      * access modifier - o modificador de acesso
      * static - torna o método membro da classe e não de instância
      * returnType - tipo do retorno
      * name - nome do método
      * params - parâmetros do método
  * Toda classe possui um método `construtor` especial:
    * Possui o mesmo nome da classe e se não for definido, um método construtor padrão é definido.
    * Não possui tipo de retorno.
    * É executado quando a classe é instanciada (com o operador `new`).
    * Pode receber parâmetros.

**OBS:** Modificadores de acesso para atributos e métodos são:

|Modificador|Descrição|
|:-:|:-:|
|private|o membro só pode ser acessado pela própria classe (**padrão**)|
|protected|o membro só pode ser acessado pela própria classe, por sua superclasse ou subclasses|
|public|o membro pode ser acessado dentro da mesma aplicação ou namespace|
|global|o membro pode ser acessado de qualquer aplicação ou namespace|

### Apex: Flow Control Statements
* Instruções de seleção  
No Apex temos o comum if, if-else, if else-if else, e switch:  

**Exemplo if:**
```
if(booleanExpression) {
  // run statements
}
```
**Exemplo if-else**
```
if(booleanExpression) {
  // run statements
} else {
  // run statements
}
```
**Exemplo if else-if else:**
```
if(booleanExpression) {
  // run statements
} 
else if (booleanExpression) {
  // run statements
} else {
  // run statements
}
```
**Exemplo switch comum**
```
switch on expression {
  when value1 {
    // code block 1
  }
  when value2 {
    // code block 2
  }
  when value3, value4 { // quando expression = value3 ou value 4...
    // code block 3
  }
  when valuen {
    // code block n
  }
  when else { // opcional
    // code block else
  }
}
```
**Exemplo switch com sObjects**
```
switch on sobject {
  when Account a {
    // code block 1
  }
  when Contact c {
    // code block 2
  }
}
```

* Instruções de repetição: Em Apex, temos os loops:
  * while:
```
while(booleanExpression) {
  // run statements
}
```
  * do-while:
```
do {
  // run statements
} while(booleanExpression);
```
  * for: Há 3 variações do loop for:
    * tradicional:
    ```
    for(initStmt; exitCondition; incrementStmt) {
      // run statement
    }
    ```
    * for-each:
    ```
    for(Object variable : list_or_set) {
      // run statement
    }
    ```
    * SOQL for:
    ```
    for(Type variable: [query soql]) {
      // run statement
    }
    ```

    **OBS:** O Salesforce impõe um limite de 200 registros por lote no retorno de uma instrução SOQL. Por exemplo:
    ```
    for (List<Account> listAcc : [SELECT Id, Name FROM Account] ) {
    // Your code
    }
    ```
    Supondo que essa query retorne 1000 registros, eles não serão retornados em uma lista única, mas em 5 listas de 200 registros. Então cada variável de iteração é uma lista (listAcc) com 200 registros cada. Como também existe um limite DML de 150 instruções por transação, o ideal é executá-las fora do loop. Uma estrutura completa de instruções SOQL e DML em massa seria:
    ```
    for (List<Account> listAcc : [SELECT Id, Name FROM Account] ) {
      for (Account a : listAcc  ) {
          // código sem instruções DML
      }
      // intruções DML sobre cada lista (listAcc)
    }
    ```
    **OBS:** Executar uma operação DML, seja em um sObject, ou lista de sObjects, é considerada como uma única instrução. Logo, no exemplo, seriam necessárias apenas 5 instruções, uma para cada lista.

* Instruções de pulo (disponíveis para instruções de repetição)
  * break: interrompe as próximas iterações do loop
  * continue: sai da iteração atual e vai para a próxima

### Operadores lógicos
* Os operadores lógicos em Apex são
  * &&
  * ||
  * !
* && e || usam short-circuit evaluation, o que significa que:
  * A && B resulta em false se A = false, independente de B
  * A || B resulta em true se A = true, independente de B

### Copy/Pass by Reference/Value
* Objetos (sObjects, collections, tipos definidos pelo usuário, etc.) são copiados/passados como referência.
* Tipos primitivos (Integer, String, Boolean, Date, Datetime, Decimal, etc.) são copiados/passados como valor.

Exemplo:

```java
// Pass:
public class MyClass {
    public void modifyLead(Lead myLead) {
        myLead.LastName = 'Modified';
    }

    public void modifyInteger(Integer myInt) {
        myInt = 100;
    }
}

Lead myLead = new Lead(LastName = 'Original');
new MyClass().modifyLead(myLead); // pass by reference
System.debug(myLead); // Output: Lead:{LastName=Modified}

Integer myInt = 50;
new MyClass().modifyInteger(myInt); // pass by value
System.debug(myInt); // Output: 50


// Copy:
Lead lead1 = new Lead(lastName = 'Smith');
Lead lead2 = lead1; // copy by reference
lead2.lastName = 'Baker';

System.debug(lead1.lastName); // Output: Baker

Integer x = 10;
Integer y = x; // copy by value
y += 2;

System.debug(X); // Output: 10
```

### Clonando objetos
* Como vimos na seção `Copy/Pass by Reference/Value`, objetos atribuídos com o operador `=` referenciam o objeto original. Clonar um objeto é criar um objeto independente do original.
* Existem duas formas de clonar objetos, que dependem do tipo:
  * Para sObjects: 
    * Usar o método `SObject clone(Boolean preserveId, Boolean isDeepClone, Boolean preserveReadonlyTimestamps, Boolean preserveAutonumber)`
  * Para outros tipos de objetos:
    * Podemos usar o `static String JSON.serialize(Object obj)` and `static Object JSON.deserialize(String json, System.type apexType)`

Exemplo:

```java
// Clonando sObjects
Lead originalLead = [SELECT Id, firstName FROM Lead LIMIT 1];
Lead clonedLead = originalLead.clone(true, true, true, true);

System.debug(originalLead); // Lead:{Id=00Q3N000005Xh2pUAC, FirstName=HERCULES}
System.debug(clonedLead); // Lead:{Id=00Q3N000005Xh2pUAC, FirstName=HERCULES}

clonedLead.firstName = 'ZEUS'; // não altera originalLead
System.debug(originalLead); // Lead:{Id=00Q3N000005Xh2pUAC, FirstName=HERCULES}

// Clonando outros tipos de objeto
List<String> originalList = new List<String>{
    'a', 'b', 'c'
};

List<String> clonedList = (List<String>)JSON.deserialize(JSON.serialize(originalList), List<String>.class);
clonedList[0] = 'x'; // não altera originalList

System.debug(originalList); // (a, b, c)
```

### Apex Classes and Interfaces: OOP and Access Modifiers
* Classes Apex são declaradas com a sintaxe:

|Sintaxe|Descrição|Opcional|Default|
|-|-|-|-|
|private, public, global|modificador de acesso|não (para classes top-level)|private (para classes internas|
|virtual, abstract|virtual ou abstrata|sim||
|with sharing, without sharing, inherited sharing|Sharing level|sim|without sharing|
|class ClassName|keyword class e nome|não||
|implements Interface|implementa interface?|sim||
|extends ClassName|estende uma superclasse?|sim||

* Modificadores de acesso:
  * private: não pode ser acessada por nenhuma outra classe. Só pode ser especificado em classes internas e classes de teste.
  * public: pode ser acessada dentro da mesma aplicação ou namespace
  * global: pode ser acessada de qualquer aplicação, namespace ou org
* Virtual e Abstract:
  * virtual: Pode ser usada em:
    * Classes: permite que a classe seja herdada (extends). 
    * Métodos: deve ser definido na classe base e é **opcional** de ser sobrescrito por classes herdadas (polimorfismo) com `override`.
  * abstract: Pode ser usada em:
    * Classes: permite que uma classe seja herdada (extends). Se uma classe contém pelo menos um método declarada como `abstract`, então ela deve ser abstrata. Classes abstratas não podem ser instanciadas. Subclasses de classes abstratas são obrigadas a definir os métodos `abstract`.
    * Métodos: deve ser declarado na classe base e definido na classe herdada. 
* extends: torna a classe subclasse de uma classe virtual ou abstrata, herdando todas as suas variáveis e métodos. **Apenas uma classe** pode ser herdada. 

* Interfaces:
  * São como classes, mas possuem **apenas declarações métodos** sem modificadores de acesso.
  * Usam a keyword `interface` em vez de `class`.
  * Classes que implementam interfaces são **obrigadas** a definir todos os seus métodos.
  * Uma classe pode implementar mais de uma interface.

**OBS:** Se algum membro da classe for `global`, a classe deve ser `global`

* As tabelas abaixo resumem as diferenças entre Virtual, Abstract e Interface

|`Superclasses`|Virtual|Abstract|Interface|
|:-:|:-:|:-:|:-:|
|**Keyword**|virtual|abstract|interface|
|**Métodos virtual**|0+|0+|não|
|**Métodos abstract**|não|0+|não|
|**Métodos sem implementação (e sem keywords)**|não|não|todos|
|**Permite modificadores de acesso**|sim|sim|não|
|**Pode ser instanciada**|sim|não|sim|
|**Instância pode receber instância da subclasse**|não|não|sim|

|`Subclasses`|Virtual|Abstract|Interface|
|:-:|:-:|:-:|:-:|
|**Keyword**|extends|extends|implements|
|**Quantas classes**|0-1|0-1|ilimitado|
|**Requere sobrescrever métodos**|abstract|abstract|todos|
|**Pode sobrescrever métodos**|virtual|virtual|todos|

|`Métodos`|virtual|abstract|interface|
|:-:|:-:|:-:|:-:|
|**Keyword na superclasse**|virtual|abstract|-|
|**Keyword na subclasse**|override|-|-|

* **Exemplos:**

  * Virtual

    ```java
    // Superclasse
    public virtual class MyVirtualClass {
      public virtual void virtualMethod() { System.debug('base method!'); }
    }
    // Subclasse
    public class MySubClass extends MyVirtualClass {
      // não é obrigatório sobrescrever o método virtual
      override public void virtualMethod() { System.debug('subclass method!'); }
    }
    // Uso
    MyVirtualClass mvc = new MyVirtualClass();
    mvc.virtualMethod(); // exibe: base method!
    MySubClass msc = new MySubClass();
    msc.virtualMethod(); // exibe: subclass method!
    ```

  * Abstract
  
    ```java
    // Superclasse
    public abstract class MyAbstractClass {
      public virtual void virtualMethod() { System.debug('base method!'); };
      public abstract void abstractMethod();
    }
    // Subclasse
    public class MySubClass extends MyAbstractClass {
      // não é obrigatório sobrescrever o método virtual, mas o método abstract sim
      override public void abstractMethod() { System.debug('subclass method!'); }
    }
    // Uso
    MySubClass msc = new MySubClass();
    msc.virtualMethod(); // exibe: base method!
    msc.abstractMethod(); // exibe: subclass method!
    ```

  * Interface

  ```java
    // Interface
    public interface MyInterfaceClass {
      void interfaceMethod();
    }
    // Classes concretas
    public class MyConcreteClass1 implements MyInterfaceClass {
      // É obrigatório implementar todos os métodos da interface
      public void interfaceMethod() { System.debug('concrete class 1 method!'); }
    }
    public class MyConcreteClass2 implements MyInterfaceClass {
      // É obrigatório implementar todos os métodos da interface
      public void interfaceMethod() { System.debug('concrete class 2 method!'); }
    }
    // Uso
    // OBS: A inserção numa lista é apenas para demonstrar que uma interface pode ser instanciada e receber objetos que a implementem
    List<MyInterfaceClass> micList = new List<MyInterfaceClass>();
    micList.add(new MyConcreteClass1());
    micList.add(new MyConcreteClass2());
    // exibe: concrete class 1 method! concrete class 2 method!
    for (MyInterfaceClass mic : micList) { mic.interfaceMethod(); }
  ```

* Keyword `super`:
  * Palavra-chave usada em métodos construtores e `@override` de subclasses (herdando de classes abstract e virtual) para referenciar métodos da superclasse extendida.
  * A sintaxe é:
    * Num construtor: `super(params)`, onde `params` são os parâmetros de um método construtor da superclasse. Importante: A instrução `super(params)` deve ser a primeira linha do método construtor da subclasse.
    * Num método `@override`: `super.methodName(params)`, onde `methodName(params)` é um método da superclasse.
  
  * **Exemplo:**

    ```java
    //superclasse
    public abstract class MyAbstractClass {
      public MyAbstractClass() {
          System.debug('MyAbstractClass constructor!');
      }
      public virtual void virtualMethod() { System.debug('base method!'); }
      public abstract void abstractMethod();
    }
    //subclasse
    public class MySubClass extends MyAbstractClass {
      public MySubClass() {
          super();
      }
      override public void abstractMethod() { 
        super.virtualMethod(); 
      }
    }
    //uso:
    MySubClass msc = new MySubClass(); // exibe: MyAbstractClass constructor!
    msc.abstractMethod(); // exibe: base method!
    ```

**OBS:** Classes Apex podem conter inner classes, que são instanciadas assim:
`myClass.myInnerClass myInnerClassObject = new myClass.myInnerClass();`

### SOQL
#### Introdução
* Salesforce Object Query Language (SOQL) é como SQL. Sintaxe básica:
```[SELECT fields FROM Object WHERE filter]```
* Não é possível usar * para selecionar todos os campos pois é um governor limit.
* SOQL é case insensitive
* Pode ser chamado em qualquer lugar que use código Apex

#### WHERE
* Filtros de expressões da cláusula WHERE incluem (tanto para números quanto strings):
  * Operadores de comparação: `=` , `!=` , `<` , `<=` , `>` , `>=`
    * **Exemplo 1:** `SELECT Name FROM Account WHERE Name = 'My Account'`
    * **Exemplo 2:** `SELECT Name,Type FROM Account WHERE Name = 'My Account'`
  * Outros: `LIKE` , `IN` , `NOT IN`
    * LIKE é usado com wildcards `%` ou `_`
      * `%` corresponde a vários caracteres
      * `_` corresponde a um caractere
      * Opera apenas com strings e é case-insensitive.
      * **Exemplo:** `SELECT Name FROM Account WHERE Name LIKE '_y%'` 
    * IN é usado como o operador `=` para múltiplas comparações
      * **Exemplo:** SELECT Name FROM Account WHERE Name IN('My Account', 'Other Account')
    * NOT IN é como o `!=` para múltiplas comparações
* É possível buscar por campos nulos ou não com `= null` ou `!= null` 
* Valores booleanos são comparados com `= TRUE` ou `= FALSE`
* Operadores condicionais podem ser usados com tipos Date, Datetime e Date Literal e Date Function
  * **Exemplo:** 
  
  |Date Type|Format|Example|
  |-|-|-|
  |Date|YYYY-MM-DD|SELECT Id FROM Opportunity WHERE closeDate >= 2017-09-01|
  |Datetime|* YYYY-MM-DD-Thh:mm:ss+hh::mm <br> * YYYY-MM-DD-Thh:mm:ss-hh::mm <br> * YYYY-MM-DD-Thh:mm:ss-hh::mm:ssZ <br>|SELECT Id FROM Opportunity WHERE closeDate >= 2017-09-01T:00:00:00Z|
  |Date Literal|* TODAY <br> * LAST_MONTH <br> * NEXT_YEAR <br> * Etc...|SELECT Id FROM Opportunity WHERE closeDate = THIS_QUARTER|
  |Date Function|* CALENDAR_MONTH() <br> * CALENDAR_YEAR() <br> * DAY_IN_MONTH() <br> * Etc...|SELECT Id FROM Opportunity WHERE DAY_IN_YEAR(closeDate) > 90|

* Operadores lógicos incluem `AND`, `OR` e `NOT`
  * **Exemplo:** SELECT Name FROM Account WHERE (Name = 'My Account' AND ID = 12345678)
* Para pular os caracteres especiais, usamos `\`
* Podemos usar SOQL no Data Loader para não precisar usar a interface.
* Enquanto em Workflow Rules e Process Builder só conseguimos acessar os registros base e relacionados, o SOQL permite acessar **qualquer** registro no Salesforce

#### Expressões após WHERE
* LIMIT n: define limite de n linhas retornadas pela query
  * **Exemplo:** SELECT Name FROM Account LIMIT 1 
* OFFSET n: define que as primeiras n linhas devem ser ignoradas no retorno da query.
  *  **Exemplo:** SELECT Name FROM Account OFFSET 10
* ORDER BY field1 [, fieldn...]: define um ou mais campos a serem ordenados no retorno da query
* ASC | DESC: define ordem ascendente (padrão) ou descendente
  * **Exemplo:** SELECT Name FROM Account ORDER BY Type DESC; 
* NULLS FIRST | LAST: define se nulls são exibidos primeiro ou por último
  * **Exemplo:**  SELECT Name FROM Account NULLS FIRST
* SELECT field, fieldn GROUP BY field, fieldn: retorna os valores distintos dos campos field, como uma estrutura de dados SET que contem os valores únicos para um ou mais campos juntos.
  * **Exemplo:** SELECT Name FROM Account GROUP BY Name

#### Aggregate functions
* Aggregate functions são funções que retornam resultados agregados:
  * COUNT()
  * COUNT(field)
  * AVG(field)
  * SUM(field)
  * MIN(field)
  * MAX(field)
  * COUNT_DISTINCT()
  * COUNT_DISTINCT(field)
* **Exemplo:** SELECT AVG(Amount) FROM Opportunity
* COUNT(field) e COUNT_DISTINCT(field) retornam um número de registros que corresponde a query, mas, diferente de suas versões sem parâmetro, retornam apenas registros com `field` não nulo.  
* **OBS:** Ao usar GROUP BY **field**, os campos no SELECT devem ter somente **field** ou funções agregadas  
* **OBS:** Se COUNT() (sem parâmetros) for usado, deve ser o único no SELECT

#### Pseudônimo
* Podemos definir pseudônimos para aggregate functions e objetos após a declaração destes, e depois referenciá-los na própria query:
* **Exemplo:** 

  ```SQL
  SELECT count() myCount
  FROM Contact c, c.Account a
  WHERE a.name = 'Edge Communications'
  ```

#### Retorno de SOQL queries
* Queries podem retornar:
  * List\<sObject>: `List<Account> myAccs = [SELECT Id, Name FROM Account];`
  * sObject: `Account myAccs = [SELECT Id, Name FROM Account LIMIT 1];`
  * List\<AggregateResult>: É o retorno de queries com aggregate functions (exceto COUNT()) e/ou GROUP BY: `List<AggregateResult> = [SELECT AVG(Amount) avg FROM Opportunity WHERE Account.Name = 'Edge Communications'];`
  * Integer: `Integer acc = [SELECT COUNT() FROM Account];`

* Podemos chamar variáveis nas queries com o uso de `:variable`. **Exemplo:**
```
Integer myInt = 1000;
Integer myList = [SELECT count() FROM Opportunity WHERE Amount > :myInt];
```

##### Mais sobre aggregate functions
* Cada aggregate function definida numa query é mapeada para um campo no objeto `AggregateResult` retornado, que por padrão é nomeada como `exprN`, onde `N` é a ordem em que a função foi declarada na query, começando por 0. Usar pseudônimos pode melhorar a leitura desses campos.
* Podemos acessar propriedades de um objeto `AggregateResult` como um map, usando `get('expressionName')`, onde `expressionName` é o nome do campo.

**Exemplo:**

```SQL
List<AggregateResult> agg = [
  SELECT AVG(Amount) avg, Count(name)
  FROM Opportunity
  WHERE Account.Name LIKE 'E%'
];
System.debug(agg[0].get('expr0')); // 'expr0' se refere a coluna Count(name) 
System.debug(agg[0].get('avg'));
```

#### Acessando objetos relacionados via SOQL
* Em SOQL queries, podemos classificar o acesso à objetos relacionados em 2 tipos:
  * Parent-to-child: 
    * Quando a query envolve acessar registros filhos do objeto principal da query
    * Isto é feito ao criar uma query interna no `SELECT` da query principal.
    * Usa-se o `Child Relationship Name` para referenciar o objeto filho. Se o filho for custom, deve-ser usar o sufixo `__r`.
    * Para cada registro do pai, uma List de filhos é retornada
    * O nível máximo de relações é 1
  * Child-to-parent:
    * Quando a query envolve acessar algum campo do objeto pai:
    * O campo pode ser o Id do pai, ou um campo de referência:
      * Para acessar o Id do objeto standard: nome do objeto + id
      * Para acessar o Id do objeto custom: nome do objeto custom
      * Para acessar um campo de referência do objeto standard: objeto.campo
      * Para acessar um campo de referência do objeto custom: objeto__r.campo
      * O nível máximo de relações é 5

  * Exemplo Parent-to-child:

    ```SQL
    // Standard Object
    List<Account> accounts = [
      SELECT ID,
      Name,
      (SELECT ID FROM Contacts)
      FROM Account
    ];

    // Custom Object
    List<Parent__c> parents = [
      SELECT ID,
      Name,
      (SELECT ID FROM Children__r)
      FROM Parent__c
    ];
    ```

* Exemplo Child-to-parent:

  ```SQL
  // Standard Object
  List<Contact> contacts = [
    SELECT ID,
    AccountId, // acessa o id diretamente
    Account.Id,
    Account.Name
    FROM Contact
  ];

  // Custom Object
  List<Child__c> children = [
    SELECT ID, 
    Parent__c, // acessa o id diretamente
    Parent__r.Name
    FROM Child__c
  ];
  ```
* Tabela de resumo de relacionamentos em SOQL:

|`Relationship by Object Type`|Parent|Child|Standard|Custom|Exemplo Standard|Exemplo Custom|
|-|:-:|:-:|:-:|:-:|:-:|:-:|
|**Parent-to-child**|-|Object|Objects|Objects__r|Contacts|Children__r|
|**Child-to-parent Id**|Object|-|ObjectId|Object__c|AccountId|Parent__c|
|**Child-to-parent Reference**|Object|-|Object|Object__r|Account|Parent__r|

#### Semi-joins e Anti-joins
Semi-joins e Anti-joins são filtros que usam campos de objetos filhos para filtrar registros do pai. Isto é possível usando `IN` (semi-join) e `NOT IN`(anti-join).

* **Exemplo Semi-join**:

  ```SQL
  // Retorna todos os Accounts que contém pelo menos uma oportunidade.
  SELECT Id FROM Account
  WHERE Id IN
    (SELECT AccountId
    FROM Opportunity)
  ```

* **Exemplo Anti-join**:

  ```SQL
  // Retorna todos os Accounts que não contém nenhuma oportunidade.
  SELECT Id FROM Account
  WHERE Id NOT IN
    (SELECT AccountId
    FROM Opportunity)
  ```

* Para entender visualmente, veja esta ilustração:
![[semi-joins-and-anti-joins.png]]

#### SOQL Dinâmico
* Podemos criar queries dinâmicas com o uso do método `Database.query(qryString)`, onde qryString é uma string representando a query (sem os `[]`). Isso nos permite queries flexíveis.
* **Exemplo:**

```java
String fields = 'Id, Name';
Database.query('SELECT ' + fields + ' FROM Account');
```

* Podemos fazer o bind de Strings (somente Strings) na query, como no SOQL estático:
  
```java
String name = 'Paul';
Database.query('SELECT Id, Name FROM Account WHERE Name = :name');
```

* Variáveis bind na qryString devem ser estar declaradas no mesmo escopo onde `Database.query` é executado.  
Para contornar essa limitação, podemos usar o método `Database.queryWithBinds(qryString, bindVariablesMap, accessLevel)`, onde:
  * bindVariablesMap: É um Map<String, Object> onde as chaves são as variáveis bind, e os valores são os valores das variáveis
  * accessLevel: Pode ser `AccessLevel.SYSTEM_MODE` ou `AccessLevel.USER_MODE`, definindo se o método é executado com acesso de sistema e usuário, respectivamente

* **Exemplo:**

```java
Map<String, Object> binds = new Map<String, Object> {
  'firstName' => 'Paulo',
  'lastName' => 'Silva'
}
Database.queryWithBinds('SELECT Id FROM Lead WHERE FirstName = :firstName AND LastName = :lastName', binds, AccessLevel.USER_MODE);
```

### SOSL
#### Introdução
* Acrônimo para `S`alesforce `O`bject `S`earch `L`anguage.
* Sintaxe:  
  FIND *string*  
  [IN *searchGroup* FIELDS]  
  [RETURNING *object1*[(*field1, fieldN* [WHERE *condition*] [LIMIT N])] [, *objectN*...]

  Onde:
  * *string* é um valor do tipo Text, Phone ou Email.  E deve ser envolta em aspas simples ('') quando usada no Apex, ou chaves ({}) no developer console ou workbench.
  * `searchGroup` é um ou mais valores da lista, separados por vírgula:
    * ALL FIELDS
    * NAME FIELDS
    * EMAIL FIELDS
    * PHONE FIELDS
    * SIDEBAR FIELDS
  * O retorno da query é um `List<List<sObject>>` e deve-se fazer um cast para um sObject concreto para acessar seus registros.
  * Se `RETURNING object1` for declarado sem parâmetros, então os registros retornados terão apenas Id.
  * Wildcards podem ser usados na `string`, onde `*` representa 0 ou mais caracteres e `?` representa um caractere.

* **Exemplo**

  ```java
  List<List<sObject>> results = [
  FIND 'John?' OR '11*'
  IN Name, Phone FIELDS
  RETURNING Account(Id, Name), Contact(Id, Name)
  ];

  List<Account> myAcc = (List<Account>)results[0];
  System.debug(myAcc[0].Name);
  ```

  * Neste exemplo:
    * A query buscará por nomes como Johny ou Johns ou por um número que comece com 11 nos campos Name e Phone nos objetos Account e Contact, e retornando Id e Name dos registros encontrados tanto em Account quanto Contact.
    * Um cast para List<Account> é feito em results[0](baseado na ordem de objetos de `RETURNING`, Account é o índice 0).
    * Um print no console é feito para o Name do primeiro registro encontrado (myAcc[0].Name).

#### Diferenças de SOQL e SOSL
|Tópico|SOQL|SOSL|
|-|-|-|
|Performance|Menor|Maior|
|Requerido especificar objeto|Sim|Não|
|Dados retornados|De um único objeto ou relacionados|De múltiplos objetos|
|Pode contar registros retornados|Sim|Não|
|Pode ser usado em triggers|Sim|Não|
|Tipos de dado buscados|Qualquer|Apenas Text, Phone ou Email|
|Pode executar DML no retorno|Sim|Não|
|Tipos retornados|List\<sObject>, sObject, Integer|List<List\<sObject>>|
|Wildcards|% e _|* e ?|

### DML
#### Introdução
* DML (`D`ata `M`anipulation `L`anguage) são instruções que manipulam registros, diferentemente de SOQL e SOSL, que consultam os registros.
* Assim como numa GUI, as operações seguem regras como validation rules e campos obrigatórios.
* Por padrão, as operações
* As operações possíveis são:

|Operação|Descrição|
|-|-|
|insert|insere registros|
|update|atualiza registros|
|upsert|atualiza se o registro já existe ou insere se não existir|
|delete|deleta registros|
|undelete|restaura o registro da lixeira|
|merge|mescla até 3 registros do mesmo objeto em um dos registros e deleta os registros restantes, reparentando registros relacionados|

* Há 2 formas de executar instruções DML. Ambas aceitam um ou múltiplos registros:
  * Usando instruções DML implícitas: 
    * Sintaxe: *operation* record | records
    * Exemplo 1: `insert new Account(name='Acc');` 
    * Exemplo 2: `merge record1 record2 record3;` 
  * Usando métodos da classe Database:
    * Sintaxe: Database.*operation*(record | records[, *params*]), onde:
      * *params* são parâmetros opcionais para diferentes sobrecargas do método Database.*operation*. Um exemplo é o parâmetro *allOrNone*, que define se a operação é parcial ou não para uma lista de registros.
    * Exemplo: `Database.insert(accounts, false)`

* Operações DML implícitas são por padrão allOrNone = true.

#### Mais sobre a classe Database
* A classe Database tem algumas vantagens sobre sua versão independente, por exemplo:
  * Permite operações parciais, ou seja, se um registro falhar, os outros ainda poderão ser salvos (com o parâmetro `allOrNone` = false).
  * O método upsert aceita o parâmetro externalIDField que serve para definir um campo como Id externo para determinar se um registro deve ser atualizado ou inserido, enquanto o upsert independente só consegue usar o próprio Id do registro pra isso.
  * Retorna um objeto ou lista de Database.*opResult* resultado da operação, que nos permite tratar erros:
  
  |Método|Retorno com 1 registro|Retorno com lista de registros|
  |-|-|-|
  |Database.insert()|Database.saveResult|List<Database.saveResult>|
  |Database.update()|Database.saveResult|List<Database.saveResult>|
  |Database.upsert()|Database.upsertResult|List<Database.upsertResult>|
  |Database.delete()|Database.deleteResult|List<Database.deleteResult>|
  |Database.undelete()|Database.undeleteResult|List<Database.undeleteResult>|
  |Database.merge()|Database.mergeResult|List<Database.mergeResult>|

* O Database.*opResult* tem 3 métodos:
  * getId() - retorna o Id do registro manipulado.
  * getErrors() - retorna uma List<Database.Error>
  * isSuccess() - retorna o resultado da operação (true ou false)
* O Database.Error tem os seguintes métodos:
  * getStatusCode() - retorna o código de status do erro
  * getMessage() - retorna a mensagem de erro
  * getFields() - retorna uma List<String> com os erros, se houverem, que impactaram no erro.

* **Exemplo:**

```java
List<Account> accsToAdd = new List<Account>();
for(Integer i = 0; i < 10; i++) {
  if (i == 9) {
    accsToAdd.add(new Account());
  } else {
    accsToAdd.add(new Account(name='Test'+i));
  }
}

List<Database.SaveResult> results = Database.insert(accsToAdd, false);

for(Database.SaveResult sr : results) {
  if (sr.isSuccess()) {
    System.debug('Account saved successfully. Id: ' + sr.getId());
  } else {
      for(Database.Error err : sr.getErrors()) {
        System.debug('An error ocurred ' + err.getStatusCode() + ' - ' + err.getMessage());
        System.debug('Account fields that affect this error: ' + err.getFields());
    }
  }
}
```

* Ao executar o código acima, o resultado deve ser este:

![[database.saveResult-log.png]]

### Savepoint e Rollback
* Podemos controlar a persistência dos registros no banco de dados durante uma transação com o uso de um `savepoint`.
* Um savepoint é um objeto retornado pelo método `Database.savepoint()`;
* A partir da execução de Database.savepoint(), todas as operações DML podem ser revertidas na execução do método `Database.rollback(sp)`

Exemplo:

```javascript
Account acc = new Account();
Savepoint sp = Database.setSavepoint();
insert acc;
Database.rollback(sp); // a inserção de acc foi revertida
```

### Apex Triggers
#### Introdução
* Triggers são blocos de código executados a partir de eventos de DML em registros, como insert, update, delete, etc..
* Podem ser criadas no setup do próprio objeto, Developer Console e VSCode.
*  São ativas por padrão (campo Status = 'Active' no registro de ApexTrigger), mas podem ser desativadas em Setup > Custom Code > Apex Triggers > Edit > defina is active como falso;
* Sintaxe:  
    trigger *triggerName* on *sObjectName*   (*triggerEvents*) {  
      //trigger code  
    }  

* Onde:
  * *triggerName* é o nome da trigger
  * sObjectName é qualquer sObject, como Account ou um objeto custom.
  * *triggerEvents* é uma lista de um ou mais tipos de evento, separados por vírgula, que são:
    * before insert
    * before update
    * before delete
    * after insert
    * after update
    * after delete
    * after undelete

* As diferenças entre before e after triggers são:

|Tópico|Before|After|
|-|-|-|
|Acionados|Antes do registro ser salvo na base|Depois do registro ser salvo na base|
|Acesso à campos gerados pelo sistema (Id, createdDate, etc.)|Não|Sim|
|DML explícito necessário|Não|Sim|
|Uso comum|Atualizar e validar registros antes de salvá-los na base|Criar relacionamentos com registros novos ou existentes a partir dos campos de sistema.|

#### Trigger Context Variables
* São variáveis que referenciam valores para diferentes contextos DML:

  |Variável|Valor|
  |-|-|
  |Trigger.new|Lista com as versões **novas** dos registros|
  |Trigger.newMap|Map de Ids para as versões **novas** dos registros|
  |Trigger.old|Lista com as versões **antigas** dos registros|
  |Trigger.oldMap|Map de Ids para as versões **antigas** dos registros|
  |Trigger.size|Total de registros na invocação da trigger|
  |isExecuting|true se o contexto atual de execução for Apex e false se for outro (interfaces, web service, etc.)|
  |isInsert|true se a trigger foi invocada por operação de insert|
  |isUpdate|true se a trigger foi invocada por operação de update|
  |isDelete|true se a trigger foi invocada por operação de delete|
  |isUndelete|true se a trigger foi invocada por operação de undelete|
  |isBefore|true se a trigger foi invocada **antes** de qualquer registro ser salvo|
  |isAfter|true se a trigger foi invocada **depois** de qualquer registro ser salvo|
  |Trigger.operationType|Retorna um ENUM do tipo `System.TriggerOperation` correspondente a operação atual (são úteis com switches): <br> * BEFORE_INSERT <br> * BEFORE_UPDATE <br> * BEFORE_DELETE <br> * AFTER_INSERT <br> * AFTER_UPDATE <br> * AFTER_DELETE <br> * AFTER_UNDELETE <br>|

* Disponibilidade de variável por contexto:

  ||Trigger.new|Trigger.newMap|Trigger.old|Trigger.oldMap|
  |-|:-:|:-:|:-:|:-:|
  |**Before Insert**|Sim(w)|Null|Null|Null|
  |**After Insert**|Sim|Sim|Null|Null|
  |**Before Update**|Sim(w)|Sim(w)|Sim|Sim|
  |**After Update**|Sim|Sim|Sim|Sim|
  |**Before Delete**|Null|Null|Sim|Sim|
  |**After Delete**|Null|Null|Sim|Sim|
  |**After Undelete**|Sim|Sim|Null|Null|

Legenda: (w) = Write-able

#### Método addError()
* Podemos impedir que registros sejam salvos na base ao executar a instrução *record*.addError(*errorMessage*), onde *record* é um registro, e *errorMessage* é uma string da mensagem de erro.

* **Exemplo:**

```java
trigger AccountDeletion on Account (before delete) {
  List<Account> accWithOpp = [
    SELECT Id, Name
    FROM Account
    WHERE Id IN (SELECT AccountId 
                  FROM Opportunity
                )
    AND Id IN :trigger.old
  ];

  for (Account myAcc : accWithOpp) {
    myAcc.addError('Cannot delete account with related opportunities!');
  }
}
```

**OBS:** Triggers devem ser usados caso as ferramentas de programação declarativa não atendam às necessidades.

### Melhores práticas com Apex triggers
* Dos and Don'ts:
  * Dos:
    * Crie triggers sem lógica. Escreva a lógica em classes **TriggerHandler**. A convenção é que essas tenham o nome composto assim: *sObject*TriggerHandler.
    * Crie apenas uma trigger por objeto (se múltiplas triggers existirem para o mesmo objeto, não há controle de qual executará primeiro).
    * Separe a lógica da classe triggerHandler em métodos de acordo com o contexto.
    * Fique atento a triggers em cascata
  * Don'ts:
    * Não assuma que apenas 1 registro iniciará a trigger (até 200 registros iniciam a trigger por vez).
    * Não execute SOQL e instruções DML dentro de um for loop.

* **Exemplo:**

  ```java
  // trigger
  Trigger AccountTrigger on Account(before insert, after insert) {
    if (Trigger.isBefore && Trigger.isInsert) {
      AccountTriggerHandler.handleBeforeInsert(Trigger.new);
    }
    else if (Trigger.isAfter && Trigger.isInsert) {
      AccountTriggerHandler.handleAfterInsert(Trigger.new);
    }
  }
  // trigger handler
  public class AccountTriggerHandler {
    public static void handleBeforeInsert(List<Account> accList) {
      for (Account acc : accList) {
        acc.Description = 'New Description'; // DML não é necessário
      }
    }
    public static void handleAfterInsert(List<Account> accList) {
      List<Task> myTasks = new List<Task>();
      for (Account acc : accList) {
        myTasks.add(new Task(
          ownerId = acc.ownerId,
          subject = 'New Account Task',
          whatId = acc.Id,
          priority = 'Normal',
        ));
      }
      insert myTasks; // DML depois do for
    }
  }
  ```

### Limites de Governança
* Por ser um ambiente multitenant, o Salesforce impõe limites em cada ORG, e ao atingir um limite, um erro é emitido: `System.LimitException: limitMessage`, onde limitMessage é a mensagem de erro.
* Como existem muitos limites, a lista pode ser vista aqui: https://developer.salesforce.com/docs/atlas.en-us.236.0.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_apexgov.htm
* Os principais limites são (por transação):

|Descrição|Limite Síncrono|Limite Assíncrono|
|-|-|-|
|Queries SOQL|100|200| 
|Registros retornados por queries SOQL|50000|50000| 
|Instruções DML|150|150|
|Registros processados por operações DML|10000|10000| 
|Callouts ou chamadas a web services|100|100| 
|Chamadas ao método SendEmail|10|10|

### Ordem de execução
* Quando salvamos um registro com um `insert`, `update` ou `upsert`, o Salesforce executa os eventos abaixo na seguinte ordem:
1. Inicia o registro original da base
2. Executa validações de sistema
3. Executa flows do tipo before save
4. Executa todas as before triggers
5. Executa validações de sistema (novamente) e de usuário
6. Executa duplicate rules
7. Salva o registro no banco de dados, mas não comita.
8. Executa todas as after triggers
9. Execute assignment rules
10. Executa auto-response rules
11. Executa workflow rules
12. Executa escalation rules
13. Executa flow automations 
14. Executa flows do tipo after save
15. Execute entitlement rules
16. Executa atualizações no Rollup Summary Field no pai e pai do pai
17. Executa criteria based sharing evaluation
18. Comita todas as operações DML na base
19. Executa lógica pós commit

* Há passos em que é possível atualizar o próprio registro ou outros registros. E quando isso acontece, estes registros podem iniciar uma nova ordem de execução completa (after trigger por exemplo), ou parcial (workflow rules).
* Em todo caso, nenhum registro executa o commit e pós commit sozinho. Todos os registros esperam para executar esses passos quando o registro que iniciou a operação DML primeiro "chegar" nesses últimos passos, e aí todos são salvos juntos.
* Abaixo, podemos ver um resumo gráfico da ordem de execução, seguido de um link para a referência completa

![[execution-order.png]]

https://developer.salesforce.com/docs/atlas.en-us.apexcode.meta/apexcode/apex_triggers_order_of_execution.htm

### Lidando com exceptions
* Exceptions são erros lançados em tempo de execução (não confundir com erros de compilação, que são erros sintáticos).
* Exceptions caem em 3 categorias: 
  * Handled
    * Tratadas no código com a instrução `try-catch-finally`
    * Não para a execução imediatamente (códigos após o bloco try-catch-finally ainda serão executados)
    * Operações DML antes da exception (na mesma transação) são comitadas
  * Unhandled
    * Unhandled - não tratadas
    * Param a execução imediatamente
    * Operações DML antes da exception (na mesma transação) sofrem rollback em vez de serem comitadas
  * Limit Exceptions
    * São exceptions do tipo `LimitException`, e não podem ser pegas
    * Erros desse tipo param a execução do código imediatamente

* Sintaxe da instrução `try-catch-finally`:

  ```java
    try {
      // code block that may cause error
    } catch(exceptionType e) {
      // catch code
    } finally {
      // will be executed anyway
    }
  ```
Onde `exceptionType` é um tipo de erro:

|Erro|Descrição|Exemplo|
|-|-|-|
|DmlException|Pega erros de DML|Inserir registro sem campos obrigatórios|
|ListException|Pega erros de tipos List|Tentar acessar índice não existente numa lista|
|NullPointerException|Pega erros de acesso a nulo|Tentar acessar variável nula|
|QueryException|Pega erros envolvendo queries|Tentar atribuir uma variável do tipo sObject ao retorno de uma query que traz uma List<sObject>|
|Exception|Pega quaisquer erros|Qualquer erro genérico|

* Um bloco try pode ter vários blocos catch e finally, mas deve ter pelo menos um catch ou finally.
* Enquanto o tipo `Exception` pega qualquer erro, é uma boa prática tratar o erro com os tipos específicos esperados primeiro, e, caso os erros específicos não ocorram, tratá-lo como o tipo genérico. Caso um erro específico ocorra, o bloco do erro genérico não é executado.
  
* Os métodos da classe `Exception` são:

|Método|Descrição|
|-|-|
|getCause|Retorna a causa do erro como um objeto exception|
|getLineNumber|Retorna a linha a qual o erro foi lançado|
|getMessage|Retorna uma string da mensagem de erro|
|getStackTraceString|Retorna o stack trace como string|
|getTypeName|Retorna o tipo de erro|
|initCause|Define o motivo do erro|
|setMessage|Define a mensagem de erro que é exibida ao usuário|

* Exemplo: 

```java
try {
  Account acc = new Account();
  fillAccData(acc); // supondo que este método preencha campos de acc...
  insert acc; // esta instrução pode ou não causar um DmlException
} catch(DmlException e) { // tipo específico do erro mais provável
  System.debug('A '+ e.getTypeName() +' ocurred at line ' + e.getLineNumber()+ ' : ' + e.getMessage());
} catch(Exception e) { // tipo genérico
    System.debug('A '+ e.getTypeName() +' ocurred at line ' + e.getLineNumber()+ ' : ' + e.getMessage());
}
System.debug('After try-catch-block'); // sempre executa pois o erro foi tratado
```

#### Throw exceptions e Custom Exception Class
* Exceptions de sistema (as que vimos até agora) são lançadas automaticamente. Podemos apenas pegá-las com `catch` e lançá-las novamente com `throw e`, onde `e` é a exception parâmetro do `catch`.

* Exemplo:

```java
try {
  riskyMethod();
} catch (Exception e) {
  throw e;
}
```

* Para lançar exceptions manualmente, devemos criar uma **Custom Exception Class**. Essa classe deve herdar da classe `Exception` e deve ter o sufixo Exception em seu nome.
* A sintaxe então é:

```java
public class CustomException extends Exception {}
```

* Note que não há necessidade de nenhum código no corpo da classe, já que ela herda de exception, então terá todos os seus métodos disponíveis.
* Para usar uma custom exception class, basta usar `throw new CustomException([arguments])`, onde `arguments` são argumentos opcionais para executar sobrecargas diversas do construtor:

|Argumentos|Código|
|-|-|
|Sem argumentos|new CustomException()|
|String da mensagem de erro|new CustomException('A custom exception has ocurred')|
|Objeto exception|new CustomException(e)|
|String da mensagem de erro com Objeto exception|new CustomException('A custom exception has ocurred', e)|

* Exemplo:

```java
public class MyException extends Exception {}

if (statement) {}
else {
  throw new MyException('This is my custom exception error message');
}
```

* Ao usar o `throw`, nós "repassamos" o erro para o código cliente tratá-lo. Isso é útil quando o erro pode ocorrer numa classe com funções mais abstratas, que são usadas por diversos clientes e cada cliente deve tratar o erro à sua maneira.

### Segurança em Apex
#### Segurança de registros
* Em Apex, códigos podem ser executados em 2 modos:
  * System mode
    * Permite acesso a todos os registros do banco de dados
    * Ignora o sharing model (without sharing)
  * User mode
    * Permite acesso somente aos registros que o usuário executando o código tem acesso.
    * Respeita o sharing model (with sharing)

* Os contextos de código e seus modos de execução são:

|Contexto|System mode|User Mode|
|-|:-:|:-:|
|Triggers|✔️||
|Custom Web Services|✔️||
|Classes de teste|✔️||
|Visualforce Controllers|Custom Controller|Standard Controller|
|Visualforce Controller Extensions|se extendido por Custom Controller|se extendido por Standard Controller|
|Anonymous block||✔️|
|Custom Apex Class|Se definida com `without sharing`|Se definida com `with sharing`|

* Na definição de classes, podemos especificar o sharing level: `accessModifier [with sharing | without sharing | inherited sharing] class ClassName`
  * Por padrão, o sharing level definido é without sharing.
  * Classes herdam o sharing level por herança ou implementação.
  * Classes internas não herdam o sharing level de sua classe container.
  * Classes com with sharing podem chamar classes com without sharing.
  * Classes sem sharing level definido, quando chamadas por classes with sharing são executadas com with sharing.
  * Inherited sharing indica que o sharing level aplicado será o mesmo que a classe que chamou esta. Se este não for explícito (se a classe não definir um sharing level ou a chamada vier de um Aura/VF controller ou API Rest por exemplo), então será with sharing.

#### Segurança de classes
* Métodos de classes top-level (que não são classes internas) só podem ser executados por usuários com acesso à classe através do profile ou permission sets.
* Para alterar o acesso pelo profile: Setup > Custom Code > Apex Classes > Selecione a classe desejada > Security > mova os perfis entre as listas `Available Profiles` e `Enabled Profiles` > Save
* Para alterar o acesso pelo permission set: Setup > Users > Permission Sets > Apex Class Access > Edit > Selecione as classes desejadas > Save

### Impacto do Apex em mudanças declarativas
* Se um código Apex tem uma referência a um campo por exemplo, e houver uma tentativa de alterar o API Name do campo na interface, um erro será exibido em tela, informando que o campo é referenciado em uma classe Apex ou trigger.

### Técnicas programáticas para prevenir vulnerabilidades de segurança

|Vulnerabilidade|Descrição|Como prevenir|
|-|-|-|
|Cross-Site Scripting (XSS)|Ocorre quando um input fornecido pelo usuário é refletido no HTML de uma página web.|Use filtro de input e codificação de output|
|SOQL Injections|Receber input fornecido pelo usuário que é utilizado em SOQL dinâmico|Evitar o uso de SOQL dinâmico e priorizar SOQL estático com variáveis de bind e usar o método String.escapeSingleQuotes(str)|
|Cross-Site Request Forgery|Quando o browser do usuário executa uma ação não intencionada em um site confiável no qual o usuário está logado atualmente|Evite executar operações no carregamento da página|

### Usando ferramentas declarativas e Apex juntos
* É possível integrar as ferramentas declarativas com Apex da seguinte forma:

  |Pode executar (->)|Apex|Flow|Process|
  |-|:-:|:-:|:-:|
  |**Apex**|-|✔️|❌|
  |**Flow**|✔️|-|-|
  |**Process**|✔️|✔️|-|

#### Executando Apex a partir de um Flow e Process
* Sobre o método Apex, deve usar a seguinte sintaxe:

  ```
  public class className {
    @InvocableMethod[(label='myLabel' description='myDescription' category='myCategory')]
    global | public static return methodName(param)
  }
  ```
  Onde:
  * `className` deve ser uma classe externa
  * `modifiers` são propriedades opcionais onde:
    * `label` e `description` e `category` definem o rótulo, descrição e categoria do método para o Flow ou Process. O padrão é respectivamente o nome do método, null e Uncategorized.
  * `param` deve ser do tipo: `List<type>`, onde `type` dos tipos:
    * Dado primitivo
    * sObject específico ou genérico
    * Tipo definido pelo usuário (classe) que contém variáveis suportadas acima.
  * `return` deve ser um do tipo `param` ou void.

* **Exemplo:**

```java
public class AccountQueryAction {

  @InvocableMethod(label='Get Account Names' description='Returns account names' category='Account')
  public static List<String> getAccNames(List<Id> ids) {
    List<String> accNames = new List<String>();
    List<Account> accs = [SELECT Name FROM Account WHERE Id in :ids];
    for (Account acc : accs) {
      accNames.add(acc.Name);
    }
    return accNames;
  }
}
```

* OBS: Perceba que o retorno do método @InvocableMethod é void ou vários tipos de list, assim como o parâmetro.
Isso se dá pois o Flow pode receber 1 ou múltiplos registros e todo o fluxo deve considerar a bulkificação.  
Além disso, se o método @InvocableMethod não retornar void, a list retornada deve ter o mesmo tamanho que a list de input.

* Para acessar o método no Flow Builder:
  * Setup > Flow > Criar novo/ Alterar Existente > Action

  ![[apex-from-flow.png]]

* Para acessar o método no Process Builder:
  * Setup > Process Builder > Criar novo/ Alterar Existente > Add Action

  ![[apex-from-process.png]]


  **OBS:** Uma outra forma de dar acesso à um método Apex é usar a interface Process.Plugin, mas o Salesforce recomenda o uso de métodos @InvocableMethod.

#### Invocable variables
* Invocable variables são variáveis Apex declaradas com a tag `@InvocableVariable` que podem ser acessadas por Flows e Processes. Têm a sintaxe:

```java
@InvocableVariable[(label='myLabel' description='myDescription' required=(true|false))]
```

* São uma forma de passar mais de um parâmetro para métodos `@InvocableMethod`, ao definir um parâmetro de tipo definido pelo usuário que contém essas variáveis.
* O tipo de uma `@InvocableVariable` deve ser um dos:
  * Dado primitivo
  * sObject genérico ou específico
  * List ou List de List de dados primitivos, sObjects, objetos criados de classes Apex ou collections

* **Exemplo:**

```java
public class MathUtil {
  @InvocableMethod(label='Add 2 Numbers')
  public static List<Integer> add(List<FlowInput> lstFI) {
    List<Integer> results = new List<Integer>();
    for (FlowInput FI : lstFI) {
      Integer myNumber = FI.n1 + FI.n2;
      results.add(myNumber);
    }
    return results;
  }
  public class FlowInput {
    @InvocableVariable(label='number 1' required=true)
    public Integer n1;
    @InvocableVariable(label='number 2' required=true)
    public Integer n2;
  }
}
```

* Para acessar as variáveis @InvocableVariable no Flow Builder:
  ![[flow-invocable-variables.png]]

* Para acessar as variáveis @InvocableVariable no Process Builder:
 ![[process-invocable-variables.png]]
 
#### Executando Flows a partir do Apex
* Para executar um Flow em Apex, usamos a sintaxe:

```java
Map<String, Object> params = new Map<String, Object>{
  'inputName1' => value1
  'inputName2' => value2
  'inputNameN' => valueN
}
// Create flow and pass arguments
Flow.Interview.flowName instanceName = new Flow.Interview.flowName(params);
// Or create flow dynamically: 
// Flow.Interview instanceName = new Flow.Interview.createInterview('flowName', params);
// run flow
instanceName.start();
// get ouput
System.debug(flow.getVariableValue('ouputName'));
```

Onde: 
* `flowName` é um Flow do tipo `Autolaunched Flow (No Trigger)`
* `inputName*` e `ouputName`correspondem à nomes de variáveis no Flow

* **Exemplo:** 
* No Flow: 
  * Crie um Flow do tipo `Autolaunched Flow (No Trigger)`
  * Defina o nome do Flow como `Square`
  * Crie duas variáveis: 
    * `input` - tipo number, Available for input
    * `output` - tipo number, Available for output
  * Crie uma fórmula: nome `square`, fórmula: {!input} * {!input}
  * Crie um elemento assignment: 
    * Variable: `output`
    * Operator: Equals
    * Value: `square`
* No Apex:

  ```java
  Map<String, Object> params = new Map<String, Object> {
    'input' => 5
  };
  Flow.Interview.Square squareFlow = new Flow.Interview.Square(params);
  squareFlow.start();
  Decimal result = (Decimal) squareFlow.getVariableValue('output');
  System.debug('The result is ' + result); // exibe 25.0
  ```

### Platform Events
#### Introdução
* Platform events é um recurso do Salesforce baseado no design pattern **Event-Driven Architecture** (EDA).
* No EDA, um serviço específico **publica** um **evento** sempre que este cria ou atualiza dados. Outros serviços podem **se inscrever** nesses eventos emitidos pelo primeiro serviço.
* A vantagem desse modelo é manter consistência dos dados entre múltiplos serviços sem necessidade de transações distribuídas.
* Terminologia:
  * Event Producer: O publicador de um evento de mensagem em um `Channel`
  * Event Consumer: Um inscrito (subscriber) em um `Channel` que recebe mensagens desse `Channel`
  * `Channel`: É o canal usado pelo `Event Producer` para transmitir a mensagem
  * Event: Um mudança de estado que é importante num processo de negócio, como por exemplo, a geração de um pedido.
  * Event Notifier: Uma mensagem que contem dados sobre o evento.

#### Como um platform event funciona?
1. Definimos um platform event e seus campos
   * Criamos um platform event em: Setup > Integrations > Platform Events > New Platform Event.
     * Notas sobre Platform Events:
       * São como Custom Objects, mas seu API Name termina com __e
       * Ao serem criados, vêm com permissão desabilitada para todos os perfis.
       * Não são buscados por SOQL ou SOSL
       * Apenas triggers after insert são suportadas
       * O "entity type" da execução de um platform event é `Automated Process`.
       * A lista de inscritos e triggers de um platform event são localizados nas seções `Subscription` e `Triggers` na página deste.
   * Criamos campos no platform event, em Custom Fields & Relationships > New. Os tipos de dados disponíveis são:
      * Checkbox
      * Date
      * Date/Time
      * Number
      * Text
      * Text Area (Long)

2. Publicamos o platform event ao criar um Process ou Trigger a partir do objeto do platform event. Numa trigger, isso é feito com a sintaxe:

  ```java
  List<EventName__e> events = new List<EventName__e>();
  for (...) {
    EventName__e event = new EventName__e(field1 = value1, field2 = value2, fieldN = valueN);
    events.add(event);
  }

  if(events.size()>0){
    EventBus.publish(events);
  }
  ```

3. Inscrevemos um serviço no objeto do platform event, que pode ser:
     * Trigger
     * Flow
     * Process
     * CometD
* Numa trigger, a sintaxe é essa:

  ```java
  // Note o único trigger event suportado: after insert
  trigger triggerName on EventName__e (after insert) {
    // trigger.new é a lista de eventos passada como argumento em EventBus.publish(events);
  }
  ```

## User Interface
### Visualforce
#### Introdução
* Visualforce (VF daqui pra frente) é uma linguagem de marcação case-insensitive, similar a HTML, e que suporta HTML.
* Quando usar? Quando a interface padrão do Salesforce não consegue atender um requisito de negócio. Por exemplo:
  * Exibir mais de 2 colunas na User Interface (o padrão é 2)
  * Exibir dados de objetos diferentes não relacionados
* Tags VF têm o prefixo `apex:` e todas as páginas devem ser inclusas dentro das tags `<apex:page>` e `</apex:page>`
* Pode ser escrita em:
  * Development Mode Footer - Habilita um footer em páginas VF para o usuário com os campos habilitados: `Development Mode` e `Show View State in Development Mode`
  * Developer Console
  * Setup (Custom Code > Visualforce Pages)
  * IDE

* **Exemplo:**

  ```html
  <apex:page>
    <apex:pageBlock title="Page Block Title">
          <!-- apex:pageBlockSection deve estar dentro de um apex:pageBlock -->
          <apex:pageBlockSection title="Section 1" columns="1">
            section 1 body
          </apex:pageBlockSection>
          <apex:pageBlockSection title="Section 2" columns="1">
            section 2 body
          </apex:pageBlockSection>
    </apex:pageBlock>
  </apex:page>
  ```

  Resultado:
  ![[vf-page.png]]

* A referência de todos os componentes (tags) VF podem ser encontrados em `instance/apexpages/apexcomponents.apexp`, onde `instance` é sua instância Salesforce, por exemplo: https://psilva-dev-ed.my.salesforce.com/apexpages/apexcomponents.apexp

#### Trabalhando com dados do Salesforce na VF
* Para exibir e enviar dados para o banco de dados Salesforce, um **controller** deve ser usado (referência do [MVC](#mvc-pattern)). Existem 3 tipos de controller:
  * Standard controller
    * Para usar esse controller para um único registro: 
      * Definimos o atributo `standardController` na tag `apex:page` com o nome do objeto (standard ou custom) que iremos acessar.
      * Obtemos o ID de um registro específico e colamos na URL da página VF da seguinte forma: `instance/apex/vfName?id=recordId`.
      * Acessamos os atributos com a sintaxe `{!Object.field}`
    * Exemplo:
      ```html
      <apex:page standardController="Account">
        {!Account.Name}<br/>
        {!Account.Phone}<br/>
        <!-- É possível acessar registros de look up -->
        {!Account.Owner.Name} 
      </apex:page>
      ```
      URL: https://psilva-dev-ed--c.visualforce.com/apex/vfTest?id=0015Y00002ahOdZQAU

      Resultado:
      ```
      Express Logistics and Transport
      (503) 421-7800
      Paulo Fernando da Silva
      ```
    * Outros exemplos de tag úteis para o standardController:
      * apex:detail - traz todo o conteúdo da seção **detail** do objeto para a página
      * <apex:relatedList> - traz todo o conteúdo da seção **Related List** do objeto para a página.
      * \<apex:outputField value="{!Object.field}"> traz o label e value do campo `field` do objeto `Object`
    * Para lidar com múltiplos registros, podemos usar um Standard List Controller, que itera sobre uma coleção de registros. Para isso:
      * Além do atributo standardController, defina o atributo `recordSetVar="collectionName"`, onde `collectionName` é o nome da coleção a ser iterada.
      * Use componentes de iteração para exibir uma coleção, como o `apex:pageBlockTable` em conjunto com `apex:column`.
      * Exemplo:
        ```html
        <apex:page standardController="Contact" recordSetVar="contacts">
          <apex:pageBlock title="Contacts List">
            <apex:pageBlockTable value="{!contacts}" var="ct">
              <apex:column value="{!ct.FirstName}"/>
              <apex:column value="{!ct.LastName}"/>
              <apex:column value="{!ct.Account.Name}"/>
            </apex:pageBlockTable>
          </apex:pageBlock>
        </apex:page>
        ``` 
        Resultado:
        ![[vf-page-stdc-list.png]]

  * Custom controller
    * Diferente do standard controller, precisamos criar o custom controller, que é uma classe Apex referenciada na tag `apex:page` pelo atributo `controller`
    * **Exemplo:**
      * VF
      ```html
      <apex:page controller="MyCustomController">
        <!-- page body -->
      </apex:page>
      ```
      * Custom Controller
      ```java
      public class MyCustomController {
          // class body
      }
      ```

  * Controller extension
    * É uma classe Apex que estende a funcionalidade de um Standard ou Custom controller.
    * Uma ou mais controller extensions podem ser referenciadas, numa lista separada por vírgulas, através do valor do atributo `extensions` da tag `apex:page`
    * A classe deve conter um construtor com um único argumento de um dos tipos:
      * ApexPages.StandardController (para estender um standard controller)
      * CustomControllerName (para estender um custom controller com o nome `CustomControllerName`)
      * **Exemplo:**
        * VF
        ```html
        <apex:page controller="MyCustomController" extensions="MyControllerExtension">
          <!-- page body -->
        </apex:page>
        ```
        * Controller Extension
        ```java
        public class MyControllerExtension {
            public MyControllerExtension(MyCustomController mcc) {}
            /* Caso a extensão fosse para um standard controller...
            public MyControllerExtension(ApexPages.StandardController msc) {}
            */
            // other class content
        }
        ```
        * Custom Controller
        ```java
        public class MyCustomController {
            // class body
        }
        ```
    * **OBS:** Se mais de um controller extension atribuída ao atributo `extensions` definir o mesmo método, o método chamado será o da classe mais à esquerda da lista.
* Ambos Custom Controller e Controller Extensions podem implementar 3 tipos de método:
  * Métodos Get - Devem começar com `get` e retornam dados da controller para a view (padrão MVC)
  * Métodos Set - Devem começar com `set` e receber um argumento e enviam dados da view para a controller
  * Métodos Action - Métodos que não envolvam retornar ou inserir dados na Model

* **Exemplo:** 
 
  * Custom Controller:
    ```java
    public class MyCustomController {
      public String myVar;
      public String getMyVar() {
        return myVar;
      }
      public void setMyVar(String value) {
        myVar = value;
      }
    }
    ```
  * VF:
    ```html
    <apex:page controller="MyCustomController">
      <apex:form>
        <apex:inputtext value="{!myVar}"/> <br/>
        <apex:outputtext value="{!myVar}"/>
      </apex:form>
    </apex:page>
    ```

  * Resultado:  
  ![[vf-custom-ctl.png]]

#### Apex Properties
* Um recurso não exclusivo das VF são **Apex Properties**, que são como variáveis, mas usam **acessores** `get` e `set` para retornar e definir variáveis, respectivamente.
* A sintaxe da declaração de uma Apex property é:
  
  ```java
  accessModifier returnType propertyName {
    get { /* get code block */ }
    set { /* set code block */ }
  }
  ```

* **Exemplo:**

  * Apex class
    ```java
    public class MyClass {
      public Integer myNumber {
        get { return myNumber; }
        set { myNumber = value; } // value referencia o valor a ser atribuído à myNumber.
      }
    }

    // Uso em Apex class
    MyClass mc = new MyClass();
    mc.myNumber = 10; // chama o acessor set
    System.debug(mc.myNumber); // chama o acessor get e exibe 10
    ```

  * VF
    ```html
    <apex:page controller="MyClass">
      <apex:form>
        <apex:inputtext value="{!myNumber}"/> <br/>
        <apex:outputtext value="{!myNumber}"/>
      </apex:form>
    </apex:page>
    ```

* A definição de Apex Properties pode ser simplificada se os acessores `get` e `set` irão apenas retornar e definir variáveis, respectivamente. Para isso, definimos **automatic properties**. Basta omitir o bloco do get ou set e substituir por `;`.
* Se um acessor `get` não for definido, a variável será somente escrita, e se o `set` não for definido, será somente leitura. Somente escrita ou somente leitura significa que um erro será lançado caso tentemos acessar ou definir essa variável.
* **Exemplo:**

  ```java
  public class AutomaticProperty {
    public Integer myReadOnlyProp { get; }
    public Double myReadWriteProp { get; set; }
    public String myWriteOnlyProp { set; }
  }
  ```

#### Standard Controller vs Custom Controller vs Controller Extension
* No contexto de controller de VF, podemos categorizar dados e ações em:
  * standard data - dados de um ou múltiplos registros do mesmo objeto
  * custom data - dados de quaisquer objetos Salesforce
  * standard behaviour - botões de ação padrão como save, edit, cancel...
  * custom behaviour - botões de ação criados pelo usuário
* Em resumo, usamos:
  * Standard Controller quando precisamos usar apenas os dados e funcionalidades padrão associados à um único objeto (standard data e standard behaviour).
  * Custom Controller quando precisamos usar dados e funcionalidades customizadas, e/ou acessar dados de múltiplos objetos não relacionados (custom data e custom behaviour).
  * Controller Extension quando precisamos estender a funcionalidade de um standard controller ou custom controller.

#### Usando recursos estáticos em VF
* Para usar recursos estáticos, precisamos:
  1. Carregar o recurso no Salesforce: Isso é feito em Setup > Custom Code > Static Resources
  2. Referenciá-lo na página VF com a variável global `$Resource`. A sintaxe depende do tipo de arquivo e local:

    |Arquivo|Exemplo de tag VF|
    |-|-|
    |Imagem|<apex:image url="{!$Resource.TestImage}"/>|
    |Javascript|<apex:includeScript value="{!$Resource.MyJSFile}"/>|
    |Imagem em um arquivo|<apex:image url="{!URLFOR($Resource.MyZipFile, 'images/BlueHills.jpg')}"/>|
    |CSS em um arquivo|<apex:stylesheet value="{!URLFOR($Resource.MyStyleResources, 'styles.css')}"/>|

#### Incorporando páginas VF na plataforma Salesforce
* Há 5 formas de se fazer isso:

|Abordagem|Descrição|
|-|-|
|De uma guia|Adicione uma guia customizada (Setup > User Interface > Tabs > Visualforce Tabs > New)|
|Dentro de um Layout de Página padrão|Estenda seu layout de página ao embutir páginas VF nele|
|Sobrescrevendo botões padrão ou links|Substitua a funcionalidade padrão de botões e links para ir para uma VF em vez da página normal|
|Usando novos botões ou links|Adicione novos botões e links para ir para uma VF|
|Link direto para uma página VF|Cada VF tem um URL único, então pode ser distribuído em outros apps, emails, documentos, etc.|

### O framework Lightning Components e suas vantagens
#### Introdução
* O framework Lightning Components é um UI Framework para desenvolver aplicativos web para dispositivos mobile e desktop.
* É um framework para construção de aplicações de página única, com interfaces dinâmicas e responsivas.
* Usa Javascript no lado do cliente e Apex no lado do servidor:
  ![[lightning-framework-mvc.jpg]]
* Usa dois modelos de programação:
  * Lightning Web Components
  * Aura Components

#### Vantagens
1. Modular e flexível
2. Sensível ao dispositivo e responsivo
3. Melhor performance
4. Arquitetura baseada em eventos
5. Tempo de desenvolvimento reduzido
6. Pode ser usado em vários lugares

## Testing, Debbuging and Deployment
### Testing Deployment Requirement and Testing Framework
* Para testar classes Apex, escrevemos testes unitários, que são métodos de testes escritos em classes Apex chamadas classes de teste.
* Testes unitários não comitam no banco de dados ou enviam emails.
* Testes são **obrigatórios** para o deploy em produção.
* O código Apex pode ser implantado em produção ou no AppExchange a partir de uma ORG sandbox, mas não pode ser escrito diretamente em produção.
* Para o deploy em produção ou no AppExchange, é necessário que todo o código Apex da Org tenha no mínimo 75% de cobertura de testes e cada trigger deve ter pelo menos 1% de cobertura.
  * Ao fazer deploy para produção, todos os testes unitários são executados
  * Chamadas ao System.debug não contam como cobertura de código
  * Classes e métodos de teste não contam como parte da cobertura de código
* Para que o deploy tenha sucesso:
  * Cada teste unitário deve passar
  * Cada trigger deve ter alguma cobertura
  * Todas as classes e triggers devem ser compiladas com sucesso
* A cobertura de código é calculada da seguinte forma: CodeCoverage = testLinesExecuted / totalApexCodeLines, onde `testLinesExecuted` é o total de linhas de código Apex executadas durantes os testes, e `totalApexCodeLines` é o total de linhas de código Apex da org (com exceção das classes de teste como já dito)
* Para executar testes, há 3 formas gerais:
  * Pela página de Setup:
    * Setup > Custom Code > Apex Test Execution > Select Tests > Run
    * Setup > Custom Code > Apex Classes > Run All Tests
    * Setup > Custom Code > Apex Classes > Selecione uma classe de teste > Run Test
  * Pelo Developer Console
  * Por uma IDE como o VSCODE

### Escrevendo Testes unitários
* Para escrever testes unitários básicos:
  * Criamos uma classe de testes com modificador de acesso `public` e notação `@isTest`, geralmente destinada a testar métodos de uma única classe Apex, mas que pode acabar testando métodos de outras classes que são chamados por esta.
  * Por ser destinada a testar uma única classe, é uma boa prática que o nome da classe de teste referencie a classe testada, por exemplo: `AccountTriggerHandlerTest`, onde `AccountTriggerHandler` é o nome da classe cujos métodos serão testados.
  * Para cada método a ser testado, criamos um método de teste com modificadores `public` e `static`, que retorna `void`, e também com a notação `@isTest`.
  * Para o nome de cada método, é uma boa prática que ele descreva o cenário que irá testar, seja positivo, ou negativo. Por exemplo, se o método **deve** fazer tal coisa, começamos o nome do método com `should` e se **não deve**, começamos com `shouldNot`.
  * No corpo de cada método, devemos executar os testes dentre a execução dos métodos `Test.startTest()` e `Test.stopTest()`. A chamada do método `Test.startTest` irá liberar um novo conjunto de limites de governança até a chamada de `Test.stopTest`.
  * É uma boa prática assegurar que os resultados esperados ocorreram, e se não, não deixar que o teste passe. Pra isso, usamos os métodos `System.assert*`:
  * Membros de classe privados não são acessados normalmente por classes de teste. Para acessá-los, precisamos da notação `@TestVisible` para cada membro privado.
  * Há casos em que precisamos condicionar o disparo de triggers ou lógicas que não queremos que afetem os limites de governança durante os testes. Nestes cenários, podemos usar o método `Test.isRunningTest()` que retorna `true` quando a execução estiver no contexto de testes, e `false` quando não.
    * **Dica:** Em alguns cenários de teste, podemos querer uma lógica sendo executada e em outros não, mas se usarmos apenas o `Test.isRunningTest()` para condicionar a execução, sempre teremos a lógica executada. Para resolver isso, uma estratégia é criar uma variável estática booleana na classe a ser testada, que possibilite alternar para um cenário de teste ou não.
    
    |Método|Descrição|
    |-|-|
    |System.assert(condition [,msg])|Verifica se `condition` = true, se não, lança erro com a mensagem opcional `msg`|
    |System.assertEquals(expected, actual [,msg])|Verifica se `expected` == `actual`, se não, lança erro com a mensagem opcional `msg`|
    |System.assertNotEquals(expected, actual [,msg])|Verifica se `expected` != `actual`, se não, lança erro com a mensagem opcional `msg`|
* **Exemplo:**
  ```java
  // classe a ser testada
  public class AccountService {
    public static void createAccount(String accName) {
      insert new Account(Name=accName);
    }
  }

  // classe de teste
  @isTest
  public class AccountServiceTest {
    @isTest
    public static void shouldCreateAccount() {
      Test.startTest();
      AccountService.createAccount('Paul');
      Test.stopTest();
      
      System.assert([SELECT Id FROM Account WHERE Name = 'Paul'].size() == 1);
    }
  }  
  ```

  * **OBS:** Como [vimos](#segurança-de-registros), métodos de teste são executados em System mode. Se quisermos forçar um bloco de código a executar usando as permissões de um usuário específico, podemos usar o `System.runas(user){codeblock}`, onde `user` é um registro de usuário e `codeblock` é o bloco de código a ser executado com as permissões deste. 
    * **Exemplo:** 
      ```java
      User u = [SELECT Id FROM User WHERE UserName='myuser@testorg.com'];
      System.runas(u) {
        // make tests
      }
      ```

### Gerando dados de teste
* Em muitos casos, precisamos gerar dados que serão consumidos pelos métodos a serem testados, já que classes de teste por padrão não têm acesso ao banco de dados, então só conseguem acessar registros criados dentro da classe de testes.
* Para gerar dados de teste, devemos:
  * Criar um método `public static void` com a notação `@testSetup`. Todos os registros criados dentro deste método são acessados por outros métodos dentro da classe de testes. Uma convenção de nome para ele é `setup`.
  * Dentro do método `setup`, temos 3 formas de criar dados:
    1. Diretamente: Cria-se os dados que serão usados no corpo do método `setup`. Exemplo: 

        ```java
        @testSetup
        public static void setup() {
          Account acc = new Account(Name='Test');
        }
        ```

    2. Usando uma classe Factory: Como o nome diz, é uma classe que cria registros, específicos pra testes. 
      * Esta classe:
        * Deve ter escopo `public` ou `global`
        * Deve ser definida com a notação `@isTest`
        * Pode conter métodos com parâmetros e que retornam valor (não devem incluir a notação `@isTest`)
      * Exemplo: 

        ```java
        @testSetup
        public static void setup() {
          List<Account> accs = TestDataFactory.createAccs(200);
          insert accs;
        }

        // Factory class
        @isTest
        public class TestDataFactory {
          public static List<Account> createAccs(Integer quantity) {
            List<Account> accsToCreate = new List<Account>();
            for (Integer i = 0; i <= quantity; i++) {
              accsToCreate.add(new Account(Name='Test'+i));
            }
            return accsToCreate;
          }
        }
        ```
    3. Carregando recursos estáticos:
       * Para isso:
         * Cria-se um arquivo csv com os campos de um objeto que se deseja criar os dados.
         * Importa-se esse csv para o Salesforce em Setup > Custom Code > Static Resources > New, com `Cache Control` = Public
         * Carrega-se o recurso estático chamando o método `Test.loadData(Object.sObjectType, 'staticResourceName')`, onde:
           * `Object` é o tipo de objeto para os campos carregados.
           * `staticResourceName` é o nome do recurso estático contendo o csv.
           * O método `Test.loadData` retorna `List<sObject>`, onde cada sObject pode ser convertido para um objeto concreto.
        * Exemplo: 
          * Recurso estático carregado de nome `testAccounts` com dados de registros de Account:
          ![[testloaddata-csv.png]]
          * Uso no código Apex:
          
          ```java
            @testSetup
            public static void setup() {
              List<sObject> accs = Test.loadData(Account.sObjectType, 'testAccounts');
            }

            @isTest
            public static void shouldDoSomething() {
              Account acc1 = (Account)accs[0];
              // other testing code
            }
          ```
* **OBS:** Podemos permitir que uma classe de teste acesse dados do banco de dados, sem precisar criar novos dados. Isto é feito definindo a propriedade `SeeAllData=true` da notação `@isTest` da classe: `@isTest(SeeAllData=true)`. Esses dados podem ser modificados dentro da classe de testes, mas não serão comitados para o banco de dados. Note que:
  * Ao usar `@isTest(SeeAllData=true)`, não podemos ter um método `@testSetup`
  * Não é recomendado usar `@isTest(SeeAllData=true)` pois usar registros reais que podem ser modificados/deletados pode causar resultados imprevisíveis nos testes.

### Executando Apex em Execute Anonymous
* Executar Apex anônimo é executar código sem necessidade de criar classes.
* Código anônimo não é salvo no banco de dados, então, se definimos uma classe em código anônimo por exemplo, esta não será salva no metadata.
* Pode ser executado através de:
  * Developer Console
  * Workbench
  * IDE
  * Pela chamada da API SOAP `executeAnonymous()`
* Mudanças no banco de dados são salvas, a não ser que um erro ocorra, nesse caso as mudanças sofrem rollback.
* Sua execução gera debug logs

### Monitorar e Acessar Debug Logs
* Debug logs registram operações em banco de dados, processos de sistema erros em transações ou ao executar testes unitários.
* Contêm níveis customizados de informação
* Têm limite de 2MB por log e 50MB de logs por ORG.
* Para ver debug logs, as permissões “Manage Users” ou “View all Data” é necessária.
* Podemos gerar/visualizar Debug logs:

  ||Gerar|Visualizar|
  |:-:|:-:|:-:|
  |**Setup Page**|✔️|✔️|
  |**Developer Console**|✔️|✔️|
  |**IDE**|❌|✔️|

* Para gerar debug logs a partir da Setup Page: Setup > Environments > Logs > Debug Logs > Seção User Trace Flags > New >
  * Traced Entity Type: O tipo de entidade para qual logs devem ser registrados
  * Traced Entity Name: O nome da entidade
  * Start Date / Expiration Date: Período de duração do log, com no máximo 24 horas.
  * Debug Level: Um conjunto de níveis de log para cada categoria de debug. Os níveis possíveis para cada categoria são:

    ||None|Error|Warn|Info|Debug|Fine|Finer|Finest|
    |:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
    |Database|✔️|||✔️||||✔️|
    |Workflow|✔️|✔️|✔️|✔️|||✔️|✔️|
    |Validation|✔️|||✔️|||||
    |Callouts|✔️|✔️|||||✔️|✔️|
    |Apex Code|✔️|✔️|✔️|✔️|✔️|✔️|✔️|✔️|
    |Apex Profiling|✔️|||✔️||✔️||✔️|
    |Visualforce|✔️|||✔️||✔️|✔️||
    |System|✔️|||✔️|✔️|✔️|||
    |Wave|✔️|✔️||✔️||✔️|✔️|✔️|
    |Nba|✔️|✔️||✔️||✔️|||

* Para gerar debug logs a partir do Developer Console:
  * Aba Debug > Change Log Levels...
* Note que no Developer Console só é possível gerar Debug Logs de Users, classes e triggers

* Para visualizar debug logs no VSCode, executamos o comando: `SFDX: Get Apex Debug Logs`

* O Traced Entity Type `User` logará informações de todas as ações de um usuário (o que pode envolver múltiplas classes). Se quisermos filtrar informações sobre as ações relacionadas a uma classe específica, temos que criar trace flags para o usuário e classe:
  * User: O usuário que será rastreado, com Debug Level com none em todos os níveis.
  * Apex Class: A classe que se deseja obter logs, com Debug Level com níveis desejados.

### Workbench
* Ferramenta cloud-based que permite:
  * Executar queries SOQL e SOSL
  * Exportar resultados de queries
  * Executar código anônimo
  * Obter informações de metadata
* Link de acesso: https://workbench.developerforce.com/login.php

### Deploying Metadata
* Deploy de metadata significa mover componentes metadata de um local para outro (entre orgs ou diretório local por exemplo).
* Algumas formas de realizar o deploy de metadatas são:
  * Change Sets
  * Packages
  * Ant Migration Tool

#### Change sets
* Change set é um grupo de componentes de metadata que formam um App ou funcionalidade.
* A vantagem é que é a forma mais simples de se fazer deploy.
* As desvantagens são:
  * O deploy só pode ser feito entre orgs relacionadas, isto é, entre **sandbox e produção** ou **sandbox e sandbox** relacionados. Não é possível fazer deploy de uma developer org para produção por exemplo.
  * Só é possível adicionar/alterar componentes. Para deletar, precisamos fazer manualmente ou usando outra ferramenta como o ANT.
* Para fazer deploy, precisa de 3 passos:
  1. Crie uma **deployment connection**, que é um link entre duas orgs, especificando a direção do deploy. Supondo que uma deployment connection seja criada entre a org sandbox `Dev1` (source) e a org produção (target):
     * Logue na org de produção
     * Vá em "Deployment Settings", onde estarão listadas todas as orgs relacionadas
     * Selecione `Dev1` > Establish Deployment Connection > Marque a opção "Allow Inbound Changes" para aceitar Change Sets desta org.
  2. Logue na org `Dev1`, crie o change set clicando em "Outbound Change Sets" > New > Defina seu Outbound change set
  3. Logue na org de produção e clique em "Inbound Change Sets" para visualizar a lista de change sets > Escolha entre `Validate`, `Deploy`, `Delete`.

#### Packages
* Packages são grupos de componentes, assim como change sets, mas podem ser distribuídos por link ou AppExchange, como já [vimos](#packages).
* São criados da seguinte forma:
  * Setup > Apps > Packaging > Package Manager > New > Defina os campos como Package Name, Language e Managed> Save > Adicione Components pela aba `Components` > Add > Escolha o component type > Add to Package > Upload > Defina os campos necessários > Upload
  * Use o link Instalation URL para distribuir o package para outros usuários

#### Ant Migration Tool
* É uma ferramenta para mover metadatas entre um diretório local e uma org Salesforce.

### Salesforce Environments e Sandboxes
* Enrivonments são orgs com objetivos específicos que caem em 3 categorias:
  * Production: O ambiente de produção
  * Development: Um sandbox isolado da produção para desenvolvimento
  * Test: Um sandbox isolado da produção para teste

### Sandbox
* São ambientes de cópia de um ambiente de produção específico.
* O desenvolvimento de aplicações deve sempre começar no sandbox
* Use-os para desenvolver, testar e treinar sem comprometer os dados e aplicações da sua org de produção
* Os tipos de sandbox são:

|Tipo|Intervalo de refresh|Limite de armazenamento|O que é copiado|Sandbox templates|
|:-:|:-:|:-:|:-:|:-:|
|Developer Sandbox|1 dia|* Data Storage: 200MB<br>* File Storage: 200MB|Apenas Metadata|Não disponível|
|Developer Pro Sandbox|1 dia|* Data Storage: 1GB<br>* File Storage: 1GB|Apenas Metadata|Não disponível|
|Partial Copy Sandbox|5 dias|* Data Storage: 5GB<br>* File Storage: O mesmo que sua production org|Metadata e dados parciais|Requerido|
|Full Sandbox|29 dias|O mesmo que sua production org|Metadata e dados parciais|Metadata e todos os dados|Disponível|

#### Básico do processamento assíncrono
* Os tipos de processamento assíncrono Apex são:

|Tipo|Descrição|Exemplo|
|-|-|-|
|Métodos futuros|Executam em seu próprio thread, apenas quando os recursos estão disponíveis|Web service callout|
|Batch Apex|Executa grandes tarefas que excederiam limites de processamento normais|Limpeza de dados ou arquivamento de registros|
|Queueable Apex|Similar a métodos futuros, mas fornece encadeamento de tarefas e permite uso de dados mais complexos|Executar operações sequenciais com serviços Web externos|
|Scheduled Apex|Agenda um código Apex para executar em determinado tempo|Tarefas diárias ou semanais|

* Alguns limites de governança são maiores ao usar Apex assíncrono (exceto Scheduled Apex, onde todos limites assíncronos são iguais aos síncronos), como o número total de queries SOQL e o tamanho do heap que dobram.
* Processos assíncronos usam um framework baseado em fila, onde seu ciclo de vida é dividido em 3 fases: 
  * Enqueue: A requisição é colocada numa fila junto com os dados necessários para processá-la.
  * Persistence: A requisição é armazenada.
  * Dequeue: A requisição é removida da fila e processada.

#### Métodos futuros
##### Introdução
* Métodos futuros são métodos que executam em uma thread separada de forma assíncrona quando os recursos estiverem disponíveis.
* Usam a notação `@future`
* São usados tipicamente para:
  * Callouts para serviços externos: Se um callout for feito de uma trigger ou depois de uma operação DML, devemos usar um método future ou queueable.
  * Operações que precisamos que executem em seu próprio thread.
  * Isolar operações DML em diferentes tipos de sObject para prevenir erro de mistura de DML (alguns sObjects não podem ser usados juntos em operações DML, mas esse é um caso peculiar).
* A ordem de execução não é garantida, e dois métodos futuros podem tentar atualizar o mesmo registro, causando um erro de runtime.

##### Sintaxe
Métodos futuros tem algumas regras:
* Devem ser `static` e retornar `void`
* Os parâmetros especificados só podem ser:
  * Tipos de dados primitivos
  * Arrays, ou coleções de tipos de dados primitivos
* Um padrão comum é passar para o método uma List de Ids de registro que queremos processar assincronamente. Exemplo:   

```java
global class someClass {

  @future
  public static void myFutureMethod(List<Id> recordIds) {
    List<Account> accs = [SELECT Id, Name FROM Account WHERE Id IN :recordIds];
    // process account records...
  }
}
```

##### Exemplo de método futuro com callout
* Como visto, callouts não devem ser chamados a partir de triggers ou depois de operações DML de forma síncrona. A razão é que um callout mantém a conexão com o banco de dados aberta enquanto a chamada externa durar, e isso é ruim. Ao executar o callout de forma assíncrona, o Apex não precisa ficar esperando o resultado do callout enquanto mantém a conexão com o banco de dados aberta.
* O código abaixo implementa dois métodos para callout:
  
```java
public class SMSUtils {

  // Quando a chamada for a partir de uma controller, etc., podemos fazer o callout sem o método futuro.
  public static String sendSMS(String fromNbr, String toNbr, String m) {
    // Supondo que SmsMessage.send() resulte num callout...
    String results = SmsMessage.send(fromNbr, toNbr, m);
    insert new SMS_Log__c(to__c=toNbr, from__c=fromNbr, msg__c=results);
    return results;
  }

  // Quando a chamada for a partir de uma trigger, etc., temos que chamar essa versão que envolve a função síncrona num método futuro. Note o uso do (callout=true) nesse caso. 
  @future (callout=true)
  public static void sendSMSAsync(String fromNbr, String toNbr, String m) {
    String results = sendSMS(fromNbr, toNbr, m);
    System.debug(results);
  }
}
```

##### Classes de teste
* Testar métodos futuros é similar ao teste de métodos comuns. Definimos o teste entre os métodos startTest e stopTest. A diferença é que o sistema coleta todos os métodos assíncronos após startTest ser executado, e executa todos sincronamente quando stopTest é executado.
* Como código de teste não faz callouts, temos que simular (mock) o callout para a cobertura de teste. Isso é feito criando uma classe que implementa a classe `HttpCalloutMock`.
Exemplo:  

```java
@isTest
global class SMSCalloutMock implements HttpCalloutMock {
  global HttpResponse respond(HttpRequest req) {
    // Cria resposta fake
    HttpResponse res = new HttpResponse();
    res.setHeader('Content-Type', 'application/json');
    res.setBody('{"status":"success"}');
    res.setStatusCode(200);
    return res;
  }
}
```

* Depois de criada a classe de mock, usamos na classe de teste, que tem um método apenas para testar o método assíncrono, já que este chama o síncrono:

```java
@IsTest
private class Test_SMSUtils {
  @IsTest
  private static void testSendSms() {
    Test.setMock(HtppCalloutMock.class, new SMSCalloutMock());
    Test.startTest();
      SMSUtils.sendSMSAsync('111', '222', 'Greetings!');
    Test.stopTest();
    // executa callout e checa os resultados
    List<SMS_Log__c> logs = [SELECT msg__c FROM SMS_Log__c];
    System.assertEquals(1, logs.size());
    System.assertEquals('success', logs[0].msg__c);
  }
}
```

##### Melhores práticas
Evite padrões que executem muitos métodos futuros em um período de tempo curto. Mas se for necessário fazer 2000 requisições ou mais, siga as práticas:
* Garanta execução mais rápida possível
* Se usar callouts, tente agrupar todos os callouts similares num único método futuro, em vez de usar múltiplos métodos futuros pra cada callout.
* Faça testes completos com grandes volumes. Se o método futuro é chamado de uma trigger, trabalhe com pelo menos 200 registros no teste.
* Considere usar Apex Batch em vez de métodos futuros para processar muitos registros assincronamente.

##### Pormenores
* Não podemos chamar um método futuro a partir de outro método futuro, ou invocar uma trigger que chama um método futuro enquanto executa um método futuro.
* Os métodos getContent() e getContentAsPDF() não podem ser usados com a notação @future.
* O limite de invocações de métodos futuros é 50 por chamada Apex, e um limite diário máximo.

#### Apex de lote
##### Introdução
* Apex de lote é uma classe destinada a processar uma grande quantidade de registros (daí o nome lote).
* Permite que a transação se mantenha dentro dos limites de governança já que cada lote processa por padrão 200 registros por vez, de forma assíncrona.
* Se um batch falhar, os outros ainda podem executar normalmente.

##### Sintaxe
* A classe Apex de lote deve:
  * Implementar a interface `Database.Batchable<sObject>` e a opcionalmente a interface `Database.Stateful`:  
    As transações não armazenam estado normalmente, ou seja, numa execução com 1000 registros, o Apex de lote processará 200 registros por lote por padrão, executando a classe 5 vezes, e a cada vez com um novo estado. Se quisermos por exemplo contar quantos registros foram processados, precisamos manter o estado entre as transações ao implementar `Database.Stateful`. Essa interface permite que variáveis membros da instância mantenham seus valores entre as transações.
  * Implementar os métodos:
    * `public (Database.QueryLocator | Iterable<sObject>) start(Database.BatchableContext bc)`  
      Coleta todos os registros a serem processados, podendo retornar essa coleção de forma simples (`Database.QueryLocator`, onde até 50 milhões de registros podem ser retornados), ou retorná-la após algum pré-processamento (`Iterable<sObject>`, com a quantidade de registros respeitando os limites de governança)

    * `public void execute(Database.BatchableContext bc, List<object> scope)`  
      Executa o processamento em cada lote de `List<object>` passado para esse método.

    * `public void finish(Database.BatchableContext bc)`  
    Executa operações de pós-processamento, como enviar um e-mail por exemplo.

* Execução da classe Apex de lote: Para executar a classe, basta instanciá-la, e passar o objeto instanciado como argumento para o método `Database.executeBatch()`, que retorna um `Id`:

  ```java
  BatchableClass batchObject = new BatchableClass();
  Id batchId = Database.executeBatch(batchObject);
  ```

  * Cada invocação de um Apex de lote gera um `Id` de um registro do tipo `AsyncApexJob`, que permite consultar dados sobre a execução via SOQL ou gerenciá-la com `Apex Job Queue` (será abordado depois).
  * Podemos especificar quantos registros queremos por lote no segundo parâmetro de `Database.executeBatch`:

    ```java
    Database.executeBatch(batchObject, 400);
    ```

##### Exemplo de Apex de lote:

```java
public class UpdateLeadSources implements Database.Batchable<sObject>, Database.Stateful {

  public Integer recordsProcessed = 0;
  
  public Database.QueryLocator start(Database.BatchableContext bc) {
    return Database.getQueryLocator(
      'SELECT Id, LeadSource FROM Lead'
    );
  }

  public void execute(Database.BatchableContext bc, List<Lead> scope) {
        
    List<Lead> leadsToUpdate = new List<Lead>();
    for(Lead lead : scope) {
        if (lead.LeadSource == 'Dreamforce') {
            lead.LeadSource = 'Dreamforce updated';
            leadsToUpdate.add(lead);
            recordsProcessed++;
        }
    }
    
    update leadsToUpdate;
  }

  public void finish(Database.BatchableContext bc) {
    System.debug('Records processed: ' + recordsProcessed);
    AsyncApexJob job = [
      SELECT Id, Status, NumberOfErrors, JobItemsProcessed, TotalJobItems, CreatedBY.Email
      FROM AsyncApexJob
      WHERE Id = :bc.getJobId()
    ];
  }
}

// uso
UpdateLeadSources updateLeadSources = new UpdateLeadSources();
Database.executeBatch(updateLeadSources);
```

##### Classes de teste
Há apenas um ponto a se atentar durante a criação de classes de teste: Para o método setup, crie no máximo 200 registros pois classes de teste só executam uma vez, portanto um único lote. Exemplo:

```java
@isTest
private class LeadProcessorTest {
	@testSetup
    static void setup() {
        List<Lead> leadsToInsert = new List<Lead>();
        for (Integer i = 0; i < 200; i++) {
            leadsToInsert.add(new Lead(LeadSource = 'Dreamforce', LastName = 'LastName', Company = 'Company'));
        }
        insert leadsToInsert;
    }
    
    @isTest
    static void test() {
        Test.startTest();
        	LeadProcessor leadProcessor = new LeadProcessor();
        	Id batchId = Database.executeBatch(leadProcessor);
        Test.stopTest();
        System.assertEquals(200, [SELECT Count() FROM Lead WHERE LeadSource = 'Dreamforce updated']);
    }
}
```

##### Melhores práticas
* Ajuste as queries SOQL para executar o mais rápido possível.
* Minimize o número de chamadas assíncronas
* Cuidado com Apex de lote dentro de triggers para não exceder o número de execução de batches.
* Só use Apex de lote se houver mais de um lote de registros à processar, caso o contrário, considere usar Queueable Apex (próximo tópico).

#### Queueable Apex
##### Introdução
Queueable Apex é um superconjunto dos métodos futuros, possuindo os benefícios adicionais:
* Tipos de dados não primitivos: Diferente de métodos futuros que só podem receber tipos de dados primitivos ou coleções destes, o queueable Apex pode receber objetos.
* Monitoramento: Ao invocar o job usando o método System.enqueueJob(), este retorna um Id de um registro de AsyncApexJob, permitindo monitorar o progresso do job via query ou pela interface do Salesforce.
* Chaining jobs: Podemos encadear jobs ao executar uma segunda tarefa a partir de um job sendo executado.
* Até 50 jobs podem ser colocados em fila.

Na maioria dos casos é preferível usar queueable Apex do que métodos futuros, a não ser em casos de refatoração em que apenas parte do código deve ser assíncrono. Neste caso é mais fácil apenas envolver o código assíncrono num método futuro do que refatorar tudo para queueable Apex.

##### Sintaxe
A sintaxe é semelhante ao Apex de lote. A classe deve:
* Implementar a interface `Queueable`
* Implementar o método `public void execute()`

* Para colocar o job na fila, criamos uma instância da classe e a passamos como argumento para `System.enqueueJob()`, que por sua vez retorna um Id de `AsyncApexJob` que pode ser monitorado, assim como no Apex de lote.

##### Exemplo de queueable Apex

* Definição da classe

```java
public class UpdateParentAccount implements Queueable {
  private List<Account> accounts;
  private Id parent;
  public UpdateParentAccount(List<Account> records, ID id) {
    this.accounts = records;
    this.parent = id;
  }
  public void execute(QueueableContext context) {
    for (Account account : accounts) {
      account.parentId = parent;
      // executa outro processamento ou callout
    }
    update accounts;
  }
}
```

* Uso

```java
List<Account> accounts = [SELECT Id FROM Account WHERE billingstate = 'NY'];
Id parentId = [SELECT Id FROM Account WHERE Name = 'ACME Corp'][0].Id;

UpdateParentAccount updateJob = new UpdateParentAccount(accounts, parentId);

Id jobId = System.enqueueJob(updateJob);
```

* Monitorar progresso do job
  
```java
SELECT Id, Status, NumberOfErrors FROM AsyncApexJob WHERE Id = :jobId
```

* Teste

```java
@isTest
public class UpdateParentAccountTest {
  @testSetup
  static void setup() {
    List<Account> accounts = new List<Account>();
    accounts.add(new Account(name='Parent'));

    for(Integer i = 0; i < 100; i++) {
      accounts.add(new Account(
        name='Test Account'+i
      ))
    }
    insert accounts;
  }

  @isTest
  static void testQueueable() {
    Id parentId = [SELECT Id FROM Account WHERE Name = 'Parent'][0].Id;
    List<Account> accounts = [SELECT Id FROM Account WHERE Name LIKE 'Test Account%'];
    UpdateParentAccount updater = new UpdateParentAccount(accounts, parentId);
    Test.startTest();
    System.enqueueJob(updater);
    Tes.stopTest();
    System.assertEquals(100, [SELECT count() FROM Account WHERE parentId = :parentId]);
  }
}
```

##### Encadeando jobs
Podemos encadear jobs ao colocá-los na fila dentro do execute de outro job. Apenas um job filho pode ser encadeado por classe, mas podemos ter vários encadeamentos, dependendo da edição da org:

```java
public class FirstJob Implements Queueable {

  public void execute(Queueable context) {
    System.enqueueJob(new SecondJob());
  }
}
```

##### Callouts dentro do execute()
Podemos fazer callouts no método execute de duas formas:
* Chamando um método futuro que faz o callout.
* Implementando a interface `Database.AllowsCallouts` e fazendo o callout direto no método execute.
A segunda forma é a recomendada. Exemplo:

```java
public class AsyncExecution implements Queueable, Database.AllowsCallouts {
    public void execute(QueueableContext context) {
        //your code including the callout     
    }
}
```

#### Scheduled Apex
##### Introdução
Apex agendado (Scheduled Apex) é uma forma de executar classes em um dia e tempo específicos.

##### Sintaxe
* Definição da classe: A classe agendada deve:
  * Implementar a interface `Schedulable`
  * Implementar o método `void execute(SchedulableContext ctx)`.
* Uso: Para agendar a execução da classe, usamos `System.schedule(jobName, sch, scheduleObj)`, onde:
  * `jobName` é uma String definindo o nome do job
  * `sch` é uma String de uma *Expressão CRON*, que representa a data e o tempo de execução.
  * `scheduleObj` é uma instância da classe que implementa a interface `Schedulable`

##### Exemplo

```java
public class RemindOpptyOwners implements Schedulable {
  public void execute(SchedulableContext ctx) {
    List<Opportunity> opptys = [SELECT Id, Name, OwnerId, CloseDate
      FROM Opportunity
      WHERE IsClosed = False AND
      CloseDate < TODAY
    ];
    // Supondo que o método TaskUtils.remindOwners criasse uma task para cada oportunidade...
    TaskUtils.remindOwners(opptys);
  }
}

RemindOpptyOwners reminder = new RemindOpptyOwners();
// Segundos, minutos, hora, dia, mês dia_da_semana, ano_opcional
String sch = '20 30 8 19 2 ?'
String jobId = System.schedule('Remind Opp Owners', sch, reminder);
```

##### Classe de teste
Como outros métodos assíncronos, o Apex agendado será executado de forma síncrona após `Test.stopTest()`

```java
@isTest
private class RemindOpptyOwnersTest {
  public static String CRON_EXP = '0 0 0 15 3 ? 2022';
  @isTest
  static void testScheduledJob() {
    List<Opportunity> opptys = new List<Opportunity>();
    Date closeDate = Date.today().addDays(-7);
    for (Integer i = 0; i < 10; i++) {
      Opportunity o = new Opportunity(
        Name = 'Opportunity ' + i,
        CloseDate = closeDate,
        StageName = 'Prospecting'
      );
      opptys.add(o)
    }
    insert opptys;

    Map<Id, Opportunity> opptyMap = new Map<Id, Opportunity>(opptys);
    List<Id> opptyIds = new List<Id>(opptyMap.keySet());
    Test.startTest();
    String jobId = System.schedule('ScheduledApexTest', CRON_EXP, new RemindOpptyOwners());
    List<Task> lt = [
      SELECT Id FROM Task WHERE WhatId IN :opptyIds
    ];
    System.assertEquals(0, lt.size());
    Test.stopTest();
    lt = [
      SELECT Id FROM Task WHERE WhatId IN :opptyIds
    ];
    System.assertEquals(opptyIds.size(), lt.size());
  }
}
```

##### Criando Schedule Apex pela UI
Podemos criar a classe schedule Apex pela interface em: 
Setup > Custom Code > Apex Classes > Schedule Apex. Defina o job name, a classe Apex, o período, e salve em `Save`.

##### Importante
Alguns pontos a se atentar ao usar scheduled Apex:
* Podemos ter até 100 jobs agendados de uma vez e existe uma quantidade máxima de execuções de schedule Apex durante um período de 24h.
* Cuidado com scheduled Apex dentro de triggers para não agendar mais jobs que o limite.
* Web service callouts síncronos não são suportados por scheduled Apex. Para fazer callouts, crie um callout assíncrono (dentro de um método futuro) e o chame de dentro da classe scheduled.

#### Monitorar Apex assíncrono


### Apex Integration Services

#### Apex REST Callouts

##### Introdução
Callouts REST são baseados em HTTP, onde cada requisição de callout está associada a:
1. Um método HTTP;
2. Um endpoint (também chamado URI - Uniform Resource Identifier)
3. Header (quando o método envolve criar/deletar/atualizar dados)
4. Body (quando o método envolve criar/deletar/atualizar dados)
Um callout Apex faz uma requisição para um endpoint do Web Service, que por sua vez retorna uma resposta ao Salesforce.

![[HTTP-request.png]]

##### Autorizando um endpoint
Para acessarmos um endpoint, precisamos autorizar seu endereço no Salesforce. Isto é feito em:
1. Setup > Remote Site Settings > New Remote Site
2. Preencha os campos Remote Site Name e Remote Site URL
3. Save

##### Métodos HTTP
Métodos HTTP fazem CRUD em dados de recursos do Web Service. Um exemplo de recurso é o objeto Account, que contem dados como Id, Name, Type, etc.

|Método|Descrição|
|-|-|
|GET|Recebe dados identificados por um URL|
|POST|Cria um recurso ou insere dados no servidor|
|DELETE|Deleta um recurso identificado por um URL|
|PUT|Cria ou recurso ou o substitui se este já existir|
|PATCH|Atualiza dados de um recurso existente|

##### Sintaxe
A sintaxe depende do método usado, mas em geral a diferença é que para o método `GET` não precisamos executar os métodos `setMethod` e `setHeader`, enquanto para os métodos `POST`, `DELETE`, `PUT` e `PATCH`, a execução é necessária.

```java
HTTP http = new Http();
HttpRequest request = new HttpRequest();
request.setEndPoint('endpointURL');
request.setMethod('HTTP_METHOD'); // GET | POST | DELETE | PUT | PATCH
request.setHeader('Content-Type', 'application/json; charset=UTF-8'); // APENAS se HTTP_METHOD != GET
request.setBody('{"property1":"value1"}'); // APENAS se HTTP_METHOD != GET
HttpResponse response = http.send(request);

if (response.getStatusCode() == statusCode) { // statusCode é um Integer representando status de sucesso (200-299)
  System.debug(response.getBody()); // response.getBody() retorna uma string com os resultados da requisição, se houver sucesso.
} else {
  // Se não, podemos verificar qual foi o código de status e o status (mensagem de erro)
  System.debug('The status code returned was not expected: ' + response.getStatusCode() + ' ' + response.getStatus());
}
```

##### Exemplos

###### GET

```java
HTTP http = new Http();
HttpRequest request = new HttpRequest();
request.setEndPoint('https://th-apex-http-callout.herokuapp.com/animals');
request.setMethod('GET');
HttpResponse response = http.send(request);

if (response.getStatusCode() == 200) {
  // Desserializamos o resultado da requisição para transformá-lo num Object
  Map<String, Object> results = (Map<String, Object>) JSON.deserializeUntyped(response.getBody());

  List<Object> animals = (List<Object>) results.get('animals');
  for (Object animal : animals) {
    // Cada dado (animal) agora poderia ser convertido para seu tipo específico, mas apenas os exibimos no console.
    System.debug(animal);
  }
} else {
  System.debug('The status code returned was not expected: ' + response.getStatusCode() + ' ' + response.getStatus());
}
```

###### SET

```java
HTTP http = new Http();
HttpRequest request = new HttpRequest();
request.setEndPoint('https://th-apex-http-callout.herokuapp.com/animals');
request.setMethod('POST');
request.setHeader('Content-Type', 'application/json; charset=UTF-8');
request.setBody('{"name":"mighty moose"}');
HttpResponse response = http.send(request);
if (response.getStatusCode() == 201) {
    // "mighty moose" deve ser exibido no fim do array animals
    System.debug(response.getBody());
} else {
  System.debug('The status code returned was not expected: ' + response.getStatusCode() + ' ' + response.getStatus());
}
```

##### Testando Callouts
Métodos de teste não conseguem fazer callouts, então para testarmos callouts, devemos simular uma resposta da requisição (criar um mock response) e usá-la no método de teste.  
Essa resposta simulada deve ser definida antes do callout ser executado, através do método: `Test.setMock(interfaceType, instance)`, onde `insterfaceType` é do tipo System.type (no caso de callouts REST é sempre `HttpCalloutMock.class`) e `instance` é um Object representando o a instância do mock.  
Há dois tipos de `instance` para se criar mocks, o que depende do tipo de requisição:
* Para requisições do tipo `GET`: o `instance` é do tipo `StaticResourceCalloutMock`, que usa um recurso estático. Para isso:
  * Criamos um recurso estático em File > New > Static Resource. Seu MIME Type deve ser `text/plain`, e seu conteúdo deve ser o corpo da resposta. Exemplo:
    ```js
    // arquivo GetAnimalResource.txt
    {"animals": ["pesky porcupine", "hungry hippo", "squeaky squirrel"]}
    ```
  * Criamos o método de teste:
    ```js
      @isTest
      static void testGetCallout() {
        StaticResourceCalloutMock mock = new StaticResourceCalloutMock();
        mock.setStaticResource('GetAnimalResource');
        mock.setStatusCode(200);
        mock.setHeader('Content-Type', 'application/json;charset=UTF-8');
        Test.setMock(HttpCalloutMock.class, mock);
        HttpResponse result = AnimalsCallouts.makeGetCallout();
        // asserts com result...
      }
    ```

* Para requisições tipo `POST`, `DELETE`, `PUT` e `PATCH`: o `instance` é uma classe que implementa a interface `HttpCalloutMock`. Para isso:
  * Criamos uma classe que implementa a interface `HttpCalloutMock`, que deve implementar seu método `respond`, que retorna a resposta:
  
    ```js
    @isTest
    public class AnimalsHttpCalloutMock implements HttpCalloutMock {
      public HttpResponse respond(HttpRequest request) {
        HttpResponse response = new HttpResponse();
        response.setHeader('Content-Type', 'application/json');
        response.setBody('{"animals": ["majestic badger", "fluffy bunny", "scary bear", "chicken", "mighty moose"]}');
        response.setStatusCode(200);
        return response;
      }
    }
    ```

  * Criamos o método de teste:
  
  ```js
  @isTest
  static void testPostCallout() {
    Test.setMock(HttpCalloutMock.class, new AnimalsHttpCalloutMock());
    HttpResponse response = AnimalsCallouts.makePostCallout();
    // asserts com response...
  }
  ```

##### Exemplo final

```js
// arquivo AnimalsCallouts.cls
public class AnimalsCallouts {
  public static void makeGetCallout {
    HTTP http = new Http();
    HttpRequest request = new HttpRequest();
    request.setEndPoint('https://th-apex-http-callout.herokuapp.com/animals');
    request.setMethod('GET');
    HttpResponse response = http.send(request);

    if (response.getStatusCode() == 200) {

      Map<String, Object> results = (Map<String, Object>) JSON.deserializeUntyped(response.getBody());

      List<Object> animals = (List<Object>) results.get('animals');
      for (Object animal : animals) {
        System.debug(animal);
      }
    } else {
      System.debug('The status code returned was not expected: ' + response.getStatusCode() + ' ' + response.getStatus());
    }
  }

  public static void makePostCallout {
    HTTP http = new Http();
    HttpRequest request = new HttpRequest();
    request.setEndPoint('https://th-apex-http-callout.herokuapp.com/animals');
    request.setMethod('POST');
    request.setHeader('Content-Type', 'application/json; charset=UTF-8');
    request.setBody('{"name":"mighty moose"}');
    HttpResponse response = http.send(request);
    if (response.getStatusCode() == 201) {

        System.debug(response.getBody());
    } else {
      System.debug('The status code returned was not expected: ' + response.getStatusCode() + ' ' + response.getStatus());
    }
  }
}

// arquivo GetAnimalResource.txt
{"animals": ["pesky porcupine", "hungry hippo", "squeaky squirrel"]}

// arquivo AnimalsHttpCalloutMock.cls
@isTest
public class {
  @isTest
  public class AnimalsHttpCalloutMock implements HttpCalloutMock {
    public HttpResponse respond(HttpRequest request) {
      HttpResponse response = new HttpResponse();
      response.setHeader('Content-Type', 'application/json');
      response.setBody('{"animals": ["majestic badger", "fluffy bunny", "scary bear", "chicken", "mighty moose"]}');
      response.setStatusCode(200);
      return response;
    }
  }
}

// arquivo AnimalsHttpCalloutsTest.cls
@isTest
private AnimalsHttpCalloutsTest
    @isTest
    static void testGetCallout() {
      StaticResourceCalloutMock mock = new StaticResourceCalloutMock();
      mock.setStaticResource('GetAnimalResource');
      mock.setStatusCode(200);
      mock.setHeader('Content-Type', 'application/json;charset=UTF-8');
      Test.setMock(HttpCalloutMock.class, mock);
      HttpResponse result = AnimalsCallouts.makeGetCallout();
    }

    @isTest
    public class AnimalsHttpCalloutMock implements HttpCalloutMock {
      public HttpResponse respond(HttpRequest request) {
        HttpResponse response = new HttpResponse();
        response.setHeader('Content-Type', 'application/json');
        response.setBody('{"animals": ["majestic badger", "fluffy bunny", "scary bear", "chicken", "mighty moose"]}');
        response.setStatusCode(200);
        return response;
      }
    }
```

##### Considerações finais
* Como já vimos na [introdução de Métodos futuros](#introdução-1), é importante que callouts sejam executados assincronamente (com notação `@future(callout=true)`) em certos cenários.

#### Apex Web Services
##### Introdução


### Leads e oportunidades para o Lightning Experience

#### Criar e converter leads em clientes potenciais
* Já vimos a [definição de lead](#corestandard-crm-objects). Agora vamos criar um: Abra a guia Leads > New > Preencha os campos obrigatórios > Save.
* A partir do registro de Lead, podemos gerenciar o status do lead (open, working, converted, etc), e atividades como envio de e-mail ou tasks e notícias por exemplo.
* Quando um lead é convertido (teve seu status atualizado para converted), uma tela se abrirá para criarmos/atribuirmos o lead para uma Account, Contact e Opportunity:

![[lead-conversion.png]]

OBS: Se o lead não incluia um company name, e se person accounts estiver habilitada, então só um person account e uma opportunity serão criados.
* O nome da Opportunity pode ser uma convenção, geralmente usando o nome da Account - produtos de interesse.


## Process Automation Specialist
#### Approval Processes
* Automatizam aprovações de registros, ou seja, quando um usuário faz um CRUD em algum registro, este pode ser enviado para aprovação através de um approval process.
* São criadas em: Setup > Process Automation > Approval Processes.  
![[approval-process.png]]

* As principais configurações de um Approval Process são:
  * Entry Criteria: Define o critério no qual um campo de objeto deve corresponder para o approval poder ser submetido.
  * Approval Assignment Email Template: O email template a ser utilizado para enviar a aprovação.
  * Initial Submission Actions: Ações automáticas executadas no envio do approval.
  * Approval Steps: Quantos e quais passos são executados, qual o aprovador de cada um, etc.
  * Final Approval Actions: O que acontece quando uma approval é aprovada (por todos os passos).
  * Final Rejection Actions: O que acontece quando uma approval é rejeitada (por todos os passos).
  * Recall Actions: O que acontece quando uma submissão ainda precisa de algo.

#### Escolha a ferramenta de automação certa
Entre Flow Builder, Process Builder e Apex, qual escolher?
* Priorize ferramentas declarativas (Flow builder e Process Builder), e programe soluções em Apex para soluções mais complexas. Nos mesmos cenários em que se pode usar um Flow builder ou Process builder, priorize o Flow Builder para novas automações de processos, enquanto para processos já existentes, use o Process Builder.
* Em geral, uma experiência orientada por processos é uma combinação de vários processos que caem em categorias, das quais podemos usar ferramentas mais adequadas:  

|Tipo de processo|Descrição|Ferramenta indicada|
|-|-|-|
|Experiência visual guiada|processos comerciais que precisam de dados de usuários (clientes ou funcionários)|Flow Builder|
|Automação nos bastidores|processos comerciais que obtém os dados necessários da org do Salesforce ou sistema conectado, sem necessidade de dados do usuário|* Flow Builder (recomendado) <br>* Process Builder (para processos já existentes)<br>* Apex|
|Automação de aprovação|processos comerciais que definem como um registro (como uma solicitação de folga), deve ser aprovado pelos stakeholders|Approvals|


# RESUMÃO DE COISAS QUE NÃO ME APROFUNDEI
## Custom Iterators
* São classes que implementam a interface `Iterator`, definindo os métodos `hasNext` e `next`

* Exemplo:

  ```java
  IterableString x = new IterableString('my iterable str');
  while(x.hasNext()){
    System.debug(x.next());
  }
  ```

* Só whiles suportam iterators
* Se quisermos criar nossa própria estrutura de dados para usar no `iterator`, devemos implementar a interface `Iterable`, que define o método `iterator`, que retorna um objeto tipo iterator.

## Classe Limits
* Contém métodos que retornam informações de limites para recursos específicos.
* Cada método tem duas versões com a variável sufixo `Resource`, onde `Resource` é o recurso em questão: 
  * getLimit`Resource`: Retorna o limite máximo de uso do recurso `Resource`
  * get`Resource`: Retorna a quantidade de usos do recurso `Resource` até o momento

* Exemplo: 

  ```java
  List<Account> accs = [
    SELECT Name
    FROM Account
  ];

  List<Contact> ctcs = [
    SELECT Name
    FROM Contact
  ];

  System.debug(Limits.getQueries()); // exibe: 2
  System.debug(Limits.getLimitQueries()); // exibe: 100
  ```

## SFDX e SFDX CLI
* O SFDX (DX de Developer Experience) é um conjunto de ferramentas que simplifica todo o ciclo de vida do desenvolvimento.
* Melhora o desenvolvimento e colaboração em equipe
* Facilita o teste automatizado e integração contínua
* Dentre as ferramentas, estão **Scratch Orgs**, que são ambientes Salesforce descartáveis e configuráveis definidos de forma rápida.

* O SFDX CLI é uma command line interface para simplificar o desenvolvimento e automação ao trabalhar com Orgs. É usado para:
  * Sincronizar recursos de/para a Org
  * Criar e gerenciar Orgs
  * Importar e exportar dados
  * Criar e executar testes
  * Criar e instalar pacotes

* Outro termo é Developer Hub Org (Dev Hub): É a principal Org usada para criar e gerenciar scratch Orgs.

## Schema Class
* Contém métodos para obter informações de schema.

|Método|Descrição|
|-|-|
|getGlobalDescribe()|Retorna um Map<String, Schema.SObjectType> onde as chaves são os nomes dos sObjectType e os valores são os sObject|
|describeDataCategoryGroups(sObjectNames)||
|describeSObjects(sObjectTypes)||
|describeSObjects(SObjectTypes, SOBjectDescribeOptions)||
|describeTabs()||
|GroupStructures(pairs)||

## Automation Tool Features

||Process Builder|Flow Builder|Workflow|Approvals|
|:-:|:-:|:-:|:-:|:-:|
|**Complexidade**|Múltiplas instruções if/then|Complexo|Uma única instrução if/then|Uma única instrução if/then|
|**Visual Designer**|✔️|✔️|||
|**Inicia quando**|* Registro criado/editado <br> * Invocado por outro process <br> * Recebe mensagem de Plaftorm event|* CRUD de registro <br> * Usuário Clica em botão/link, acessa uma página ou utility bar <br> * Invocado por Process <br> * Invocado por Apex|Registro criado/editado|* Usuário Clica em botão/link <br> * Process ou Flow iniciam uma ação Submit for Approval <br> * Invocado por Apex|
|**Suporta ações agendadas**|✔️|✔️|✔️||
|**Suporta interação de usuário**||✔️|||
|**Invoca código Apex**|✔️|✔️|||
|**Invoca processes**|✔️||||
|**Invoca Flows**|✔️|✔️|||
|**Cria Registros**|✔️|✔️|apenas Tasks|apenas Tasks|
|**Deleta Registros**||✔️|||
|**Atualiza Campos**|Qualquer registro relacionado|Qualquer registro|O registro ou seu pai|O registro ou seu pai|
|**Posta no Chatter**|✔️|✔️|||
|**Envia email**|✔️(Apenas alertas de email)|✔️|✔️(Apenas alertas de email)|✔️(Apenas alertas de email)|
|**Envia Notificação Customizada**|✔️|✔️|||
|**Envia outbound messages**||✔️|✔️|✔️|
|**Envia para aprovação**|✔️|✔️|||

## Lightning Web Components (LWC)
* Para criar um LWC, precisamos de:
* Um arquivo HTML (obrigatório):
* Um arquivo JS (obrigatório):
* Um arquivo CSS (opcional):
* Aura components podem conter LWCs, mas não o contrário.
* Lightning Data Service (LDS) permite acessar dados e metadata do Salesforce.
* Lightning Locker previne que LWCs de um namespace acessem LWCs de outro.

### Criando um LWC:
* Crie uma pasta com os arquivos do componente com o mesmo nome. Para nomear apps, use o padrão **camelCase**, e o nome do componente será mapeado para o padrão **kebab-case**. Então, myComponent seria referenciado como `<c-myComponent>`.
  * Exemplo:

    ![name](lwc-app-folder.png)

* Crie um arquivo HTML com a tag `template` obrigatória e identificadores (variáveis com `{}`), que são vinculados à variáveis de mesmo nome no JS.
  * Exemplo:

    ```html
    <template>
      <div id="waiting" if:false={ready}>Loading…</div>
      <div id="display" if:true={ready}>
        <div>Name: {name}</div>
        <div>Description: {description}</div>v>
        <div>Price: {price}</div>
        <div><img src={pictureUrl}/></div>
      </div>
    </template>
    ```

* Crie o arquivo JS:
  * Exemplo:

  ```js
  import { LightningElement } from 'lwc';
  export default class App extends LightningElement {
    name = 'Electra X4';
    description = 'A sweet bike built for comfort.';
    category = 'Mountain';
    material = 'Steel';
    price = '$2,700';
    pictureUrl = 'https://s3-us-west-1.amazonaws.com/sfdc-demo/ebikes/electrax4.jpg';
    ready = false;
    connectedCallback() {
        setTimeout(() => {
            this.ready = true;
        }, 3000);
    }
  }
  ```

* Para usar plaftform events em LWC:

  ```js
  import {
    subscribe,
    unsubscribe,
    onError
  } from 'lightning/empAPI'
  ```

* Para um `child component` notificar um `parent component`, podemos usar um `Custom event`:

  * No filho:
  ```js
  handleClick(event) {
    this.dispatchEvent(new CustomEvent('previous'));
  }
  ```

  * No pai:
  ```html
  <template>
    <c-navigate-buttons
      onprevious={previousHandler}>

    </c-navigate-buttons>
  </template>
  ```

* Para expor um método à uma API SOAP, este deve ser definido com a key-word `webservice`:

  ```java
  webservice static Id makeContact(...)
  ```

* Recursos acessados por LWC:
  * Content Asset files
  * Static Resources
  * SVG Resources

* Em LWC, para um component pai passar valores para o filho, há 2 formas:
  * O parent component invoca um método no child component
  * O parent component usa uma public property para passar dados para o filho

* Podemos usar o método setCreatedDate(recordId, createdDatetime) para definir a data de criação de um registro numa classe de teste (apenas).

* Um formula field pode ser usado para exibir imagens com a função IMAGE("URL", "name")

* Exemplos de campos polimórficos são:
  * Campo `Who` de uma Task que pode receber um Contact ou Lead
  * Campo `What` de um Evento, que pode receber Account, Opportunity, Solution

* Process Builder só pode enviar para aprovação, o próprio registro que o iniciou.

*  Não há garantia na ordem de execução de getters e setters para uma VF, e os getters são obrigatórios para acessar valores de uma controller, mas para passar valores pra controller, um setter não é obrigatório.

* Aura events:
  * Crie um Application Event:

  ```html
  <!-- Nome do HTML: myAppEvent -->
  <aura:event type="APPLICATION" description="my app event">
    <aura:attribute name="message" type="string">
  </aura:event>
  ```

  * Crie um Notifier:
  
  ```html
  <!-- Nome do HTML: Notifier -->
  <aura:component>
    <aura:registerEvent name="appEvent" type="c:myAppEvent">
    <!-- button com onclick={!c.fireAppEvent} -->
  </aura:component>
  ```

  ```js
  // Nome do js: Notifier.js
  ({
    fireAppEvent : function(component, event, helper) {
      let appEvent = $A.get('e.c:myAppEvent');
      appEvent.setParams({
        "message" : "an application event fired me."
      });
      appEvent.fire();
    }
  })
  ```

* Para expor um método Apex para um LWC:
  * O método deve ter a notação `@AuraEnabled` e ser `public`/`global` `static`
* A partir de um LWC, podemos acessar o método de 3 formas:
  * Wire de um método Apex à uma propriedade
  * Wire de um método Apex à uma função
  * Chamar métodos Apex imperativamente 
* Exemplo de `wire`:

  ```js
  // aqui, getAccounts é o método Apex, os parâmetros são passados como um objeto no segundo argumento, onde cada parâmetro do método corresponde à uma propriedade do objeto. Então getAccounts recebe uma String searchTerm. E accountList retorna o resultado da chamada.
  @wire(getAccounts, {searchTerm: '$searchTerm'})
  accountList;
  ```

* `with sharing` impõe **record-level** security, enquanto **object-level** security e **field-level** security devem ser manualmente impostas (CRUD and FLS)
* Para impor permissões **object-level**  **field-level**, há algumas formas:
  * Use à cláusula `WITH SECURITY_ENFORCED`: É a mais simples para quando a tratativa de erros de permissão não precisa ser muito detalhada. 
    * **Exemplo:**

      ```java
      public with sharing class MyController {
        @AuraEnabled
        public static List<Order__c> getOrders {
          return [
            SELECT Id, Name, Price, Client__c FROM Order
            WITH SECURITY_ENFORCED
          ];
        }
      }
      ```
    * Os campos e objetos de queries e subqueries que o usuário não tem acesso farão a query lançar um erro.  
  * Use o método `Security.stripInaccessible(acessType, records)`, onde:
    * `acessType` é um ENUM AccessType de um dos tipos:
      * CREATABLE
      * READABLE
      * UPDATABLE
      * UPSERTABLE
    * `records` é um registro ou lista de registros cujo o acesso é verificado.
    * O método remove os objetos e campos que o usuário atual não tem acesso, e não exibe erro se houver registros não acessíveis.
    * O método retorna um `SObjectAccessDecision` que tem os métodos:
      * getModifiedIndexes()
      * getRecords()
      * getRemovedFields()
    * **Exemplo:**

      ```java
      public with sharing class MyController {
        @AuraEnabled
        public static List<Order__c> getOrders {
          List<Order__c> orders = [
            SELECT Id, Name, Price, Client__c FROM Order
          ];
          sObjectAccessDecision decision = Security.stripInaccessible(AcessType.READABLE, orders);

          if (!decision.getModifiedIndexes().isEmpty()) {
            throw new AuraHandledException('Data was stripped');
          }
          return orders;
        }
      }
      ``` 
  * Usar a classe DescribeFieldResult (forma depreciada)
 * @remoteAction é uma notação usada em métodos Apex para poderem ser chamados por JS de VFs. Deve ser `public/global` `static`.
   * **Exemplo:**

    ```java
    global class RemoteActionSample {
      @remoteAction
      global static String myMethod() {}
    }
    ```

* Incluir estilo lightning em páginas VF: `<apex:page LightningStyleSheets="true">` 

* SOQL and Tooling API podem ser usados para checar a cobertura de testes de Processes e Flows ativos.
* Processes e Flows são implantados como inativos e precisam ser ativados manualmente, **exceto** quando se usa o modelo de integração e entrega contínua para deploy de metadados, nesse caso é possível habilitar uma opção pra isso.

* Lightning Data Service cuida de sharing rules e field-level security pra nós ;]

* Expondo um LWC para uso:
  * Para um LWC ser utilizável, devemos customizar o arquivo <component>.js-meta.xml com as tags `isExposed` como `true` e pelo menos um `target`:
  * **Exemplo:**
    
    ```xml
    ...
    <isExposed>true</isExposed>
    <targets>
      <target>lightning__RecordPage</target>
    </targets>
    ...
    ```
  * Os tipos de target são:
    * lightning__AppPage
    * lightning__FlowScreen
    * lightning__HomePage
    * lightning__inbox
    * lightning__RecordAction
    * lightning__RecordPage

* Trace flags podem ter os tipos de entidade:
  * Automated Process
  * Platform Integration
  * User
  * Apex Class
  * Apex Trigger

* `NoAccessException` é um tipo de exceção que ocorre quando o perfil não tem acesso a um sObject.

* Evento Monitoring é uma ferramenta que permite registrar detalhes de atividades de usuário na org, e ver essas atividadades como `eventos`.

* A tag <ltng:require> pode:
  * Definir a ordem de loading
  * Carregar scripts em paralelo
  * Tem one-time loading para scripts duplicados

* Podemos fazer override de botões padrão usando VF ou Lightning:
  * Para sobrescrever Salesforce classic, só com SF classic
  * Para sobrescrever Lightning Experience e Mobile, pode ser SF classic ou um component lightning