# Portfólio das APIs — Davi Soares Fernandes dos Santos

<img src="https://avatars.githubusercontent.com/u/94925054?v=4" alt="Davi Soares Fernandes dos Santos" width="150" align="right">

## Sobre mim

Estudante de Banco de Dados na Fatec São José dos Campos – Prof. Jessen Vidal e desenvolvedor de software na IACIT, em São José dos Campos, onde me especializo em DevOps e em backend com Spring.

Ao longo da graduação transitei entre desenvolvedor e Product Owner conforme a necessidade de cada projeto, o que me deu uma visão do ciclo inteiro: levantamento de requisitos e priorização de backlog de um lado, arquitetura de API, modelagem de banco e entrega em produção do outro. Os seis projetos integrados a seguir estão organizados nessa chave — o que fiz com as próprias mãos em cada um, o que deu errado e o que eu faria diferente. Todas as reflexões estão escritas do ponto de vista de agora, no encerramento do sexto semestre, e não do que eu pensava ao fim de cada projeto.

Atuo também com projetos freelance. O aprendizado acumulado no período da Fatec é o que me permite hoje conduzir, com confiança e de forma independente, todo o percurso de um projeto: da coleta de requisitos com o cliente ao deploy em uma VM.

• [LinkedIn](https://www.linkedin.com/in/dsf21/) • [GitHub](https://github.com/DaviSFS21) •

---

## Sumário

| Semestre | Projeto | Parceiro | Meu papel |
|:-|:-|:-|:-|
| [1º • 1/2024](#1º-semestre--12024--calculadora-científica) | Calculadora Científica | Fatec SJC (CADI) | Desenvolvedor |
| [2º • 2/2024](#2º-semestre--22024--avaliador-de-soft-skill) | Avaliador de Soft Skill | Fatec SJC (CADI) | Product Owner |
| [3º • 1/2025](#3º-semestre--12025--sistema-de-ponto-e-geração-de-relatórios) | Sistema de Ponto e Relatórios | Altave | Product Owner |
| [4º • 2/2025](#4º-semestre--22025--radarius--monitoramento-inteligente-de-tráfego) | Radarius | Prefeitura de São José dos Campos | Desenvolvedor |
| [5º • 1/2026](#5º-semestre--12026--lunae--data-warehouse-corporativo) | Lunae | SIATT | Desenvolvedor |
| [6º • 2/2026](#6º-semestre--22026--índice--gestão-documental-inteligente) | Índice | Akaer | Desenvolvedor |

---

**Legenda dos níveis técnicos**

| Nível | Descrição |
|:-|:-|
| 🟡 Sei fazer com ajuda | Uso prático em entregas reais, com apoio de colega ou documentação em pontos-chave. |
| 🟢 Sei fazer com autonomia | Implemento, decido e corrijo sozinho, incluindo depuração e ajuste de arquitetura. |

Cada habilidade vem acompanhada do artefato que a sustenta — arquivo, configuração ou documento do repositório do semestre —, de modo que o nível declarado possa ser verificado no código.

---

## 1º Semestre • 1/2024 • Calculadora Científica

![VisualG](https://img.shields.io/badge/VisualG_3.0-6E4B9E?style=flat) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white) ![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=nodedotjs&logoColor=white) ![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)

O parceiro deste semestre foi a própria Faculdade de Tecnologia de São José dos Campos – Prof. Jessen Vidal, por meio do CADI (Centro de Aprendizagem em Desenvolvimento e Integração), atuando como cliente interno.

A demanda era uma calculadora científica capaz de resolver operações básicas e complexas que apareciam em rotinas contábeis do dia a dia, até então resolvidas em ferramentas separadas ou à mão. O desafio real do semestre, porém, era anterior ao produto: era a primeira vez que a turma organizava trabalho em equipe sob o modelo de API, com sprints, backlog e entrega periódica.

A solução foi construída em duas etapas deliberadas. Primeiro em VisualG (Portugol), para que o grupo fechasse a lógica de cada operação antes de discutir sintaxe. Depois em TypeScript, na versão funcional, com menu de navegação, conversão entre bases numéricas, cálculos financeiros e equação do segundo grau.

**Repositório:** [SQLutions-FATEC/API-1-Semestre](https://github.com/SQLutions-FATEC/API-1-Semestre)

### 🛠️ Tecnologias utilizadas

- **VisualG 3.0 (Portugol)** — permitiu validar a lógica das operações com o grupo inteiro, incluindo quem ainda não programava, antes de qualquer decisão de linguagem. Foi o que manteve a discussão em cima do algoritmo e não da ferramenta.
- **TypeScript** — escolhido justamente pela tipagem estática. Em JavaScript ou Python, nada nos obrigaria a definir a estrutura do dado que entrava em cada operação; a tipagem forçou esse pensamento desde o primeiro módulo e reduziu erro de conversão silencioso nos cálculos.
- **Node.js com `ts-node`** — ambiente de execução que permitia rodar o TypeScript direto, sem etapa de build, mantendo o ciclo de teste curto para um time que estava aprendendo a linguagem.
- **Git e GitHub** — versionamento e organização das tarefas em backlog, primeira experiência do grupo com histórico de código compartilhado.

### 👤 Contribuições pessoais

- **Meu papel e a configuração do projeto.** Atuei como desenvolvedor e assumi a preparação do ambiente: `package.json` com `typescript` e `ts-node`, `.gitignore` e a estrutura de pastas que o restante do time passou a usar. Fiz isso porque havia colegas mais experientes no grupo e ninguém tomou a frente; era uma tarefa que travava todo mundo até alguém fazer.
- **Conversão de bases numéricas.** Escrevi o módulo `conversaoDeBase.ts` com as conversões entre binário, octal, decimal e hexadecimal, nas duas versões do projeto, incluindo validação de entrada e tratamento de erro para valores inválidos em cada base. Foi o módulo que mais exigia lógica pura e me candidatei a ele por isso, mesmo sem dominar a linguagem ainda.
- **Menu e controle de fluxo.** Implementei `menu.ts` e `index.ts`, com os laços de repetição, estruturas de decisão e o encadeamento entre as operações. É o arquivo que amarra a aplicação e por onde todo módulo dos colegas passava para ser acessado.
- **Cálculos financeiros, equação do 2º grau e refatoração.** Desenvolvi o módulo de juros simples e compostos em `juros.ts`, unificando operações que estavam espalhadas em arquivos separados, e o cálculo de segundo grau com tratamento do discriminante. Também padronizei nomes e corrigi bugs de interface ao longo das sprints.

### 📊 Hard Skills

| Habilidade | Nível alcançado | Evidência |
|:-|:-|:-|
| Lógica de programação (VisualG) | 🟢 Sei fazer com autonomia | `VisualG/calculadora_cientifica.alg` |
| TypeScript | 🟡 Sei fazer com ajuda | `TypeScript/operacoesLogicas/conversaoDeBase.ts` |
| Modularização de código | 🟢 Sei fazer com autonomia | `TypeScript/menu.ts` e `index.ts` encadeando `operacoesLogicas/` |
| Git e GitHub | 🟢 Sei fazer com autonomia | Histórico e backlog do repositório do semestre |
| Tratamento e validação de entrada | 🟢 Sei fazer com autonomia | Validação por base em `conversaoDeBase.ts`; discriminante em `funcaoSegundoGrau.ts` |

### 🧠 Soft Skills

- **Absorção de trabalho alheio no lugar do confronto.** O grupo tinha dez pessoas e parte delas estava concentrada em emprego ou em outras disciplinas, deixando tarefas paradas perto do fim da sprint. Diante disso eu entregava pela pessoa em vez de levar a ausência ao grupo ou ao professor. A entrega do semestre saiu, mas o problema não foi tratado, só reabsorvido — e voltou nos dois semestres seguintes com o mesmo formato. Hoje, olhando do sexto semestre, sei que essa não era generosidade, era falta de disposição para uma conversa difícil aos 18 anos.
- **Iniciativa técnica em terreno desconhecido.** Eu havia acabado de sair do ensino médio e escolhi deliberadamente entrar como desenvolvedor, e não em papel de gestão, para aprender ao lado de colegas mais experientes. Ainda assim, quando apareceu o módulo de conversão de bases, que era o mais exigente em lógica, me candidatei antes de saber se daria conta. A lógica que eu trazia do técnico em informática cobriu a parte algorítmica e o TypeScript eu aprendi durante a implementação.
- **Disciplina de organização desde o início.** Adotei mensagens de commit descritivas (`feat`, `fix`, `refactor`) e insisti em padronização de código já no primeiro semestre, o que tornou o histórico rastreável quando precisamos achar a origem de um bug. A unificação do `juros.ts` foi um caso concreto disso: reorganizei arquivos que já existiam para reduzir duplicação.

> Este semestre é a linha de base da minha trajetória: o Davi que preferiu ficar no papel técnico para observar, que não sabia o que esperar de um projeto em equipe e que resolvia a falta de comprometimento dos outros trabalhando mais. Os semestres seguintes são, em boa parte, a correção desses três pontos.

---

## 2º Semestre • 2/2024 • Avaliador de Soft Skill

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white) ![JavaFX](https://img.shields.io/badge/JavaFX-5382A1?style=flat&logo=java&logoColor=white) ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=mysql&logoColor=white) ![JDBC](https://img.shields.io/badge/JDBC-F80000?style=flat&logo=oracle&logoColor=white)

O parceiro foi novamente a Fatec São José dos Campos por meio do CADI, com os professores das disciplinas P2 e M2 no papel de cliente.

O cliente precisava aplicar a avaliação PACER (Proatividade, Autonomia, Colaboração e Entrega de Resultados) entre alunos da mesma equipe. As avaliações vinham sendo feitas em formatos variados, sem cálculo automático de médias, o que consumia tempo excessivo do professor e dificultava comparar resultados entre sprints e entre turmas.

A solução foi uma aplicação desktop em Java com JavaFX que padronizou o fluxo de avaliação, automatizou o cálculo das médias e deu ao professor o controle de equipes, sprints e critérios, com exportação dos resultados em CSV.

**Repositório:** [SQLutions-FATEC/API-2-Semestre](https://github.com/SQLutions-FATEC/API-2-Semestre)

### 🛠️ Tecnologias utilizadas

- **Java** — linguagem exigida pelas disciplinas do semestre e um salto de robustez em relação ao TypeScript do primeiro. Eu já vinha estudando Java por conta, antecipando esse salto, e isso definiu o quanto eu conseguiria apoiar o time tecnicamente.
- **JavaFX** — viabilizou uma aplicação desktop que o professor rodava na própria máquina, sem servidor nem instalação de dependência de rede, o que era o cenário real de uso durante a aula.
- **MySQL** — armazenava equipes, sprints, critérios e notas. A modelagem precisava sustentar o cálculo de média por aluno, por critério e por sprint, que era o coração do produto.
- **JDBC** — conexão direta com o banco, sem ORM. Exigiu escrever e revisar as consultas na mão, o que na prática me deu leitura do custo de cada tela que eu especificava como PO.
- **GitHub com branch por sprint** — organizou a entrega em ciclos fechados e tornou possível revisar código por sprint em vez de acumular tudo no fim.

### 👤 Contribuições pessoais

- **Meu papel, requisitos e backlog junto ao cliente.** Atuei como Product Owner. Conduzi as sessões de dúvidas com os professores a cada sprint e documentei as respostas no repositório, incluindo regras de negócio como o professor definir o limite de pontos por grupo e a avaliação abrir após o fim da sprint com uma semana para conclusão. Escrevi as User Stories com DoR separado por camada — componentes de tela, endpoints e tabelas envolvidas — e defini o DoD de cada sprint.
- **Atuação técnica além do papel de PO.** Fiz boa parte da infraestrutura do backend, implementei o controle de pontuação do aluno com label em tempo real e mudança de cor do botão ao atingir o limite, corrigi a exportação de CSV (conversão de float para int na nota e ajuste do path de download), criei o alerta de confirmação de exclusão de aluno e as seeds do banco. Era o time que mais precisava de apoio técnico e eu era quem tinha mais afinidade com Java. Olhando do sexto semestre, leio isso como desvio de função, não como mérito.
- **Revisão e merge de aproximadamente 15 Pull Requests.** Assumi o papel de revisor do time, o que na prática me deu controle de qualidade do que entrava na main e visibilidade de quem estava produzindo.
- **Manual de usuário.** Foi a primeira vez que o grupo produziu documentação voltada a quem ia usar o sistema, e não a quem ia desenvolvê-lo. Escrevê-lo me obrigou a percorrer o produto inteiro pela ótica do professor.

### 📊 Hard Skills

| Habilidade | Nível alcançado | Evidência |
|:-|:-|:-|
| Java | 🟢 Sei fazer com autonomia | `src/main/java/app/` — controllers, DAOs e models |
| JavaFX | 🟡 Sei fazer com ajuda | `app/controllers/SetScoreController.java` |
| MySQL | 🟢 Sei fazer com autonomia | `src/main/resources/assets/sql/schema.sql` e `default_dump.sql` (seeds) |
| JDBC | 🟢 Sei fazer com autonomia | `app/helpers/DatabaseConnection.java` e as classes de `app/DAOs/` |
| Escrita de User Stories com DoR e DoD | 🟢 Sei fazer com autonomia | Documentação de requisitos em `docs/` |
| Priorização de backlog | 🟡 Sei fazer com ajuda | Backlog por sprint no repositório |
| Documentação para usuário final | 🟢 Sei fazer com autonomia | `docs/guide/README.md` |

### 🧠 Soft Skills

- **O custo de decidir por afinidade.** O integrante com mais experiência em backend passou a descumprir os critérios de permanência da equipe, faltando a reuniões e não entregando o que assumia. Eu insisti em mantê-lo, por afinidade pessoal, e o grupo passou por cima do próprio critério. O resultado foi previsível: a ausência dele recaiu sobre quem estava presente, e fui eu que assumi a lacuna técnica no backend — a mesma atuação que, olhando do sexto semestre, considero desvio do meu papel. O problema não foi resolvido neste semestre; ficou pendente até a API seguinte.
- **Aprender um papel sem saber por onde começar.** Assumi como PO sem referência prática do que o papel exigia e passei as primeiras sprints perdido, sem saber se meu trabalho era documentar, priorizar, cobrar ou programar. O que me tirou disso foi o cliente ser um professor da Fatec, disponível e didático, que respondia dúvida no mesmo dia. Documentar cada resposta no repositório virou meu método de reduzir ambiguidade, e é o hábito que sustentou meu trabalho de produto nos semestres seguintes.
- **Autocrítica sobre delimitação de papel.** Terminei o semestre com uma entrega sólida em requisitos, backlog e manual, e ao mesmo tempo com a percepção de que boa parte da minha energia foi para código que não era minha responsabilidade. Reconhecer isso foi mais útil do que o resultado da entrega: a proatividade que funcionou no primeiro semestre, aplicada no papel de PO, virou acúmulo de função e enfraqueceu meu trabalho de produto. O que ficou de fora foi justamente o núcleo do papel: aprofundar as regras de negócio e explorar o cliente. Era o cliente mais acessível que eu teria em toda a graduação — um professor da própria Fatec, que respondia no mesmo dia — e eu não aproveitei esse acesso porque estava ocupado com o backend. Olhando do sexto semestre, essa é a troca que mais me incomoda neste projeto.

---

## 3º Semestre • 1/2025 • Sistema de Ponto e Geração de Relatórios

![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat&logo=springboot&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white) ![Vue.js](https://img.shields.io/badge/Vue.js-4FC08D?style=flat&logo=vuedotjs&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white) ![Swagger](https://img.shields.io/badge/Swagger-85EA2D?style=flat&logo=swagger&logoColor=black)

O parceiro foi a [Altave](https://altave.com.br/), empresa de monitoramento e inspeção com uso de aeróstatos e visão computacional. Foi o primeiro cliente externo real da minha trajetória, com um representante da própria Altave atuando como cliente.

Navios têm custo alto de manutenção e o reparo é frequentemente feito por empresa terceirizada. O proprietário precisa acompanhar a presença e a jornada dos funcionários dessa terceirizada para não absorver prejuízo por atraso, e esse controle não existia de forma auditável. A Altave pediu um sistema de ponto que registrasse as movimentações, apresentasse indicadores e gerasse relatórios.

A solução foi um sistema web com backend em Spring Boot, frontend em Vue.js e PostgreSQL, com dashboards de movimentação, controle de contratos e exportação de relatórios, empacotado para rodar via Docker Compose.

**Repositório:** [SQLutions-FATEC/API-3-Semestre](https://github.com/SQLutions-FATEC/API-3-Semestre)

### 🛠️ Tecnologias utilizadas

- **Spring Boot** — estruturou a API REST em camadas e permitiu que o time trabalhasse em controllers e services separados sem colisão. Eu já vinha estudando Spring por fora, o que me colocou como referência técnica do time nesta stack.
- **PostgreSQL** — sustentou o modelo de empresas, funcionários, contratos e movimentações, incluindo as consultas agregadas dos dashboards e o soft delete que preservava histórico de quem saía.
- **Vue.js** — frontend das telas de cadastro, filtro e dashboard, consumindo a API. Foi a camada em que atuei menos e onde declaro dependência de apoio.
- **Docker e Docker Compose** — foi decisão de produto, não conveniência de desenvolvimento: o cliente precisava rodar o sistema sozinho para validar, e um `docker-compose up -d` subia o banco configurado sem que ele instalasse PostgreSQL na máquina.
- **Swagger / OpenAPI** — deu ao cliente e aos professores uma forma de validar os endpoints direto no navegador, sem Postman e sem depender de nós.
- **JPA / Hibernate e Lombok** — reduziram o código repetitivo de acesso a dados e de DTOs, o que importava num semestre em que eu dividia meu tempo entre produto e backend.
- **Jira** — backlog, acompanhamento de sprint e burndown, que era também o material de prestação de contas ao cliente.

### 👤 Contribuições pessoais

- **Meu papel e a negociação de requisitos com cliente externo.** Atuei como Product Owner, agora diante de um cliente de fora da faculdade. Documentei as oito User Stories do projeto com DoR, DoD e critérios de aceite, incluindo regras específicas como validação de datas de contrato, máscara de CNPJ, filtros de movimentação por empresa, funcionário e data, e regras de exportação. Diferente do semestre anterior, o cliente tinha agenda própria e tempo de resposta longo, o que exigiu renegociar escopo e prazo de entrega mais de uma vez ao longo das sprints.
- **Decisões técnicas tomadas em função da validação pelo cliente.** Configurei o Spring com `spring.sql.init.mode=always` e `ddl-auto=create-drop` para que 228 linhas de dados realistas de empresas, funcionários, contratos e movimentações fossem carregadas a cada inicialização. O cliente abria o sistema e já tinha o que validar. A entrega final foi empacotada como `.jar` do backend, `dist` do frontend e `compose.yaml` em uma pasta única, com instalação em três comandos.
- **Desenvolvimento do backend.** Construí a estrutura de controllers, services com interface e implementação, repositories, DTOs e entities, e os CRUDs de Movimentações, Empresas e Funcionários. Desenvolvi o módulo de Analytics com as consultas de registros diários, horas por cargo, contratos a expirar, clock-ins incompletos e funcionários por turno, além do soft delete com filtro nas queries. Olhando do sexto semestre, foi o mesmo desvio de função do 2º semestre, repetido: eu era o Product Owner e, ainda assim, construí a base do backend.

### 📊 Hard Skills

| Habilidade | Nível alcançado | Evidência |
|:-|:-|:-|
| Spring Boot | 🟢 Sei fazer com autonomia | `controller/`, `service/impl/` e `repository/` do backend |
| PostgreSQL | 🟢 Sei fazer com autonomia | `src/main/resources/data.sql` — 228 linhas de carga inicial |
| Docker / Docker Compose | 🟢 Sei fazer com autonomia | `compose.yaml` e `Dockerfile` do backend |
| JPA / Hibernate | 🟢 Sei fazer com autonomia | `entity/` e `repository/`, com soft delete filtrado nas queries |
| Swagger / OpenAPI | 🟢 Sei fazer com autonomia | Dependência springdoc em `pom.xml`, endpoints anotados |
| Vue.js | 🟡 Sei fazer com ajuda | Repositório de frontend do projeto |
| Escrita de documentação técnica | 🟢 Sei fazer com autonomia | `docs/install/README.md` — guia com troubleshooting |
| Gestão de produto e negociação de requisitos | 🟢 Sei fazer com autonomia | `docs/README.md` e burndowns em `docs/media/` |

### 🧠 Soft Skills

- **Lidar com as consequências.** O integrante que vinha descumprindo os critérios de permanência desde o segundo semestre continuou no grupo, agora com o desgaste visível na equipe. Fui eu, com dois colegas, que levei a decisão de aplicar o critério e desligá-lo, num grupo de nove pessoas em que a maioria era passiva e não colocava posição na mesa. Foram cerca de dez meses entre o primeiro sintoma e a decisão. Aprendi que critério que não se aplica não é critério, e que como PO a responsabilidade de puxar essa conversa era minha, não do professor nem do grupo.
- **Escuta de requisito sem preencher lacuna com interpretação própria.** Com um cliente real, percebi que eu completava as informações que faltavam com o meu próprio entendimento do negócio em vez de voltar e perguntar, o que gerou retrabalho em pontos de regra de negócio. O trabalho de produto foi elogiado pelo cliente ao fim do semestre, mas, olhando do sexto semestre, eu faria diferente: desconstruiria a fala dele, daria alguns passos atrás para entender os conceitos nos termos dele e validaria mais com o professor orientador antes de transformar conversa em User Story.
- **Gestão de dependência externa.** O tempo de resposta do cliente foi a maior fonte de atrito do semestre e travou decisões que eu não podia tomar sozinho. Foi frustrante, e foi também a experiência mais próxima de mercado que tive até aqui: aprendi a manter frentes paralelas andando enquanto uma resposta não chegava, e a registrar por escrito o que estava bloqueado e desde quando.

---

## 4º Semestre • 2/2025 • Radarius — Monitoramento Inteligente de Tráfego

![Spring Boot](https://img.shields.io/badge/Spring_Boot_3-6DB33F?style=flat&logo=springboot&logoColor=white) ![Oracle](https://img.shields.io/badge/Oracle_Database-F80000?style=flat&logo=oracle&logoColor=white) ![Vue.js](https://img.shields.io/badge/Vue.js_3-4FC08D?style=flat&logo=vuedotjs&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white) ![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat&logo=nginx&logoColor=white) ![JWT](https://img.shields.io/badge/JWT-000000?style=flat&logo=jsonwebtokens&logoColor=white)

O parceiro foi a [Prefeitura de São José dos Campos](https://www.sjc.sp.gov.br/), por meio da área de mobilidade urbana.

A cidade tinha dados de radares, mas não tinha um sistema que os transformasse em decisão. Não havia como definir indicadores com níveis de severidade, disparar alerta quando um limiar fosse ultrapassado nem alocar agentes de mobilidade com base no que estava acontecendo na via.

A solução foi o Radarius, com dashboard interativo, mapa zonal, alertas automáticos e controle de acesso por perfil de usuário. Backend em Spring Boot 3 com Oracle Database, frontend em Vue.js 3 com Vite e deploy completo em Docker com Nginx.

**Repositório:** [DenariusData/API-4SEM](https://github.com/DenariusData/API-4SEM)

### 🛠️ Tecnologias utilizadas

- **Spring Boot 3** — base da API REST e do agendamento interno de verificação de indicadores. A versão 3 exigiu adequação de configuração em relação ao que eu conhecia do semestre anterior.
- **Oracle Database com autenticação por Wallet** — requisito do semestre e a primeira vez que subi um banco acessado remotamente por todo o time. O Wallet exigiu tratar credencial como volume no container, não como variável solta.
- **Vue.js 3 com Vite** — frontend do dashboard e do mapa, com build otimizado para servir em produção.
- **Spring Security com JWT** — sustentou o controle de acesso por perfil, que era pré-requisito de praticamente toda tela do sistema: gestor, agente e administrador veem coisas diferentes.
- **Docker, Docker Compose e Nginx** — containerização das três pontas com health checks, rede isolada e proxy reverso do frontend para a API, o que permitiu subir o sistema inteiro em qualquer máquina do time com a mesma configuração.
- **GitHub Actions** — automação da descrição de Pull Requests, para reduzir o custo do code review obrigatório que estabelecemos.

### 👤 Contribuições pessoais

- **Meu papel e a camada de segurança completa.** Voltei à cadeira de desenvolvedor depois de dois semestres como Product Owner. Implementei a autenticação com JWT de ponta a ponta — `JwtIssuer`, `JwtAuthenticationFilter`, `TokenDecoder` e `JwtToPrincipalConverter` — mais a configuração do Spring Security em `WebSecurityConfig`, o `AuthController` com login e o `CustomUserDetailService` para integração com o banco. Também protegi os endpoints garantindo que a lógica por ROLE funcionasse em cada rota. Era o módulo que desbloqueava o trabalho dos outros e por isso foi o primeiro a ser entregue.
- **Ciclo de alerta e monitoramento.** Implementei a lógica de criação do log de alerta e o `LevelScheduler`, que verificava mudança de nível nos indicadores de tráfego e disparava alerta ao ultrapassar o limiar — classe que o time depois substituiu por um scheduler de processamento das leituras de radar. Implementei também o ciclo completo do alerta: criação automática, registro em `AlertLog`, associação com causa raiz e protocolo, filtragem por região do usuário e endpoint de finalização. Criei também o CRUD de protocolos e causas raiz, que é o que permite ao gestor orientar o agente em campo.
- **Banco em nuvem e infraestrutura.** Subi o Oracle Database acessado por todo o time, com configuração de Wallet, migrando o projeto do PostgreSQL. A migração quebrou a estratégia de geração de ID, que passou a `SEQUENCE`, e exigiu renomear entidades (`User` → `Person`, `Zone` → `Region`) e remover relações que só existiam por conveniência do Postgres. Escrevi o `Dockerfile` do backend com Zulu OpenJDK 21, o do frontend com Node 20 e Nginx, e o `docker-compose.yml` com health check em `/actuator/health`, rede bridge isolada, volume para o Wallet e política de restart.
- **Processo de engenharia.** Defini o padrão de Conventional Commits, a estrutura de branches com prazo (domingo às 19h para features e 23h para a main) e o code review obrigatório com responsabilidade compartilhada entre autor e revisor. Foi a experiência de PO dos dois semestres anteriores aplicada a partir de uma cadeira de desenvolvedor.

### 📊 Hard Skills

| Habilidade | Nível alcançado | Evidência |
|:-|:-|:-|
| Spring Boot 3 | 🟢 Sei fazer com autonomia | Backend `data.denarius.radarius` |
| Spring Security e JWT | 🟢 Sei fazer com autonomia | `security/` — `JwtIssuer`, `JwtAuthenticationFilter`, `TokenDecoder`, `JwtToPrincipalConverter`, `WebSecurityConfig` |
| Oracle Database | 🟢 Sei fazer com autonomia | `src/main/resources/application.yaml` com autenticação por Wallet |
| Docker / Docker Compose | 🟢 Sei fazer com autonomia | `docker-compose.yml` e `DOCKER_README.md` |
| Modelagem de banco de dados | 🟢 Sei fazer com autonomia | `entity/` — `Person`, `Region`, `CriterionLevel`, `AlertLog` |
| Vue.js 3 | 🟡 Sei fazer com ajuda | Repositório de frontend do projeto |
| Nginx e proxy reverso | 🟡 Sei fazer com ajuda | `nginx.conf` do frontend |
| CI/CD com GitHub Actions | 🟡 Sei fazer com ajuda | Workflow `pr-description` |

### 🧠 Soft Skills

- **Autoridade sem mandato.** Eu e mais dois colegas saímos do grupo de nove pessoas do semestre anterior justamente pela morosidade da equipe, e entramos num grupo menor. O perfil do problema mudou de forma: no lugar de gente parada, encontramos gente que propunha muita ideia e entregava pouco. A diferença decisiva em relação ao semestre anterior é que este grupo nunca tinha definido critério de permanência: no 3º semestre havia uma regra escrita que eu pude invocar para conduzir um desligamento, e aqui não havia regra nenhuma, então não havia o que aplicar. Como éramos três recém-chegados, também nos sentimos acuados para propor uma do zero. Faltou coragem, e o resultado foi que os módulos críticos do sistema ficaram concentrados em nós três. Aprendi que critério de permanência se pactua na entrada, enquanto ninguém ainda está sendo cobrado por ele — depois que o problema aparece, qualquer regra proposta vira acusação pessoal.
- **Adaptabilidade sob requisito imposto.** A troca de PostgreSQL para Oracle veio como requisito do semestre logo no início, antes de o backend estar funcionando. O custo foi refazer o planejamento e descobrir os drivers e a configuração corretos para o Oracle, além de ajustar a geração de ID, o Wallet no container e a modelagem que eu já tinha começado. Por ter acontecido cedo, a mudança não bloqueou ninguém do time.
- **Contrapeso técnico às ideias do grupo.** Com o papel de PO ocupado por um dos colegas que vieram comigo, eu servia como uma segunda cabeça pensando do lado do código: quando os colegas mais "sonhadores" da equipe cogitavam prometer ao cliente mais do que a stack ou o prazo permitiam, era eu quem questionava a viabilidade técnica antes que a ideia virasse compromisso. Esse contrapeso, somado a definir o padrão de commit, o prazo de branch e o code review obrigatório, foi a forma que encontrei de dar previsibilidade a uma equipe em que eu não tinha autoridade formal para cobrar ninguém. Foi a primeira vez que usei análise técnica e processo como substituto de autoridade, e funcionou melhor do que a cobrança direta que eu não me sentia à vontade para fazer.

---

## 5º Semestre • 1/2026 • Lunae — Data Warehouse Corporativo

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white) ![Django](https://img.shields.io/badge/Django-092E20?style=flat&logo=django&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white) ![Vue.js](https://img.shields.io/badge/Vue.js-4FC08D?style=flat&logo=vuedotjs&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white) ![Packer](https://img.shields.io/badge/Packer-02A8EF?style=flat&logo=packer&logoColor=white) ![QEMU](https://img.shields.io/badge/QEMU-FF6600?style=flat&logo=qemu&logoColor=white) ![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat&logo=nginx&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat&logo=githubactions&logoColor=white) ![Locust](https://img.shields.io/badge/Locust-2F855A?style=flat)

O parceiro foi a [SIATT](https://www.siatt.com.br/), empresa do setor de defesa. Por lidar com dados sensíveis, a empresa exigia que a aplicação rodasse inteiramente on-premise, sem que o dashboard ou seus dados transitassem pela internet.

A SIATT não tinha uma fonte única de verdade: informações de diferentes departamentos viviam espalhadas, sem um modelo comum que permitisse cruzar dados entre áreas. A demanda era um data warehouse que centralizasse essas informações e servisse de base analítica para toda a empresa.

A solução foi o **Lunae**, um data warehouse com backend em Django e frontend em Vue.js/TypeScript, modelado em star schema sobre PostgreSQL. Como o deploy não podia depender de internet nem de acesso remoto contínuo da equipe, a entrega incluiu uma imagem de VM pronta para ativação, provisionada via Packer e configurada automaticamente no primeiro boot via cloud-init.

**Repositório:** [23deFevereiro/FATEC-API-5-Semestre](https://github.com/23deFevereiro/FATEC-API-5-Semestre)

### 🛠️ Tecnologias utilizadas

- **Django** — não era minha stack mais forte até então (vinha de dois semestres em Spring Boot), mas ainda assim acabei como peça central do desenvolvimento, o que exigiu ritmo de aprendizado acelerado dentro do próprio projeto.
- **PostgreSQL com modelagem em star schema** — organizou os dados em tabelas fato e dimensão para sustentar consultas analíticas entre departamentos, em vez de um modelo puramente transacional.
- **Packer com builder QEMU/KVM** — construiu uma imagem de disco reprodutível a partir do Ubuntu 24.04 cloud image, eliminando a instalação manual a cada ativação. A imagem sai em `qcow2` e é convertida para VDI, formato que o time de TI da SIATT consegue importar direto.
- **Cloud-init (datasource NoCloud)** — configurou rede, banco e variáveis de ambiente da aplicação automaticamente no primeiro boot da VM, via seed ISO entregue ao time de TI do cliente.
- **Nginx e Gunicorn** — nginx serve o build estático do Vite e faz proxy reverso para o Gunicorn, que escuta apenas em `127.0.0.1:8000`. Num cliente de defesa, isso significa que o Django não fica exposto à rede mesmo se o firewall da VM for mal configurado.
- **GitHub Actions** — transformou a geração da imagem em pipeline: o build que antes eu rodava na mão virou um workflow disparável por versão, o que tornou a imagem reproduzível por qualquer pessoa do time.
- **Locust** — teste de carga que serviu de base para o parecer de dimensionamento. Sem número medido, a discussão sobre recursos com o cliente seria opinião contra opinião.
- **NestJS, React/TypeScript e PostgreSQL (Scrum Warden)** — sistema próprio que construí para automatizar a contabilização dos critérios de permanência da equipe.

### 👤 Contribuições pessoais

- **Meu papel e a modelagem do data warehouse.** Comecei como Scrum Master e, ainda na primeira semana, passei a desenvolvedor depois que o time identificou que a demanda técnica do projeto pedia mais força nessa frente. Construí o star schema do projeto, organizando os dados da SIATT em tabelas fato e dimensão para sustentar o papel do Lunae como fonte única de verdade entre departamentos.
- **Pipeline de deploy on-premise.** Defini e implementei a estratégia de entrega via imagem de VM. Montei o build Packer com QEMU/KVM sobre o Ubuntu 24.04, com um script de provisionamento que instala a stack, cria usuário de serviço sem shell, publica o backend em venv e o frontend estático, configura o site do nginx e registra o Gunicorn como unidade systemd. O cloud-init assume no primeiro boot, de modo que o time de TI da SIATT apenas ativa a VM e a integra à rede interna, sem depender de mim para instalação.
- **Automação da geração da imagem.** Levei o build para um workflow de GitHub Actions: habilita KVM no runner, compila o frontend, empacota back e front, instala Packer e QEMU, gera uma chave SSH efêmera injetada no cloud-init só para o build, converte `qcow2` para VDI e publica a imagem versionada em um bucket de object storage com link de download. O ganho real não foi conveniência, e sim reprodutibilidade: a imagem deixou de depender da minha máquina.
- **Dimensionamento de capacidade com teste de carga.** O cliente já tinha definido os recursos da VM e meu papel foi dizer se bastavam. Medi três cenários com Locust e escrevi o parecer: com 1 vCPU, 50 usuários simultâneos respondem com p95 de 3,6 s, mas 200 usuários levam o p95 a 11 s, o que inviabiliza o uso; com 4 vCPUs, o mesmo pico volta a 4,0 s e o throughput dobra para 32,5 RPS. Recomendei manter 1 vCPU até o 12º mês e provisionar 4 antes do 13º, e documentei também o que não precisava mudar — RAM, nginx e o banco, que no pico não passou de quatro conexões ativas.
- **Scrum Warden.** Ainda na semana como Scrum Master, formalizei os critérios de permanência da equipe em documento (sistema de pontos por sprint, limites e consequências) e construí uma aplicação própria — NestJS, React com TypeScript e PostgreSQL, containerizada com Docker — para contabilizar essas regras automaticamente, em vez de depender de planilha manual.

### 📊 Hard Skills

| Habilidade | Nível alcançado | Evidência |
|:-|:-|:-|
| Django | 🟡 Sei fazer com ajuda | `API_5_SEM_BACK/api/` |
| Modelagem dimensional (star schema) | 🟡 Sei fazer com ajuda | `api/models/` — oito dimensões `dim_*` e quatro fatos `fato_*` |
| Packer e provisionamento de imagens | 🟢 Sei fazer com autonomia | `infra/packer/lunae.pkr.hcl` e `scripts/install.sh` |
| Cloud-init | 🟢 Sei fazer com autonomia | `infra/packer/cloud-init/user-data.example` e `examples/` |
| Nginx e Gunicorn em produção | 🟢 Sei fazer com autonomia | `infra/packer/files/nginx-site.conf` e `lunae-backend.service` |
| CI/CD com GitHub Actions | 🟢 Sei fazer com autonomia | `.github/workflows/build-image.yml` |
| Teste de carga com Locust | 🟡 Sei fazer com ajuda | `docs/deploy.md`, seção 2.2 — RPS, p50 e p95 por cenário |
| Dimensionamento de capacidade | 🟡 Sei fazer com ajuda | `docs/deploy.md`, seção 2 — parecer de vCPUs e justificativa |
| NestJS | 🟢 Sei fazer com autonomia | Repositório do Scrum Warden |

### 🧠 Soft Skills

- **Equipe com critério pactuado na entrada.** Eu e os dois colegas que me acompanham desde o início do curso entramos no semestre já com critérios de permanência sérios definidos, corrigindo o que faltou no 4º semestre: pactuar regra de convivência desde o início, não depois que o problema aparece. Foi um alívio real ter uma equipe que de fato funcionava nesse aspecto, mesmo que, tecnicamente, o grupo não tenha sido tão eficiente.
- **Demora em validar decisão técnica.** Levei tempo demais para validar a estratégia de deploy on-premise com o professor orientador, o que só piorou a situação — eu vinha de uma concepção limitada, habituado a deploy em VMs de nuvem, e isso tornou o problema mais difícil do que precisava ser. Olhando do sexto semestre, eu teria buscado validação bem mais cedo.
- **O custo de escolher a entrega pelo conforto do cliente.** Optei pela imagem de VM porque era o que o hypervisor da SIATT consumia direto, sem que o TI tivesse trabalho. A decisão estava certa do ponto de vista do cliente e cara do meu: achar uma imagem base que servisse, resolver a instalação dentro do build e acertar o cloud-init consumiu semanas de tentativa e erro, e o histórico de commits registra isso em commits de depuração. Olhando do sexto semestre, eu pelo menos colocaria na mesa a alternativa de um instalável autocontido antes de assumir o formato mais pesado — não porque a escolha tenha sido errada, mas porque eu nunca comparei o custo das duas.

---

## 6º Semestre • 2/2026 • Índice — Gestão Documental Inteligente

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white) ![Django](https://img.shields.io/badge/Django-092E20?style=flat&logo=django&logoColor=white) ![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat&logo=scikitlearn&logoColor=white) ![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat&logo=ollama&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white) ![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat&logo=mongodb&logoColor=white) ![Vue.js](https://img.shields.io/badge/Vue.js_3-4FC08D?style=flat&logo=vuedotjs&logoColor=white)

O parceiro foi a [Akaer](https://akaer.com.br/), empresa de engenharia e tecnologia que atua nos setores aeroespacial, de defesa e industrial.

A gestão de documentos técnicos na Akaer era inteiramente manual: o profissional lia cada documento, associava-o às normas e aos arquivos semelhantes já existentes na base e atribuía os rótulos que permitiriam encontrá-lo depois. Pelo volume e pela complexidade dos conceitos envolvidos, o processo consumia horas de trabalho especializado e era sujeito a erro. Some-se a isso o fato de que boa parte desse material, num cliente dos setores de defesa e aeroespacial, não pode circular fora da empresa.

A solução foi o Índice, uma plataforma de ingestão, classificação e busca de documentos técnicos. Cada arquivo enviado é classificado automaticamente, recebe título e resumo gerados por modelo de linguagem e passa a ser recuperável por busca, com controle de acesso por perfil.

**Repositório:** [Pragma-Co/indice](https://github.com/Pragma-Co/indice)

### 🛠️ Tecnologias utilizadas

- **PyTorch** — base da rede neural de classificação. O modelo roda em CPU dentro do próprio container do backend, sem GPU e sem chamada a serviço externo, que era a condição imposta pelo cliente.
- **scikit-learn** — vetorização TF-IDF do texto dos documentos, que alimenta a rede, e divisão estratificada da base entre treino e avaliação.
- **Ollama com Llama 3.2 1B** — gerou título e resumo localmente. Um modelo de 1 bilhão de parâmetros cabe na máquina do cliente, e esse foi o critério de escolha: o conteúdo do documento não deixa a infraestrutura.
- **Django com PostgreSQL e MongoDB** — o relacional guarda os metadados estruturados de documento, revisão e permissão; o MongoDB guarda o conteúdo não estruturado extraído dos arquivos.
- **Docker** — empacotou backend, bancos e Ollama, garantindo que o modelo treinado rodasse igual em qualquer máquina do time e na do cliente.
- **GitHub Actions** — integração contínua validando build, padrão de commit, lint e testes a cada Pull Request.

### 👤 Contribuições pessoais

- **Meu papel e o classificador de documentos.** Atuei como desenvolvedor e assumi o modelo de classificação automática, que era a entrega central do semestre. Construí o pipeline inteiro — pré-processamento do texto, vetorização TF-IDF com 5.000 features e uma rede neural em PyTorch com tronco compartilhado e três saídas, que classificam de uma vez disciplina, tipo de documento e área. Substituí modelos separados por campo por essa rede única, apliquei balanceamento de classes e parada antecipada, e o modelo final chegou a 93,8% de acurácia em disciplina e em tipo de documento e 88,5% em área.
- **Destilação para contornar a falta de dados.** A Akaer não forneceu base rotulada suficiente para treinar, e a base que montamos à mão também não bastou. Usei então um modelo de linguagem maior para rotular os documentos e treinei a rede pequena com esses rótulos, chegando a 565 documentos de treino. Foi a decisão que destravou o semestre: sem ela, não havia classificador.
- **Sigilo como requisito de arquitetura.** Num primeiro momento usei a API do Groq como solução paliativa para sugerir os metadados. O próprio cliente criticou a abordagem pela falta de sigilo, já que o conteúdo do documento saía para um serviço de terceiros. Troquei então a sugestão pelo classificador local e integrei o Ollama para gerar resumo em português e título derivado dele, com resposta em streaming — nenhum documento deixa mais a infraestrutura.
- **Exclusão de usuário que sobrevive ao backup (LGPD).** A LGPD era o tema do semestre, e excluir a conta não bastava, porque qualquer restore de backup a traria de volta. Criei um banco PostgreSQL separado, em container próprio e fora do restore da aplicação, que guarda só o hash HMAC do e-mail de cada conta excluída, sem dado pessoal. Depois de um restore, o comando `reapply_user_erasures` compara as contas restauradas com esse registro e reaplica a anonimização ou a exclusão, gravando cada reaplicação no log de auditoria.
- **Integração contínua.** Configurei os quatro workflows do projeto: build da imagem do backend, verificação do padrão das mensagens de commit, lint e execução dos testes, todos disparados a cada Pull Request.

### 📊 Hard Skills

| Habilidade | Nível alcançado | Evidência |
|:-|:-|:-|
| Redes neurais com PyTorch | 🟡 Sei fazer com ajuda | `classifier/network.py` — tronco compartilhado e três cabeças de classificação |
| Pré-processamento e vetorização de texto | 🟡 Sei fazer com ajuda | `classifier/text_preprocessing.py` e `tfidf_input.py` |
| Treino e avaliação de modelos | 🟡 Sei fazer com ajuda | `classifier/neural_training.py`, `evaluation.py` e as métricas em `classifier_artifacts/metadata.json` |
| Rotulagem assistida por LLM e destilação | 🟡 Sei fazer com ajuda | `classifier/dataset.py` e o catálogo de rótulos em `catalog.json` |
| Execução local de LLM com Ollama | 🟢 Sei fazer com autonomia | `core/ollama_client.py` — geração de título e resumo em streaming |
| Adequação à LGPD (eliminação de dados) | 🟢 Sei fazer com autonomia | `core/services/user_erasure_reapplication_service.py`, `excluded_identifier_service.py` e a seção de restore em `infra/README.md` |
| CI com GitHub Actions | 🟢 Sei fazer com autonomia | `.github/workflows/` — `build`, `commit-lint`, `lint` e `test` |

### 🧠 Soft Skills

- **Resposta à crítica do cliente.** A Akaer apontou que a solução paliativa expunha o conteúdo dos documentos a um serviço de terceiros. Em vez de defender o atalho que eu mesmo tinha escolhido, tratei a crítica como requisito e redesenhei a sugestão de metadados para rodar inteiramente dentro do sistema. Num cliente de defesa, sigilo não é etapa final de projeto: é premissa da primeira versão, e eu só entendi isso depois de ouvir do cliente.
- **Aprender em terreno novo, e o custo de fazer isso sozinho.** Era a primeira vez que eu treinava um modelo de classificação, e passei boa parte do semestre quebrando a cabeça por conta própria — inclusive na falta de dados, que era o problema mais difícil. O conhecimento estava disponível nos professores e eu não fui buscar. É o mesmo padrão do 5º semestre, quando demorei a validar a estratégia de deploy com o orientador, e reconhecer a repetição foi o que me fez perceber que não era falta de acesso, e sim resistência a pedir ajuda.
- **Decidir pesando a consequência antes, não depois.** Foi o semestre com menos atrito de equipe de toda a trajetória e a entrega saiu antes do prazo, e isso não foi sorte: quase tudo que importou foi decidido antes de o projeto começar. O grupo combinou na entrada que levaria o projeto a sério, fixou os critérios de permanência para que pudéssemos cobrar uns aos outros de forma acordada — sustentados pelo Scrum Warden, que eu havia construído no semestre anterior — e escolheu as tecnologias com produtividade como critério explícito, não por preferência. É a resposta direta ao que faltou no 4º semestre, quando entrei num grupo sem critério nenhum e não tive o que invocar. A exceção foi o classificador, onde eu avancei por tentativa e erro em vez de medir o terreno antes.

---

## Fio condutor dos seis semestres

O mesmo problema atravessa os quatro primeiros: como lidar com falta de comprometimento em equipe acadêmica. No 1º semestre eu entregava pela pessoa. No 2º, insisti em manter no grupo, por afinidade, justamente quem estava ausente — e absorvi o vácuo técnico dela. No 3º, apliquei o critério de permanência e conduzi o desligamento, dez meses depois do primeiro sintoma. No 4º, mudei de ambiente e descobri que trocar de grupo não substitui pactuar regra na entrada. No 5º, esse arco se fecha: entramos com critério de permanência pactuado desde o primeiro dia, não mais construído em resposta a um problema já instalado. E no 6º ele deixa de ser arco e vira método: o critério foi acordado na entrada e sustentado por uma ferramenta que eu mesmo havia construído para isso, num semestre que terminou antes do prazo e com o menor atrito de equipe de toda a graduação.

No eixo técnico o caminho é inverso e mais linear: comecei em lógica e módulos isolados, passei por dois semestres em que a técnica veio como desvio de função, e voltei ao papel de desenvolvedor com a camada de segurança, o banco em nuvem e a infraestrutura do time — agora no lugar certo. No 5º semestre esse eixo ganha uma dobra nova: entrei numa stack (Django) e num domínio (deploy on-premise, provisionamento de imagem) onde eu tinha menos base do que em qualquer semestre anterior, e ainda assim acabei como peça central da entrega — o que mostra que a atuação técnica deixou de depender de terreno conhecido. O 6º leva isso ao limite, com o treino de uma rede neural de classificação, território em que eu não tinha base nenhuma. E acrescenta um movimento que os anteriores não tinham: a decisão técnica central do projeto — trocar a API externa por modelo rodando localmente — foi tomada por uma razão de negócio, o sigilo exigido pelo cliente, e não por preferência de arquitetura.

O último eixo usa o vocabulário do [CliftonStrengths](https://www.gallup.com/cliftonstrengths/pt/253724/34-temas-cliftonstrengths.aspx), modelo da Gallup que descreve 34 temas de talento distribuídos em quatro domínios: Execução, Influência, Construção de relacionamento e Pensamento estratégico. Os temas a seguir foram atribuídos a partir das situações narradas nas soft skills de cada semestre, e servem para nomear o que se repete entre elas.

Nesse eixo, o percurso começa pelo apetite de aprendizado, com Estudioso no 1º semestre e Input no 2º, ao lado da Disciplina de organização que já aparece no primeiro projeto. O que falta no 2º é o Foco, quando a energia se dispersa entre o papel de PO e um backend que não era meu. A Restauração chega no 3º, com a disposição de agir dirigida, enfim, ao problema certo. A Adaptabilidade aparece duas vezes em contextos diferentes — dependência de cliente no 3º, requisito técnico imposto no 4º —, sinal de que deixou de ser reação pontual para virar padrão. O Comando que faltava ao fim do 4º semestre aparece exercido no 5º, com o critério de permanência pactuado desde o início. O tema que demora mais a chegar é a Prudência: faltou ao interpretar requisito no 3º, apareceu só de forma indireta como Analítico no 4º, voltou a faltar no 5º com a demora em validar a estratégia de deploy, e só se firma no 6º, quando quase tudo que importou foi decidido antes de o projeto começar. A Restauração reaparece ali no mesmo movimento — a crítica do cliente ao sigilo não virou defesa do atalho, virou reescrita da solução.

### 📈 Evolução dos temas CliftonStrengths

| Domínio | Tema | 1º | 2º | 3º | 4º | 5º | 6º |
|:-|:-|:-:|:-:|:-:|:-:|:-:|:-:|
| Execução | Disciplina | ✅ | | | | | |
| Execução | Foco | | ❌ | | | | |
| Execução | Restauração | | | ✅ | | | ✅ |
| Execução | Prudência | | | ❌ | | ❌ | ✅ |
| Pensamento estratégico | Estudioso | ✅ | | | | | ✅\* |
| Pensamento estratégico | Input | | ✅ | | | | |
| Pensamento estratégico | Analítico | | | | ✅ | | |
| Construção de relacionamento | Adaptabilidade | | | ✅ | ✅ | | |
| Influência | Comando | | | | ❌ | ✅ | |

✅ *Exercido* significa que o tema sustentou a atuação naquele semestre; ❌ *Ausente*, que a situação o exigia e ele não apareceu. Célula vazia indica que o tema não foi determinante no semestre.

\* No 6º semestre, Estudioso aparece exercido no aprendizado de uma técnica inteiramente nova, mas acompanhado da resistência em pedir ajuda aos professores — o mesmo padrão do 5º semestre, quando demorei a validar a estratégia de deploy com o orientador.

---

## Agradecimento

Ao longo dos seis semestres, dois colegas estiveram comigo em todos os projetos: Tiago Reis e Augusto Piatto. Boa parte do que descrevo aqui como decisão minha foi, na prática, decisão tomada com eles — da saída do grupo no 4º semestre ao critério de permanência pactuado no 5º. Os papéis formais variaram a cada semestre, mas o núcleo de confiança não, e isso é o que tornou possível sustentar posição em grupos onde eu não tinha autoridade formal para cobrar ninguém.