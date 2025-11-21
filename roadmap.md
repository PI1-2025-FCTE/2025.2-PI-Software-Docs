# Roadmap

## Introdução

<div align="justify">&emsp;&emsp;
Este documento apresenta a organização estratégica do projeto, descrevendo as principais fases, entregas e marcos planejados ao longo do seu desenvolvimento. O roadmap tem como finalidade orientar as atividades, garantir o alinhamento entre os envolvidos e permitir uma visão clara do progresso ao longo do tempo.
</div>

## Objetivos

Os principais objetivos deste roadmap são:

- Definir claramente as etapas do projeto e suas respectivas entregas;
- Facilitar o acompanhamento do cronograma e da evolução das atividades;
- Auxiliar na priorização de tarefas de acordo com o impacto e necessidade;
- Promover melhor comunicação e alinhamento entre os participantes do projeto.

## Equipe

| Nome                                                                  | Matrícula | Papel                                 |
| --------------------------------------------------------------------- | --------- | ------------------------------------- |
| [Eduardo Matheus dos Santos Sandes](https://github.com/DiceRunner714) | 221008024 | Gerente de software e desenvovedor    |
| [Guilherme Flyan Araujo](https://github.com/GFlyan)                   | 231011408 | Subgerente de software e desenvovedor |
| [André João Cordeiro Gomes](https://github.com/AJCGassassin)          | 211061402 | Desenvovedor                          |
| [Cássio Sousa dos Reis](https://github.com/csreis72)                  | 221021886 | Desenvovedor                          |
| [Márcio Henrique de Sousa Costa](https://github.com/DeM4rcio)         | 221039497 | Desenvovedor                          |
| [Yasmin Dayrell Albuquerque](https://github.com/YasminDayrell)        | 232014226 | Desenvovedora                         |

---

## Sprint 1: Pesquisa e capacitação
- **Duração:** 7 dias  
- **Início:** 15/09/2025  
- **Término/Entrega:** 22/09/2025

### Objetivos
- Pesquisa sobre ferramentas:
    - Como enviar e receber dados de ESP32 via bluetooth ou WiFi?
    - Docker
    - Python3
    - fastAPI (API's REST nos atendem?)
    - PostgreSQL
    - React
    - TypeScript
- Definir formato dos dados entre o software e o hardware;
- Início do levantamento de requisitos.

### Tarefas chave
- Se capacitar nas ferramentas desconhecidas;
- Pequisar sobre a comunicação com o Hardware;
- Realizar um brainstorming para começar o levantamento de requisitos e soluções.

## Alocação da equipe

| Nome                                                   | Tarefas |
| ------------------------------------------------------ | ------- |
| [Eduardo Sandes](https://github.com/DiceRunner714)     | Todas   |
| [André Gomes](https://github.com/AJCGassassin)         | Todas   |
| [Cássio Reis](https://github.com/csreis72)             | Todas   |
| [Guilherme Araujo](https://github.com/GFlyan)          | Todas   |
| [Márcio Costa](https://github.com/DeM4rcio)            | Todas   |
| [Yasmin Albuquerque](https://github.com/YasminDayrell) | Todas   |

---

## Sprint 2: Levantamento, priorização e modelagem de requisitos além de prototipação
- **Duração:** 2 semanas
- **Início:** 22/09/2025
- **Término/Entrega:** 06/10/2025

### Objetivos
- Definir qual o escopo de software;
- Levantar os requisitos da área de software;
- Documentar os requisitos de forma clara;
- Modelar os requisitos;
- Priorizar os requisitos;
- Gerar protótipos de baixa e alta fidelidade.

### Entregáveis
- ✅ [Diagrama de casos de uso](https://github.com/PI1-2025-FCTE/2025.2-PI-Software-Docs/blob/main/diagrama-caso-uso.md)
- ✅ [Histórias de usuário](https://github.com/PI1-2025-FCTE/2025.2-PI-Software-Docs/blob/main/historias-de-usuario.md)
- ✅ [MoSCoW](https://github.com/PI1-2025-FCTE/2025.2-PI-Software-Docs/blob/main/moscow.md)
- ✅ [Diagrama entidade relacionamento (DER)](https://github.com/PI1-2025-FCTE/2025.2-PI-Software-Docs/blob/main/assets/diagrama-entidade-relacionamento.png)
- ✅ [Diagrama lógico de dados (DLD)](https://github.com/PI1-2025-FCTE/2025.2-PI-Software-Docs/blob/main/assets/diagrama-logico-de-dados.png)
- ✅ [Diagrama BPMN](https://github.com/PI1-2025-FCTE/2025.2-PI-Software-Docs/blob/main/assets/BPMN%20.png)
- ✅ [Diagrama de estados](https://github.com/PI1-2025-FCTE/2025.2-PI-Software-Docs/blob/main/diagrama-estados.md)
- ❌ Fluxo de dados
- ✅ [Requisitos não funcionais (RNF's)](https://github.com/PI1-2025-FCTE/2025.2-PI-Software-Docs/blob/main/requisitos-nao-funcionais)
- ✅ [Diagrama de alto nível (arquitetura)](https://github.com/PI1-2025-FCTE/2025.2-PI-Software-Docs/blob/main/arquitetura.md)
- ✅ Protótipo de baixa fidelidade
- ✅ [Protótipo de alta fidelidade](https://www.figma.com/design/OkpO39vj7ImHyDWaKpwxHB/Prot%C3%B3tipo-Telas-de-Controle-do-Carrinho?node-id=0-1&p=f&t=gJBnpnv5p6toqXYq-0)
- ❌ Casos de teste
- ✅ [Matriz de rastreabilidade (Backward from)](https://github.com/PI1-2025-FCTE/2025.2-PI-Software-Docs/blob/main/casos-de-teste.md)

### Tarefas chave
- Conversar com o departamento de hardware para definir o formato das instruções;
- Desenvolver os entregáveis.

## Alocação da equipe

| Nome                                                   | Tarefas                                                                                                                 |
| ------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------- |
| [Eduardo Sandes](https://github.com/DiceRunner714)     | Casos de uso, MoSCow, Histórias de usuário, Arquitetura, DER, DLD, Fluxo de dados, Backward from, RNF's, Casos de teste |
| [André Gomes](https://github.com/AJCGassassin)         | BPMN, Diagrama de Estados, Protótipo de baixa fidelidade, Protótipo de alta fidelidade                                  |
| [Cássio Reis](https://github.com/csreis72)             | Casos de uso, MoSCow, BPMN, Arquitetura, Casos de teste, DER                                                            |
| [Guilherme Araujo](https://github.com/GFlyan)          | RNF's, Diagrama de Estados, Protótipo de alta, Histórias de usuário fidelidade                                          |
| [Márcio Costa](https://github.com/DeM4rcio)            | Casos de uso, RNF's, Arquitetura, Casos de teste                                                                        |
| [Yasmin Albuquerque](https://github.com/YasminDayrell) | Fluxo de dados, DER                                                                                                     |

---

## Sprint 3: Escrita do relatório 1
**Duração:** 7 dias  
**Início:** 06/10/2025  
**Término/Entrega:** 13/10/2025

### Entregáveis
- ✅ Relatório 1
    - ✅ Descrição do software
    - ✅ Objetivo do projeto
    - ✅ Justificativa
    - ❌ Indicadores
- ✅ [Casos de teste](https://github.com/PI1-2025-FCTE/2025.2-PI-Software-Docs/blob/main/casos-de-teste.md)
- ❌ Fluxo de dados
- ✅ Protótipo interativo

## Alocação da equipe

| Nome                                                   | Tarefas                                                           |
| ------------------------------------------------------ | ----------------------------------------------------------------- |
| [Eduardo Sandes](https://github.com/DiceRunner714)     | Descrição do software, Casos de teste, revisão final do relatório |
| [André Gomes](https://github.com/AJCGassassin)         | -                                                                 |
| [Cássio Reis](https://github.com/csreis72)             | Descrição do software, Casos de teste                             |
| [Guilherme Araujo](https://github.com/GFlyan)          | Protótipo interativo                                              |
| [Márcio Costa](https://github.com/DeM4rcio)            | Objetivo do projeto, Casos de teste, Justificativa                |
| [Yasmin Albuquerque](https://github.com/YasminDayrell) | Fluxo de dados, Indicadores                                       |

---

## Sprint 4: Setup de ambiente e Infraestrutura
**Duração:** 7 dias  
**Início:** 13/10/2025  
**Término/Entrega:** 20/10/2025

### Objetivos
- Criar os repositórios para o frontend e o backend
- Subir o docker em cada repositório
- Criar uma esteira de qualidade CI em ambos os repositórios

### Entregáveis
- ✅ Guias de contribuição
- ✅ Template issue
- ✅ Template PR
- ✅ [Repositório - 2025.2-PI-Front](https://github.com/PI1-2025-FCTE/2025.2-PI-Front)
    - ✅ Repositório criado
    - ✅ Estrutura do docker
    - ✅ Estrutura básica do Next.js 
    - ✅ CI
- ✅ [Repositório - 2025.2-PI-Service](https://github.com/PI1-2025-FCTE/2025.2-PI-Service)
    - ✅ Repositório criado
    - ✅ Estrutura do docker
    - ✅ Estrutura básica do FastAPI
    - ✅ Tabelas da base de dados criadas
    - ✅ Conexão com banco de dados
    - ✅ CI 
- ✅ [Fluxo de dados](https://github.com/PI1-2025-FCTE/2025.2-PI-Software-Docs/blob/main/assets/fluxo-de-dados.jpg)

## Alocação da equipe

| Nome                                                   | Tarefas                                                                                                                                  |
| ------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------- |
| [Eduardo Sandes](https://github.com/DiceRunner714)     | Estrutura do docker (frontend), Estrutura básica do FastAPI, Tabelas da base de dados criadas, Conexão com banco de dados, CI (frontend) |
| [André Gomes](https://github.com/AJCGassassin)         | -                                                                                                                                        |
| [Cássio Reis](https://github.com/csreis72)             | Estrutura do docker (backend), Estrutura básica do FastAPI, Tabelas da base de dados criadas, Conexão com banco de dados, CI (backend)   |
| [Guilherme Araujo](https://github.com/GFlyan)          | -                                                                                                                                        |
| [Márcio Costa](https://github.com/DeM4rcio)            | Guias de contribuição, Template issue, Template PR, Repositórios criados, Estrutura básica do Next.js                                    |
| [Yasmin Albuquerque](https://github.com/YasminDayrell) | Fluxo de dados                                                                                                                           |

---

## Sprint 5: Frontend completo e desenvolvimento da API
**Duração:** 7 dias  
**Início:** 20/10/2025  
**Término/Entrega:** 27/10/2025

### Objetivos
- Terminar as telas de acordo com o protótipo
- Criar os endpoints básicos da api
- Entender como implementar a comunicação com o hardware

### Entregáveis
- ✅ Telas do frontend
    - ✅ Instrução
    - ✅ Listagem
    - ✅ Detalhe
- ✅ Endpoints da API
- 🟡 Arquitetura validada (comunicação com a ESP32) 

## Alocação da equipe

| Nome                                                   | Tarefas                                        |
| ------------------------------------------------------ | ---------------------------------------------- |
| [Eduardo Sandes](https://github.com/DiceRunner714)     | Endpoints da API                               |
| [André Gomes](https://github.com/AJCGassassin)         | Telas: Detalhe, Testes                         |
| [Cássio Reis](https://github.com/csreis72)             | Endpoints da API                               |
| [Guilherme Araujo](https://github.com/GFlyan)          | Telas: Instrução, Listagem, Detalhe, Testes    |
| [Márcio Costa](https://github.com/DeM4rcio)            | Arquitetura validada (comunicação com a ESP32) |
| [Yasmin Albuquerque](https://github.com/YasminDayrell) | Telas: Instrução, Testes                       |

---

## Sprint 6: Testes, refatoração e pesquisa sobre a comunicação com hardware
**Duração:** 7 dias  
**Início:** 27/10/2025  
**Término/Entrega:** 03/11/2025

### Objetivos
- Finalizar mudanças arquiteturais
- Testar o código produzido

### Entregáveis
- ✅ Testes da API
- ❌ Testes do frontend
- ✅ Telas melhoradas
- ✅ Funcionalidade implementada: mapa das trajetórias
- ✅ Arquitetura refinada

### Tarefas chave
- Final UI/UX refinements
- Set up production infrastructure
- Create deployment runbooks
- Implement monitoring and alerting

## Alocação da equipe

| Nome                                                   | Tarefas              |
| ------------------------------------------------------ | -------------------- |
| [Eduardo Sandes](https://github.com/DiceRunner714)     | Testes da API        |
| [André Gomes](https://github.com/AJCGassassin)         | Mapa das trajetórias |
| [Cássio Reis](https://github.com/csreis72)             | Testes da API        |
| [Guilherme Araujo](https://github.com/GFlyan)          | Telas melhoradas     |
| [Márcio Costa](https://github.com/DeM4rcio)            | Arquitetura refinada |
| [Yasmin Albuquerque](https://github.com/YasminDayrell) | Testes do frontend   |

---

## Milestones

| Milestone | Target Date | Status |
|-----------|-------------|--------|
| 🎯 MVP Complete | End of Sprint 2 | 🟡 In Progress |
| 🎯 Beta Release | End of Sprint 4 | ⚪ Not Started |
| 🎯 Production Ready | End of Sprint 5 | ⚪ Not Started |
| 🎯 Public Launch | End of Sprint 6 | ⚪ Not Started |

---

## Status Legend
- ✅ **Completed** - Task is finished
- 🟢 **On Track** - Progressing as planned
- 🟡 **In Progress** - Currently being worked on
- 🟠 **At Risk** - May need attention
- 🔴 **Blocked** - Requires intervention
- ⚪ **Not Started** - Scheduled for future sprint

---

## Notes
- Each sprint includes a planning session (Monday) and retrospective (Friday)
- Daily standups at 10:00 AM
- Sprint reviews with stakeholders at end of each sprint
- Adjust timelines as needed based on project complexity

---

**Last Updated:** [Date]  
**Project Manager:** [Name]  
**Team Size:** [Number]