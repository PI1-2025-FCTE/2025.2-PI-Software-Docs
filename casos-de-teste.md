# Casos de Teste

Os testes de software com integração com o hardware têm como objetivo garantir a qualidade, segurança e funcionalidade de todo o sistema, evitando retrabalhos da equipe e permitindo criar novas funcionalidades sem perder o controle sobre implementações antigas.  
A seguir, são apresentados dois casos de teste para este projeto (*Iniciar Missão* e *Inserir Instruções*).  

---

## Caso de Teste 1: Iniciar a Missão

- **Nome:** Teste de Iniciar Missão  
- **Tipo:** Teste de Sistema / Teste Funcional  
- **Objetivo:** Verificar se o software é capaz de iniciar corretamente a Missão encarregada pelo carrinho, percorrer o trajeto completo pré-definido, coletar, transportar e entregar a carga frágil.

### Pré-condições
- O carrinho deve estar montado, com a bateria carregada e posicionado corretamente no ponto de partida demarcado.  
- A interface gráfica de monitoramento deve estar aberta e conectada à ESP.

### Descrição dos Procedimentos
- O operador envia o comando **"Iniciar Missão"** através da interface gráfica.  
- Observar o comportamento inicial do carrinho: ele deve ativar seus motores e sensores.  
- Verificar a execução do mecanismo de entrega da carga.  
- Acompanhar o transporte da carga até o ponto de entrega.

### Resultado Esperado
- O carrinho deve completar 100% do ciclo da missão de forma autônoma.  
- A carga deve ser entregue intacta, sem trincas ou danos.  
- O desvio da trajetória não deve exceder **±5 cm** do caminho definido.

### Especificação do Reparo (se o teste falhar)
- **Se o carrinho não iniciar:** verificar conexões de bateria, alimentação dos motores e comunicação com o software de controle.  
- **Se o carrinho sair da rota:** calibrar os sensores de linha/distância, ajustar parâmetros do controlador (PID) e revisar a lógica do algoritmo de navegação.

---

## Caso de Teste 2: Teste de Envio de Instruções

- **Nome:** Teste de Envio de Instruções via Interface  
- **Tipo:** Teste de Sistema  
- **Objetivo:** Validar se a interface gráfica consegue enviar comandos específicos para o carrinho e se o veículo responde corretamente a tais comandos.

### Pré-condições
- O carrinho deve estar ligado e posicionado em uma área de teste segura.  
- A conexão sem fio (Wi-Fi) entre a interface gráfica e o carrinho deve estar ativa e estável.

### Descrição dos Procedimentos
- Na interface gráfica, acionar o comando **"A15ED"**.  
- Quando aplicável, enviar um comando de emergência **"Parada Imediata"** enquanto o veículo está em movimento.

### Resultado Esperado
- Ao receber o comando **"A15ED"**, o carrinho deve:
  - mover-se para frente de forma contínua até 15 cm,  
  - virar à esquerda 90°,  
  - e depois virar à direita 90°.

### Especificação do Reparo (se o teste falhar)
- **Se o carrinho não responder aos comandos:** verificar o status da conexão sem fio e depurar o código de comunicação (na interface e no embarcado) para garantir que as mensagens estão sendo enviadas e recebidas corretamente.  
- **Se o carrinho executar comandos incorretos:** revisar a lógica de interpretação dos comandos no software embarcado para garantir que cada instrução seja mapeada corretamente às ações dos motores.
