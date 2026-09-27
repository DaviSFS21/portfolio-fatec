# Portfólio das APIs — Davi Soares Fernandes dos Santos

**Legenda dos níveis técnicos**

| Nível | Descrição |
|:-|:-|
| Sei fazer com ajuda | Uso prático em entregas reais, com apoio de colega ou documentação em pontos-chave. |
| Sei fazer com autonomia | Implemento, decido e corrijo sozinho, incluindo depuração e ajuste de arquitetura. |

---

## 1º Semestre • 1/2024 • Calculadora Científica

![VisualG](https://img.shields.io/badge/VisualG_3.0-6E4B9E?style=flat) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white) ![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=nodedotjs&logoColor=white) ![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)

O parceiro deste semestre foi a própria Faculdade de Tecnologia de São José dos Campos – Prof. Jessen Vidal, por meio do CADI (Centro de Aprendizagem em Desenvolvimento e Integração), atuando como cliente interno.

A demanda era uma calculadora científica capaz de resolver operações básicas e complexas que apareciam em rotinas contábeis do dia a dia, hoje resolvidas em ferramentas separadas ou à mão. O desafio real do semestre, porém, era anterior ao produto: era a primeira vez que a turma organizava trabalho em equipe sob o modelo de API, com sprints, backlog e entrega periódica.

A solução foi construída em duas etapas deliberadas. Primeiro em VisualG (Portugol), para que o grupo fechasse a lógica de cada operação antes de discutir sintaxe. Depois em TypeScript, na versão funcional, com menu de navegação, conversão entre bases numéricas, cálculos financeiros e equação do segundo grau.

**Repositório:** [SQLutions-FATEC/API-1-Semestre](https://github.com/SQLutions-FATEC/API-1-Semestre)

**Meu papel:** Desenvolvedor

### Tecnologias utilizadas

- **VisualG 3.0 (Portugol)** — permitiu validar a lógica das operações com o grupo inteiro, incluindo quem ainda não programava, antes de qualquer decisão de linguagem. Foi o que manteve a discussão em cima do algoritmo e não da ferramenta.
- **TypeScript** — escolhido justamente pela tipagem estática. Em JavaScript ou Python, nada nos obrigaria a definir a estrutura do dado que entrava em cada operação; a tipagem forçou esse pensamento desde o primeiro módulo e reduziu erro de conversão silencioso nos cálculos.
- **Node.js com `ts-node`** — ambiente de execução que permitia rodar o TypeScript direto, sem etapa de build, mantendo o ciclo de teste curto para um time que estava aprendendo a linguagem.
- **Git e GitHub** — versionamento e organização das tarefas em backlog, primeira experiência do grupo com histórico de código compartilhado.

### Contribuições pessoais

- **Configuração do projeto e commit inicial.** Assumi a preparação do ambiente: `package.json` com `typescript` e `ts-node`, `.gitignore` e a estrutura de pastas que o restante do time passou a usar. Fiz isso porque havia colegas mais experientes no grupo e ninguém tomou a frente; era uma tarefa que travava todo mundo até alguém fazer.
- **Conversão de bases numéricas.** Escrevi o módulo `conversaoDeBase.ts` com as conversões entre binário, octal, decimal e hexadecimal, nas duas versões do projeto, incluindo validação de entrada e tratamento de erro para valores inválidos em cada base. Foi o módulo que mais exigia lógica pura e me candidatei a ele por isso, mesmo sem dominar a linguagem ainda.
- **Menu e controle de fluxo.** Implementei `menu.ts` e `index.ts`, com os laços de repetição, estruturas de decisão e o encadeamento entre as operações. É o arquivo que amarra a aplicação e por onde todo módulo dos colegas passava para ser acessado.
- **Cálculos financeiros, equação do 2º grau e refatoração.** Desenvolvi o módulo de juros simples e compostos em `juros.ts`, unificando operações que estavam espalhadas em arquivos separados, e o cálculo de segundo grau com tratamento do discriminante. Também padronizei nomes e corrigi bugs de interface ao longo das sprints.

### Hard Skills

| Habilidade | Nível alcançado |
|:-|:-|
| Lógica de programação (VisualG) | Sei fazer com autonomia |
| TypeScript | Sei fazer com ajuda |
| Modularização de código | Sei fazer com autonomia |
| Git e GitHub | Sei fazer com autonomia |
| Tratamento e validação de entrada | Sei fazer com autonomia |

### Soft Skills

- **Absorção de trabalho alheio no lugar do confronto — ~~Responsabilidade (Executing).~~** O grupo tinha dez pessoas e parte delas estava concentrada em emprego ou em outras disciplinas, deixando tarefas paradas perto do fim da sprint. Diante disso eu entregava pela pessoa em vez de levar a ausência ao grupo ou ao professor. A entrega do semestre saiu, mas o problema não foi tratado, só reabsorvido — e voltou nos dois semestres seguintes com o mesmo formato. Hoje eu sei que essa não era generosidade, era falta de disposição para uma conversa difícil aos 18 anos.
- **Iniciativa técnica em terreno desconhecido — Estudioso (Strategic Thinking).** Eu havia acabado de sair do ensino médio e escolhi deliberadamente entrar como desenvolvedor, e não em papel de gestão, para aprender ao lado de colegas mais experientes. Ainda assim, quando apareceu o módulo de conversão de bases, que era o mais exigente em lógica, me candidatei antes de saber se daria conta. A lógica que eu trazia do técnico em informática cobriu a parte algorítmica e o TypeScript eu aprendi durante a implementação.
- **Disciplina de organização desde o início — Disciplina (Executing).** Adotei mensagens de commit descritivas (`feat`, `fix`, `refactor`) e insisti em padronização de código já no primeiro semestre, o que tornou o histórico rastreável quando precisamos achar a origem de um bug. A unificação do `juros.ts` foi um caso concreto disso: reorganizei arquivos que já existiam para reduzir duplicação.

> Este semestre é a linha de base da minha trajetória: o Davi que preferiu ficar no papel técnico para observar, que não sabia o que esperar de um projeto em equipe e que resolvia a falta de comprometimento dos outros trabalhando mais. Os semestres seguintes são, em boa parte, a correção desses três pontos.

---

## 2º Semestre • 2/2024 • Avaliador de Soft Skill

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white) ![JavaFX](https://img.shields.io/badge/JavaFX-5382A1?style=flat&logo=java&logoColor=white) ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=mysql&logoColor=white) ![JDBC](https://img.shields.io/badge/JDBC-F80000?style=flat&logo=oracle&logoColor=white)

O parceiro foi novamente a Fatec São José dos Campos por meio do CADI, com os professores das disciplinas P2 e M2 no papel de cliente.

O cliente precisava aplicar a avaliação PACER (Proatividade, Autonomia, Colaboração e Entrega de Resultados) entre alunos da mesma equipe. As avaliações vinham sendo feitas em formatos variados, sem cálculo automático de médias, o que consumia tempo excessivo do professor e dificultava comparar resultados entre sprints e entre turmas.

A solução foi uma aplicação desktop em Java com JavaFX que padronizou o fluxo de avaliação, automatizou o cálculo das médias e deu ao professor o controle de equipes, sprints e critérios, com exportação dos resultados em CSV.

**Repositório:** [SQLutions-FATEC/API-2-Semestre](https://github.com/SQLutions-FATEC/API-2-Semestre)

**Meu papel:** Product Owner

### Tecnologias utilizadas

- **Java** — linguagem exigida pelas disciplinas do semestre e um salto de robustez em relação ao TypeScript do primeiro. Eu já vinha estudando Java por conta, antecipando esse salto, e isso definiu o quanto eu conseguiria apoiar o time tecnicamente.
- **JavaFX** — viabilizou uma aplicação desktop que o professor rodava na própria máquina, sem servidor nem instalação de dependência de rede, o que era o cenário real de uso durante a aula.
- **MySQL** — armazenava equipes, sprints, critérios e notas. A modelagem precisava sustentar o cálculo de média por aluno, por critério e por sprint, que era o coração do produto.
- **JDBC** — conexão direta com o banco, sem ORM. Exigiu escrever e revisar as consultas na mão, o que na prática me deu leitura do custo de cada tela que eu especificava como PO.
- **GitHub com branch por sprint** — organizou a entrega em ciclos fechados e tornou possível revisar código por sprint em vez de acumular tudo no fim.

### Contribuições pessoais

- **Requisitos e backlog junto ao cliente.** Conduzi as sessões de dúvidas com os professores a cada sprint e documentei as respostas no repositório, incluindo regras de negócio como o professor definir o limite de pontos por grupo e a avaliação abrir após o fim da sprint com uma semana para conclusão. Escrevi as User Stories com DoR separado por camada — componentes de tela, endpoints e tabelas envolvidas — e defini o DoD de cada sprint.
- **Atuação técnica além do papel de PO.** Fiz boa parte da infraestrutura do backend, implementei o controle de pontuação do aluno com label em tempo real e mudança de cor do botão ao atingir o limite, corrigi a exportação de CSV (conversão de float para int na nota e ajuste do path de download), criei o alerta de confirmação de exclusão de aluno e as seeds do banco. Era o time que mais precisava de apoio técnico e eu era quem tinha mais afinidade com Java. *Hoje leio isso como desvio de função, não como mérito.*
- **Revisão e merge de aproximadamente 15 Pull Requests.** Assumi o papel de revisor do time, o que na prática me deu controle de qualidade do que entrava na main e visibilidade de quem estava produzindo.
- **Manual de usuário.** Foi a primeira vez que o grupo produziu documentação voltada a quem ia usar o sistema, e não a quem ia desenvolvê-lo. Escrevê-lo me obrigou a percorrer o produto inteiro pela ótica do professor.

### Hard Skills

| Habilidade | Nível alcançado |
|:-|:-|
| Java | Sei fazer com autonomia |
| JavaFX | Sei fazer com ajuda |
| MySQL | Sei fazer com autonomia |
| JDBC | Sei fazer com autonomia |
| Escrita de User Stories com DoR e DoD | Sei fazer com autonomia |
| Priorização de backlog | Sei fazer com ajuda |
| Documentação para usuário final | Sei fazer com autonomia |

### Soft Skills

- **O custo de decidir por afinidade — ~~Harmonia (Relationship Building).~~** O integrante com mais experiência em backend passou a descumprir os critérios de permanência da equipe, faltando a reuniões e não entregando o que assumia. Eu insisti em mantê-lo, por afinidade pessoal, e o grupo passou por cima do próprio critério. O resultado foi previsível: *a ausência dele recaiu sobre quem estava presente, e fui eu que assumi a lacuna técnica no backend* — a mesma atuação que hoje considero desvio do meu papel. O problema não foi resolvido neste semestre; ficou pendente até a API seguinte.
- **Aprender um papel sem saber por onde começar — Input (Strategic Thinking).** Assumi como PO sem referência prática do que o papel exigia e passei as primeiras sprints perdido, sem saber se meu trabalho era documentar, priorizar, cobrar ou programar. O que me tirou disso foi o cliente ser um professor da Fatec, disponível e didático, que respondia dúvida no mesmo dia. Documentar cada resposta no repositório virou meu método de reduzir ambiguidade, e é o hábito que sustentou meu trabalho de produto nos semestres seguintes.
- **Autocrítica sobre delimitação de papel — ~~Foco (Executing).~~** Terminei o semestre com uma entrega sólida em requisitos, backlog e manual, e ao mesmo tempo com a percepção de que boa parte da minha energia foi para código que não era minha responsabilidade. Reconhecer isso foi mais útil do que o resultado da entrega: a proatividade que funcionou no primeiro semestre, aplicada no papel de PO, virou acúmulo de função e enfraqueceu meu trabalho de produto.

---

## 3º Semestre • 1/2025 • Sistema de Ponto e Geração de Relatórios

![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat&logo=springboot&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white) ![Vue.js](https://img.shields.io/badge/Vue.js-4FC08D?style=flat&logo=vuedotjs&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white) ![Swagger](https://img.shields.io/badge/Swagger-85EA2D?style=flat&logo=swagger&logoColor=black)

O parceiro foi a [Altave](https://altave.com.br/), empresa de monitoramento e inspeção com uso de aeróstatos e visão computacional. Foi o primeiro cliente externo real da minha trajetória, com Celso Reis atuando como cliente do lado da empresa.

Navios têm custo alto de manutenção e o reparo é frequentemente feito por empresa terceirizada. O proprietário precisa acompanhar a presença e a jornada dos funcionários dessa terceirizada para não absorver prejuízo por atraso, e esse controle não existia de forma auditável. A Altave pediu um sistema de ponto que registrasse as movimentações, apresentasse indicadores e gerasse relatórios.

A solução foi um sistema web com backend em Spring Boot, frontend em Vue.js e PostgreSQL, com dashboards de movimentação, controle de contratos e exportação de relatórios, empacotado para rodar via Docker Compose.

**Repositório:** [SQLutions-FATEC/API-3-Semestre](https://github.com/SQLutions-FATEC/API-3-Semestre)

**Meu papel:** Product Owner

### Tecnologias utilizadas

- **Spring Boot** — estruturou a API REST em camadas e permitiu que o time trabalhasse em controllers e services separados sem colisão. ***Eu já vinha estudando Spring por fora, o que me colocou como referência técnica do time nesta stack.***
- **PostgreSQL** — sustentou o modelo de empresas, funcionários, contratos e movimentações, incluindo as consultas agregadas dos dashboards e o soft delete que preservava histórico de quem saía.
- **Vue.js** — frontend das telas de cadastro, filtro e dashboard, consumindo a API. Foi a camada em que atuei menos e onde declaro dependência de apoio.
- **Docker e Docker Compose** — foi decisão de produto, não conveniência de desenvolvimento: o cliente precisava rodar o sistema sozinho para validar, e um `docker-compose up -d` subia o banco configurado sem que ele instalasse PostgreSQL na máquina.
- **Swagger / OpenAPI** — deu ao cliente e aos professores uma forma de validar os endpoints direto no navegador, sem Postman e sem depender de nós.
- **JPA / Hibernate e Lombok** — reduziram o código repetitivo de acesso a dados e de DTOs, o que importava num semestre em que eu dividia meu tempo entre produto e backend.
- **Jira** — backlog, acompanhamento de sprint e burndown, que era também o material de prestação de contas ao cliente.

### Contribuições pessoais

- **Negociação de requisitos com cliente externo.** Documentei as oito User Stories do projeto com DoR, DoD e critérios de aceite, incluindo regras específicas como validação de datas de contrato, máscara de CNPJ, filtros de movimentação por empresa, funcionário e data, e regras de exportação. Diferente do semestre anterior, o cliente tinha agenda própria e tempo de resposta longo, o que exigiu renegociar escopo e prazo de entrega mais de uma vez ao longo das sprints.
- **Decisões técnicas tomadas em função da validação pelo cliente.** Configurei o Spring com `spring.sql.init.mode=always` e `ddl-auto=create-drop` para que 228 linhas de dados realistas de empresas, funcionários, contratos e movimentações fossem carregadas a cada inicialização. O cliente abria o sistema e já tinha o que validar. A entrega final foi empacotada como `.jar` do backend, `dist` do frontend e `compose.yaml` em uma pasta única, com instalação em três comandos.
- **Desenvolvimento do backend.** Construí a estrutura de controllers, services com interface e implementação, repositories, DTOs e entities, e os CRUDs de Movimentações, Empresas e Funcionários. Desenvolvi o módulo de Analytics com as consultas de registros diários, horas por cargo, contratos a expirar, clock-ins incompletos e funcionários por turno, além do soft delete com filtro nas queries.

### Hard Skills

| Habilidade | Nível alcançado |
|:-|:-|
| Spring Boot | Sei fazer com autonomia |
| PostgreSQL | Sei fazer com autonomia |
| Docker / Docker Compose | Sei fazer com autonomia |
| JPA / Hibernate | Sei fazer com autonomia |
| Swagger / OpenAPI | Sei fazer com autonomia |
| Vue.js | Sei fazer com ajuda |
| Escrita de documentação técnica | Sei fazer com autonomia |
| Gestão de produto e negociação de requisitos | Sei fazer com autonomia |

### Soft Skills

- **Gestão de consequência — Restauração (Executing).** O integrante que vinha descumprindo os critérios de permanência desde o segundo semestre continuou no grupo, agora com o desgaste visível na equipe. ***Fui eu, com dois colegas, que levei a decisão de aplicar o critério e desligá-lo***, num grupo de nove pessoas em que a maioria era passiva e não colocava posição na mesa. Foram cerca de dez meses entre o primeiro sintoma e a decisão. Aprendi que critério que não se aplica não é critério, e que como PO a responsabilidade de puxar essa conversa era minha, não do professor nem do grupo.
- **Escuta de requisito sem preencher lacuna com interpretação própria — Prudência (Executing).** Com um cliente real, percebi que eu completava as informações que faltavam com o meu próprio entendimento do negócio em vez de voltar e perguntar, o que gerou retrabalho em pontos de regra de negócio. ***O trabalho de produto foi elogiado pelo cliente ao fim do semestre,*** *mas hoje eu faria diferente: desconstruiria a fala dele, daria alguns passos atrás para entender os conceitos nos termos dele e validaria mais com o professor orientador antes de transformar conversa em User Story.*
- **Gestão de dependência externa — Adaptabilidade (Relationship Building).** O tempo de resposta do cliente foi a maior fonte de atrito do semestre e travou decisões que eu não podia tomar sozinho. Foi frustrante, e foi também a experiência mais próxima de mercado que tive até aqui: ***aprendi a manter frentes paralelas andando enquanto uma resposta não chegava, e a registrar por escrito o que estava bloqueado e desde quando.***

---

## 4º Semestre • 2/2025 • Radarius — Monitoramento Inteligente de Tráfego

![Spring Boot](https://img.shields.io/badge/Spring_Boot_3-6DB33F?style=flat&logo=springboot&logoColor=white) ![Oracle](https://img.shields.io/badge/Oracle_Database-F80000?style=flat&logo=oracle&logoColor=white) ![Vue.js](https://img.shields.io/badge/Vue.js_3-4FC08D?style=flat&logo=vuedotjs&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white) ![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat&logo=nginx&logoColor=white) ![JWT](https://img.shields.io/badge/JWT-000000?style=flat&logo=jsonwebtokens&logoColor=white)

O parceiro foi a [Prefeitura de São José dos Campos](https://www.sjc.sp.gov.br/), por meio da área de mobilidade urbana.

A cidade tinha dados de radares, mas não tinha um sistema que os transformasse em decisão. Não havia como definir indicadores com níveis de severidade, disparar alerta quando um limiar fosse ultrapassado nem alocar agentes de mobilidade com base no que estava acontecendo na via.

A solução foi o Radarius, com dashboard interativo, mapa zonal, alertas automáticos e controle de acesso por perfil de usuário. Backend em Spring Boot 3 com Oracle Database, frontend em Vue.js 3 com Vite e deploy completo em Docker com Nginx.

**Repositório:** [DenariusData/API-4SEM](https://github.com/DenariusData/API-4SEM)

**Meu papel:** Desenvolvedor

### Tecnologias utilizadas

- **Spring Boot 3** — base da API REST e do agendamento interno de verificação de indicadores. A versão 3 exigiu adequação de configuração em relação ao que eu conhecia do semestre anterior.
- **Oracle Database com autenticação por Wallet** — requisito do semestre e a primeira vez que subi um banco acessado remotamente por todo o time. O Wallet exigiu tratar credencial como volume no container, não como variável solta.
- **Vue.js 3 com Vite** — frontend do dashboard e do mapa, com build otimizado para servir em produção.
- **Spring Security com JWT** — sustentou o controle de acesso por perfil, que era pré-requisito de praticamente toda tela do sistema: gestor, agente e administrador veem coisas diferentes.
- **Docker, Docker Compose e Nginx** — containerização das três pontas com health checks, rede isolada e proxy reverso do frontend para a API, o que permitiu subir o sistema inteiro em qualquer máquina do time com a mesma configuração.
- **GitHub Actions** — automação da descrição de Pull Requests, para reduzir o custo do code review obrigatório que estabelecemos.

### Contribuições pessoais

- **Camada de segurança completa.** Implementei a autenticação com JWT de ponta a ponta — `JwtIssuer`, `JwtAuthenticationFilter`, `TokenDecoder` e `JwtToPrincipalConverter` — mais a configuração do Spring Security em `WebSecurityConfig`, o `AuthController` com login e o `CustomUserDetailService` para integração com o banco. Também protegi os endpoints garantindo que a lógica por ROLE funcionasse em cada rota. Era o módulo que desbloqueava o trabalho dos outros e por isso foi o primeiro a ser entregue.
- **Ciclo de alerta e monitoramento.** Auxiliei no `LevelScheduler`, que verifica mudança de nível nos indicadores de tráfego e dispara alerta ao ultrapassar o limiar, e implementei o ciclo completo do alerta: criação automática, registro em `AlertLog`, associação com causa raiz e protocolo, filtragem por região do usuário e endpoint de finalização. Criei também o CRUD de protocolos e causas raiz, que é o que permite ao gestor orientar o agente em campo.
- **Banco em nuvem e infraestrutura.** Subi o Oracle Database acessado por todo o time, com configuração de Wallet, migrando o projeto do PostgreSQL. A migração quebrou a estratégia de geração de ID, que passou a `SEQUENCE`, e exigiu renomear entidades (`User` → `Person`, `Zone` → `Region`) e remover relações que só existiam por conveniência do Postgres. Escrevi o `Dockerfile` do backend com Zulu OpenJDK 21, o do frontend com Node 20 e Nginx, e o `docker-compose.yml` com health check em `/actuator/health`, rede bridge isolada, volume para o Wallet e política de restart.
- **Processo de engenharia.** Defini o padrão de Conventional Commits, a estrutura de branches com prazo (domingo às 19h para features e 23h para a main) e o code review obrigatório com responsabilidade compartilhada entre autor e revisor. Foi a experiência de PO dos dois semestres anteriores aplicada a partir de uma cadeira de desenvolvedor.

### Hard Skills

| Habilidade | Nível alcançado |
|:-|:-|
| Spring Boot 3 | Sei fazer com autonomia |
| Spring Security e JWT | Sei fazer com autonomia |
| Oracle Database | Sei fazer com autonomia |
| Docker / Docker Compose | Sei fazer com autonomia |
| Modelagem de banco de dados | Sei fazer com autonomia |
| Vue.js 3 | Sei fazer com ajuda |
| Nginx e proxy reverso | Sei fazer com ajuda |
| CI/CD com GitHub Actions | Sei fazer com ajuda |

### Soft Skills

- **Autoridade sem mandato — ~~Comando (Influencing).~~** Eu, Tiago Reis e Augusto Piatto saímos do grupo de nove pessoas do semestre anterior justamente pela morosidade da equipe, e entramos num grupo menor. O perfil do problema mudou de forma: no lugar de gente parada, encontramos gente que propunha muita ideia e entregava pouco. Como éramos três recém-chegados, nos sentimos acuados para impor ordem, mesmo eu tendo aprendido no semestre anterior a aplicar critério de permanência. Faltou coragem, e o resultado foi que os módulos críticos do sistema ficaram concentrados em nós três. Aprendi que a decisão de trocar de ambiente resolve menos do que parece se as regras de convivência não forem pactuadas na entrada.
- **Adaptabilidade sob requisito imposto — Adaptabilidade (Relationship Building).** A troca de PostgreSQL para Oracle veio como requisito do semestre com o backend já em funcionamento, e não foi uma troca de driver: quebrou a geração de ID, exigiu Wallet no container e me obrigou a renomear entidades e remover relações da modelagem. Conduzi a migração sem parar o cronograma do time.
- **Contrapeso técnico às ideias do grupo — Analítico (Strategic Thinking).** Com Augusto atuando como PO, eu servia como uma segunda cabeça pensando do lado do código: quando os colegas mais "sonhadores" da equipe cogitavam prometer ao cliente mais do que a stack ou o prazo permitiam, era eu quem questionava a viabilidade técnica antes que a ideia virasse compromisso. Esse contrapeso, somado a definir o padrão de commit, o prazo de branch e o code review obrigatório, foi a forma que encontrei de dar previsibilidade a uma equipe em que eu não tinha autoridade formal para cobrar ninguém. Foi a primeira vez que usei análise técnica e processo como substituto de autoridade, e funcionou melhor do que a cobrança direta que eu não me sentia à vontade para fazer.

---

## 5º Semestre • 1/2026 • Lunae — Data Warehouse Corporativo

O parceiro foi a **SIATT**, empresa do setor de defesa. Por lidar com dados sensíveis, a empresa exigia que a aplicação rodasse inteiramente on-premise, sem que o dashboard ou seus dados transitassem pela internet.

A SIATT não tinha uma fonte única de verdade: informações de diferentes departamentos viviam espalhadas, sem um modelo comum que permitisse cruzar dados entre áreas. A demanda era um data warehouse que centralizasse essas informações e servisse de base analítica para toda a empresa.

A solução foi o **Lunae**, um data warehouse com backend em Django e frontend em Vue.js/TypeScript, modelado em star schema sobre PostgreSQL. Como o deploy não podia depender de internet nem de acesso remoto contínuo da equipe, a entrega incluiu uma imagem de VM pronta para ativação, provisionada via Packer e configurada automaticamente no primeiro boot via cloud-init.

**Repositório:** [23deFevereiro/FATEC-API-5-Semestre](https://github.com/23deFevereiro/FATEC-API-5-Semestre)

**Meu papel:** Scrum Master na primeira semana; Desenvolvedor pelo restante do semestre, após o time identificar que a demanda técnica pedia mais força nessa frente.

### Tecnologias utilizadas

- **Django** — não era minha stack mais forte até então (vinha de dois semestres em Spring Boot), mas ainda assim acabei como peça central do desenvolvimento, o que exigiu ritmo de aprendizado acelerado dentro do próprio projeto.
- **PostgreSQL com modelagem em star schema** — organizou os dados em tabelas fato e dimensão para sustentar consultas analíticas entre departamentos, em vez de um modelo puramente transacional.
- **Packer com builder QEMU/KVM** — construiu uma imagem de disco `.vmdk` reprodutível a partir do Ubuntu 24.04 cloud image, eliminando a necessidade de instalação manual em cada ativação.
- **Cloud-init (datasource NoCloud)** — configurou rede, banco e variáveis de ambiente da aplicação automaticamente no primeiro boot da VM, via seed ISO entregue ao time de TI do cliente.
- **NestJS, React/TypeScript e PostgreSQL (Scrum Warden)** — sistema próprio que construí para automatizar a contabilização dos critérios de permanência da equipe.

### Contribuições pessoais

- **Modelagem do data warehouse.** Construí o star schema do projeto, organizando os dados da SIATT em tabelas fato e dimensão para sustentar o papel do Lunae como fonte única de verdade entre departamentos.
- **Pipeline de deploy on-premise.** Defini e implementei a estratégia de entrega via imagem de VM: montei o build Packer com QEMU/KVM gerando um `.vmdk` a partir do Ubuntu 24.04, e configurei o cloud-init para que o time de TI da SIATT apenas ativasse a VM e a integrasse à rede interna, sem depender de mim para instalação.
- **Scrum Warden.** Ainda na semana como Scrum Master, formalizei os critérios de permanência da equipe em documento (sistema de pontos por sprint, limites e consequências) e construí uma aplicação própria — NestJS, React com TypeScript e PostgreSQL, containerizada com Docker — para contabilizar essas regras automaticamente, em vez de depender de planilha manual.

### Hard Skills

| Habilidade | Nível alcançado |
|:-|:-|
| Django | Sei fazer com ajuda |
| Modelagem dimensional (star schema) | Sei fazer com ajuda |
| Packer e provisionamento de imagens | Sei fazer com autonomia |
| Cloud-init | Sei fazer com autonomia |
| NestJS | Sei fazer com autonomia |

### Soft Skills

- **Equipe com critério pactuado na entrada — Comando (Influencing).** Eu, Tiago Reis e Augusto Piatto entramos no semestre já com critérios de permanência sérios definidos, corrigindo o que faltou no 4º semestre: pactuar regra de convivência desde o início, não depois que o problema aparece. Foi um alívio real ter uma equipe que de fato funcionava nesse aspecto — mesmo que, tecnicamente, o grupo não tenha sido tão eficiente, porque outras questões tomaram boa parte da nossa atenção.
- **Demora em validar decisão técnica — ~~Prudência (Executing).~~** Levei tempo demais para validar a estratégia de deploy on-premise com o professor orientador, o que só piorou a situação — eu vinha de uma concepção limitada, habituado a deploy em VMs de nuvem, e isso tornou o problema mais difícil do que precisava ser. Hoje eu teria buscado validação bem mais cedo.

---

## Fio condutor dos cinco primeiros semestres

O mesmo problema atravessa os quatro primeiros: como lidar com falta de comprometimento em equipe acadêmica. No 1º semestre eu entregava pela pessoa. No 2º, insisti em manter no grupo, por afinidade, justamente quem estava ausente — e absorvi o vácuo técnico dela. No 3º, apliquei o critério de permanência e conduzi o desligamento, dez meses depois do primeiro sintoma. No 4º, mudei de ambiente e descobri que trocar de grupo não substitui pactuar regra na entrada. No 5º, esse arco finalmente se fecha: eu, Tiago Reis e Augusto Piatto entramos com critério de permanência pactuado desde o primeiro dia, não mais construído em resposta a um problema já instalado.

No eixo técnico o caminho é inverso e mais linear: comecei em lógica e módulos isolados, passei por dois semestres em que a técnica veio como desvio de função, e voltei ao papel de desenvolvedor com a camada de segurança, o banco em nuvem e a infraestrutura do time — agora no lugar certo. No 5º semestre esse eixo ganha uma dobra nova: entrei numa stack (Django) e num domínio (deploy on-premise, provisionamento de imagem) onde eu tinha menos base do que em qualquer semestre anterior, e ainda assim acabei como peça central da entrega — o que mostra que a atuação técnica deixou de depender de terreno conhecido.

No eixo dos temas CliftonStrengths, o percurso é o de uma Responsabilidade mal calibrada (1º) que se torna Harmonia usada para evitar conflito (2º), até virar Restauração — a mesma disposição de agir, agora dirigida ao problema certo (3º). Em paralelo, Estudioso e Input mostram uma disciplina de aprendizado que amadurece em Foco, e a Adaptabilidade aparece duas vezes em contextos diferentes (dependência de cliente no 3º, requisito técnico imposto no 4º), sinal de que deixou de ser reação pontual para virar padrão. O Comando que faltava ao fim do 4º semestre finalmente aparece exercido no 5º: eu, Tiago Reis e Augusto Piatto entramos com critério de permanência pactuado desde o início, não mais reconstruído depois do problema instalado. Mas a Prudência segue como tema em aberto — a mesma cautela que faltou ao interpretar requisito no 3º semestre, e que apareceu só de forma indireta como Analítico no 4º, continua ausente no 5º: a demora em validar a estratégia de deploy com o orientador é o mesmo padrão, agora em contexto técnico em vez de contato com cliente. É uma habilidade que só passo a exercer sobre mim mesmo no 6º semestre.