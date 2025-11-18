# Descrição da Arquitetura

<!-- Descrição da arquitetura da solução de software proposta:
– Propósito do software (qual o seu papel no sistema);
– Estilo arquitetural contendo:
∗ Padrão adotado: MVC, MVP, Microsserviços, Monolítico, etc (Justificar);
∗ Linguagens de programação: Java, Python, C#, JavaScript, etc.
∗ Frameworks e bibliotecas: Spring Boot, .NET Core, React, Angular, Django,
etc.
∗ Banco de dados: Relacional (PostgreSQL, MySQL, etc) X NãoSQL (Mon-
goDB,etc).
Capítulo 4. Projeto Conceitual do Produto 18
– Diagrama de alto nível: representação esquemática dos componentes da arqui-
tetura, suas responsabilidades e comunicações, esclarecendo a composição do
front-end e do back-end. -->

## Propósito do Software

<div align="justify">&emsp;&emsp;
O Software proposto é uma plataforma web que atua como interface central para o controle, monitoramento e análise do carrinho autônomo equipado com um sistema embarcado ESP32. As principais funcnionalidades incluem: planejamento detalhado de rotas, o envio de missões ao veículo, o acompanhamento de sua posição e a análise dos dados coletados durante as missões.
</div>

---

## Estilo Arquitetural

<div align="justify">&emsp;&emsp;
A solução proposta adota o padrão arquitetural Cliente-Servidor, que estabelece separação das responsabilidades entre os diferentes componentes do sistema. Esta escolha foi fundamentada na necessidade de centralizar a lógica de negócio na camada de backend (servidor) enquanto mantém uma interface de usuário leve e responsiva no frontend (cliente). Tais escolhas se justificam pelos seguintes motivos:
</div>

1. **Separação de responsabilidades:** O backend gerencia toda a comunicação TCP com intermediação de um broker com a ESP32, valida os comandos, realiza cálculos de trajetória e faz a persistência de dados, enquanto o frontend se concentra exclusivamente na experiência do usuário.

2. **Escalabilidade:** A arquitetura permite que múltiplos clientes (navegadores) acessem o mesmo backend sem gerar conflitos.

<div align="justify">&emsp;&emsp;
O frontend consiste em uma aplicação web desenvolvida em React com TypeScript, executada no navegador do usuário. Esta camada é responsável por toda a interação com o usuário, incluindo:
</div>

- Interface gráfica para criação de trajetórias
- Visualização de status de conexão
- Renderização de gráficos de trajetória
- Exibição de histórico de trajetórias

<div align="justify">&emsp;&emsp;
A comunicação entre o frontend e o backend ocorre exclusivamente através de protocolo HTTP/HTTPS para requisições REST.
</div>

<div align="justify">&emsp;&emsp;
O backend, implementado em Python utilizando o framework FastAPI, funciona como o núcleo da aplicação. Suas responsabilidades incluem:
</div>

### REST API
- Expor endpoints HTTP para o frontend  
- Validar requisições e parâmetros  
- Publicar e inscrever-se em dados na fila usando protocolo MQTT  
- Retornar respostas formatadas em JSON  

### Eclipse Mosquitto
- Broker responsável pela comunicação entre os serviços da ESP32 e o backend  

### ESP32 Service (TCP Client)
- Estabelecer e manter conexões TCP com o broker  
- Implementar protocolo de comunicação binário/ASCII  
- Gerenciar timeouts e reconexões  
- Detectar perda de conexão (RNF09)  
- Codificar comandos de alto nível para o protocolo da ESP32  
- Decodificar respostas enviadas pela ESP32

<div align="justify">&emsp;&emsp;
O PostgreSQL foi escolhido como sistema de gerenciamento de banco de dados devido à sua robustez, conformidade com padrões SQL e suporte nativo a tipos de dados JSON. O backend se comunica com o banco através de um ORM (Object-Relational-Mapping), facilitando operações de CRUD e garantindo a integridade dos dados.
</div>

<div align="justify">&emsp;&emsp;
ESP32 atua como um cliente/servidor TCP que publica status e trajetos, além de assinar os dados dos comandos enviados pelo backend no broker de comunicação. Da mesma forma, o backend, também atuando como cliente/servidor, publica apenas os comandos que devem ser executados pelo ESP32 e se inscreve nos tópicos de status e trajetos.
</div>





## Diagrama de alto nível

<center>

![DiagramaAltoNivel](assets/diagrama-arquitetura.png)

</center>