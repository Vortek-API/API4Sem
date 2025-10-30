# **DESCRIÇÃO DO PRODUTO**

O sistema proposto visa a manipulação e análise de dados de radares de trânsito de São José dos Campos, permitindo a visualização de informações em tempo real por meio de dashboards interativos. Será construído sobre um banco de dados relacional, com API RESTful em Spring Boot e atualizações via WebSocket, garantindo acesso seguro e eficiente. A interface em Vue.js será responsiva e intuitiva, integrando gráficos e mapas georreferenciados, permitindo monitoramento de indicadores, disparo de alertas automáticos facilitando a tomada de decisão na gestão do tráfego urbano.

---

<div align="center">

<div style="display: flex; justify-content: center; align-items: center; flex-direction: column; min-height: 100vh; gap: 20px;">

  <!-- Requisitos Funcionais -->
  <table border="1" cellpadding="8" style="border-collapse: collapse;">
<tr>
  <th><strong>Requisitos Funcionais (RF)</strong></th>
  </tr>
  <tr><td>Tratamento dos dados</td></tr>
  <tr><td>Criação de indicadores de acompanhamento de tráfego na cidade</td></tr>
  <tr><td>Criação de níveis de monitoramento</td></tr>
  <tr><td>Dashboard que demonstre o tráfego de forma simples e lúdica, de preferência com georreferenciamento</td></tr>
  <tr><td>Sugestões de dados externos que possam complementar a avaliação</td></tr>
  <tr><td>Criação de sistema de alertas, que permita a notificação e acionamento de protocolos</td></tr>
  </table>
  
<br>
<br>

  <!-- Requisitos Não Funcionais -->
  <table border="1" cellpadding="8" style="border-collapse: collapse;">
    <tr>
      <th><strong>Requisitos Não Funcionais (RNF)</strong></th>
    </tr>
    <tr><td>Manual de Instalação</td></tr>
    <tr><td>Manual do Usuário detalhado</td></tr>
    <tr><td>Documentação API – Application Programming Interface</td></tr>
    <tr><td>Modelagem de Banco de Dados ou Arquivo de Dados</td></tr>
    <tr><td>Operacional em cloud</td></tr>
    <tr><td>Padrões de arquitetura modular e injeção de dependências (Spring Boot)</td></tr>
    <tr><td>Interface intuitiva e responsiva (Vue.js)</td></tr>
  </table>

</div>
</div>

---

# TECNOLOGIAS UTILIZADAS

<p align="center">
<img src="https://go-skill-icons.vercel.app/api/icons?i=java,vue,nuxt,oracle,git,github,figma,vscode,spring,docker,redis" width="600" />
</p>

---
# O PRODUTO

<details>
<summary>Backlog</summary>

| Ranking | Sprint  | User Story | Prioridade | Estimativa (pts) |
|---------|---------|------------|------------|-----------------|
| 1       |  1 | Como cliente, quero cadastrar indicadores de tráfego para monitoramento automático para poder acompanhar o desempenho da cidade. | Alta | 8 |
| 2       |  1 | Como sistema, quero processar e tratar os dados de tráfego para que fiquem prontos para análise para fornecer informações confiáveis aos usuários. | Alta | 6 |
| 3       |  1 | Como cliente, quero calcular o nível geral de tráfego da cidade e por regiões para identificar áreas críticas. | Alta | 8 |
| 4       |  1 | Como cliente, quero autenticar-me no sistema para acessar minhas informações de forma segura para proteger meus dados pessoais. | Alta | 5 |
| 5       |  1 | Como cliente, quero registrar histórico de criação e atualização dos indicadores para manter rastreabilidade das alterações. | Média | 3 |
| 6       |  1 | Como cliente, quero visualizar indicadores no mapa em tempo real, incluindo pings representando radares para monitorar a situação do tráfego instantaneamente. | Média | 8 |
| 7       |  2 | Como cliente, quero carregar as rotas e horários da frota de ônibus para que estejam disponíveis no sistema para consulta e planejamento. | Alta | 3 |
| 8       |  2 | Como cliente, quero classificar o tráfego em níveis automáticos com base nos dados para fornecer informações imediatas e confiáveis aos usuários. | Alta | 8 |
| 9       |  2 | Como cliente, quero que os dados carregados da frota de ônibus estejam integrados aos indicadores específicos no dashboard para ter uma visão completa do tráfego. | Média | 6 |
| 10      |  2 | Como cliente, quero visualizar gráficos de velocidade de tráfego de ônibus e carros para entender a fluidez do trânsito. | Média | 5 |
| 11      |  2 | Como cliente, quero pesquisar por endereço ou ponto de ônibus no mapa para encontrar rapidamente minha rota. | Baixa | 5 |
| 12      |  3 | Como cliente, quero enviar alertas automáticos quando os indicadores ultrapassarem limites para que o cliente seja notificado e possa tomar decisões. | Alta | 8 |
| 13      |  3 | Como cliente, quero visualizar indicadores no mapa em tempo real, incluindo pings representando radares para monitorar a situação do tráfego instantaneamente. | Alta | 8 |
| 14      |  3 | Como cliente, quero responder aos alertas e que o sistema registre logs completos de envio, resposta e encerramento para garantir rastreabilidade das ações. | Média | 8 |
| 15      |  3 | Como cliente, quero receber sugestões de dados externos que possam complementar a análise do tráfego para ter insights mais completos. | Baixa | 5 |
| 16      |  3 | Como cliente, quero visualizar um mapa da cidade com cores indicando níveis de tráfego por região para identificar rapidamente áreas congestionadas. | Baixa | 5 |

</details>

---

<details>
<summary>Sprint 1</summary>

# Backlog da Sprint 1
<div align="center">
<div style="display: flex; justify-content: center; align-items: center; flex-direction: column; min-height: 100vh; gap: 20px;">

| Ranking | Sprint  | User Story | Prioridade | Estimativa (pts) |
|---------|---------|------------|------------|-----------------|
| 1       |  1 | Como cliente, quero cadastrar indicadores de tráfego para monitoramento automático para poder acompanhar o desempenho da cidade. | Alta | 8 |
| 2       |  1 | Como cliente, quero processar e tratar os dados de tráfego para que fiquem prontos para análise para fornecer informações confiáveis aos usuários. | Alta | 6 |
| 3       |  1 | Como cliente, quero calcular o nível geral de tráfego da cidade e por regiões para identificar áreas críticas. | Alta | 8 |
| 4       |  1 | Como cliente, quero autenticar-me no sistema para acessar minhas informações de forma segura para proteger meus dados pessoais. | Alta | 5 |
| 5       |  1 | Como sistema, quero registrar histórico de criação e atualização dos indicadores para manter rastreabilidade das alterações. | Média | 3 |
| 6       |  1 | Como cliente, quero visualizar indicadores no mapa em tempo real, incluindo pings representando radares para monitorar a situação do tráfego instantaneamente. | Média | 8 |

</div>
</div>

<br>
<br>

<div align="center">
<div style="display: flex; justify-content: center; align-items: center; flex-direction: column; min-height: 100vh; gap: 20px;">

### Sprint 1 – Organização
  
| Critério | Sprint |
|----------|--------|
| Capacidade estimada da Equipe por Sprint: | 38 story points |
| Meta da Sprint: | US de ranking 1, 2, 3, 4 (27 story points) |
| Previsão da Sprint (extras, sem compromisso de entrega) | US de ranking 1, 5, 6 (11 story points) |


</div>
</div>

### Sprint 1 – DoR e DoD

<div align="center">
<div style="display: flex; justify-content: center; align-items: center; flex-direction: column; min-height: 100vh; gap: 20px;">

| Ranking | DoR | DoD |
|---------|-----|-----|
| 1 | Requisitos de acompanhamento de tráfego definidos pelo cliente | Indicadores cadastrados corretamente com todos os campos obrigatórios preenchidos e visíveis no sistema |
| 2 | Dados de tráfego disponíveis para tratamento e análise | Dados tratados, validados e prontos para visualização no dashboard |
| 3 | Critérios para cálculo de níveis gerais e por região definidos | Dashboard mostra claramente os níveis gerais e por região, com informações confiáveis |
| 4 | Cliente com credenciais válidas | Autenticação realizada com sucesso e acesso seguro às informações pessoais |
| 5 | Histórico de indicadores definido | Logs armazenados corretamente com usuário, data e ação realizada |
| 6 | Indicadores e posições de radares disponíveis | Mapa atualizado em tempo real com pings representando radares e indicadores visíveis |

</div>
</div>


</details>

---

<details>
<summary>Sprint 2</summary>

# Backlog da Sprint 2
<div align="center">
<div style="display: flex; justify-content: center; align-items: center; flex-direction: column; min-height: 100vh; gap: 20px;">

| Ranking | Sprint | User Story | Prioridade | Estimativa (pts) |
|---------|--------|------------|------------|-----------------|
| 7       |  2 | Como cliente, quero carregar as rotas e horários da frota de ônibus para que estejam disponíveis no sistema para consulta e planejamento. | Alta | 3 |
| 8       |  2 | Como cliente, quero classificar o tráfego em níveis automáticos com base nos dados para fornecer informações imediatas e confiáveis aos usuários. | Alta | 8 |
| 9       |  2 | Como cliente, quero que os dados carregados da frota de ônibus estejam integrados aos indicadores específicos no dashboard para ter uma visão completa do tráfego. | Média | 6 |
| 10      |  2 | Como cliente, quero visualizar gráficos de velocidade de tráfego de ônibus e carros para entender a fluidez do trânsito. | Média | 5 |
| 11      |  2 | Como cliente, quero pesquisar por endereço ou ponto de ônibus no mapa para encontrar rapidamente minha rota. | Baixa | 5 |

</div>
</div>

<br>
<br>

<div align="center">
<div style="display: flex; justify-content: center; align-items: center; flex-direction: column; min-height: 100vh; gap: 20px;">

## Sprint 2 – Organização
  
| Critério | Sprint |
|----------|--------|
| Capacidade estimada da Equipe por Sprint: | 27 story points |
| Meta da Sprint: | US de ranking 7, 9, 10 (16 story points) |
| Previsão da Sprint (extras, sem compromisso de entrega) | US de ranking 8, 11 (11 story points) |

</div>
</div>

<br>
<br>

### Sprint 2 – DoR e DoD (por US)

<div align="center">
<div style="display: flex; justify-content: center; align-items: center; flex-direction: column; min-height: 100vh; gap: 20px;">

#  DoR e DoD — Sprint 2


| **Ranking** | **DoR (Definition of Ready)** | **DoD (Definition of Done)** |
|:--:|:--|:--|
| **7**<br>_Carregar rotas e horários da frota_ | - Diagrama do banco de dados atualizado e validado pelo backend, com tabelas de **rotas** e **horários**.<br>- Estrutura das tabelas definida (`route_id`, `bus_line`, `departure_time`, `arrival_time`).<br>- Script de carga planejado, com formato dos arquivos (CSV/JSON) e exemplos reais.<br>- Protótipo da interface de pesquisa e visualização aprovado.<br>- Critérios de aceitação definidos: consulta deve retornar linha, horários e paradas sem duplicar dados.<br>- Acesso ao banco de teste liberado.<br>- Dependências e endpoints mapeados. | - Diagrama do BD alterado e versionado.<br>- Tabela criada com migrations documentadas.<br>- Script de importação funcionando e registrando logs.<br>- Backend enviando dados pro front seguindo padrões do projeto.<br>- Front exibe rotas e horários corretamente; busca por linha operando.<br>- Testes unitários e de integração aprovados.<br>- QA validou com dados reais.<br>- Documentação técnica atualizada (modelo, endpoints, payloads).<br>- Manual de uso pronto.<br>- Logs de import salvos e monitorados.<br>- PR revisado e deploy feito em staging. |
| **8**<br>_Classificar o tráfego automaticamente_ | - Fontes de dados de tráfego disponíveis e validadas.<br>- Regras de classificação documentadas (ex: leve = até 40 km/h, moderado = 20 km/h, intenso = 10 km/h).<br>- Padrão de cores e ícones definidos com design.<br>- Mockup do dashboard mostrando o status de tráfego.<br>- Frequência de atualização automática definida (ex: a cada 5 min). | - Classificação automática implementada e atualizando em tempo real.<br>- Cores e legendas aplicadas conforme padrão.<br>- Backend calcula níveis com base nos dados de velocidade e envia ao front sem delay.<br>- Testes unitários e de integração feitos, cobrindo casos extremos.<br>- Dashboard atualiza sozinho, sem recarregar.<br>- Logs e métricas funcionando.<br>- Documentação do algoritmo e dos níveis publicada.<br>- PO testou e confirmou resultados corretos. |
| **9**<br>_Integrar dados da frota aos indicadores do dashboard_ | - Indicadores que usarão dados da frota definidos (ex: velocidade média, total de ônibus ativos).<br>- Mapeamento de origem dos dados e frequência de atualização definidos.<br>- Mockup do dashboard atualizado com cards reservados.<br>- Dados da frota testados e validados. | - Indicadores aparecem no dashboard integrados aos demais.<br>- Backend calcula e envia dados corretamente.<br>- Valores dos indicadores conferem com dados reais.<br>- Front adaptado e responsivo.<br>- Testes unitários e de integração realizados.<br>- Logs registrando erros e tempos de atualização.<br>- Documentação técnica revisada.<br>- PO validou o dashboard e aprovou a integração. |
| **10**<br>_Visualizar gráficos de velocidade (ônibus e carros)_ | - Dados de velocidade disponíveis (histórico e em tempo real).<br>- Tipo de gráfico (linha/área) e filtros definidos (tipo de veículo, horário, região).<br>- Mockup da tela validado com PO.<br>- Endpoint para puxar dados de velocidade documentado.<br>- Critério de aceitação: atualização automática e carregamento < 3s. | - Tela de dashboard criada e seguindo padrões do sistema.<br>- Backend implementa cálculos e agrega velocidades corretamente.<br>- Gráficos mostram ônibus e carros com legendas e tooltips.<br>- Atualização automática funcionando (ex: a cada 1 min).<br>- Testes unitários e manuais validados.<br>- Documentação técnica pronta (cálculos + endpoint).<br>- PO aprovou a visualização e valores exibidos. |
| **11**<br>_Pesquisar por endereço ou ponto de ônibus no mapa_ | - Base de endereços e pontos de ônibus validada (`lat`, `lon`, `address`, `route_id`).<br>- API de geolocalização configurada e chave liberada.<br>- Mockup da busca revisado com UX.<br>- Casos de teste definidos (endereço exato, parcial, inexistente, ponto específico). | - Pings dos pontos de ônibus aparecem corretamente no mapa.<br>- Barra de pesquisa retorna endereços e pontos, centralizando o mapa no resultado.<br>- Resposta rápida (< 2s) e feedback visual pro usuário.<br>- Testes unitários e integração da API de geolocalização aprovados.<br>- Validação manual com diferentes tipos de busca.<br>- Documentação atualizada (estrutura da base + funcionamento da busca).<br>- Logs de pesquisa ativos.<br>- PO validou e aprovou a usabilidade. |


</div>
</div>

</details>

---

<details>
<summary>Sprint 3</summary>

# Backlog da Sprint 3
<div align="center">
<div style="display: flex; justify-content: center; align-items: center; flex-direction: column; min-height: 100vh; gap: 20px;">

| Ranking | Sprint | User Story | Prioridade | Estimativa (pts) |
|---------|---------|------------|------------|-----------------|
| 12 | 3 | Como cliente, quero enviar alertas automáticos quando os indicadores ultrapassarem limites para que o cliente seja notificado e possa tomar decisões. | Alta | 8 |
| 13 | 3 | Como cliente, quero visualizar indicadores no mapa em tempo real, incluindo pings representando radares para monitorar a situação do tráfego instantaneamente. | Alta | 8 |
| 14 | 3 | Como cliente, quero responder aos alertas e que o sistema registre logs completos de envio, resposta e encerramento para garantir rastreabilidade das ações. | Média | 8 |
| 15 | 3 | Como cliente, quero receber sugestões de dados externos que possam complementar a análise do tráfego para ter insights mais completos. | Baixa | 5 |
| 16 | 3 | Como cliente, quero visualizar um mapa da cidade com cores indicando níveis de tráfego por região para identificar rapidamente áreas congestionadas. | Baixa | 5 |


</div>
</div>

<br>
<br>

<div align="center">
<div style="display: flex; justify-content: center; align-items: center; flex-direction: column; min-height: 100vh; gap: 20px;">

## Sprint 3 – Organização
  
| Critério | Sprint |
|----------|--------|
| Capacidade estimada da Equipe por Sprint: | 34 story points |
| Meta da Sprint: | US de ranking 12, 13, 14 (24 story points) |
| Previsão da Sprint (extras, sem compromisso de entrega) | US de ranking 15, 16 (10 story points) |

</div>
</div>

<br>
<br>

### Sprint 3 – DoR e DoD (por US)

<div align="center">
<div style="display: flex; justify-content: center; align-items: center; flex-direction: column; min-height: 100vh; gap: 20px;">

#  DoR e DoD — Sprint 3

| **Ranking** | **DoR (Definition of Ready)** | **DoD (Definition of Done)** |
|:--:|:--|:--|
| **12**<br>_Enviar alertas automáticos ao ultrapassar limites (incluindo envio via Telegram)_ | - Limites de cada indicador definidos e documentados (ex: velocidade, fluxo, tempo de congestionamento).<br>- Tipos de alerta configurados (e-mail, notificação no sistema e Telegram).<br>- Bot do Telegram criado e configurado com token de acesso e webhook ativo.<br>- Regras de disparo e mensagens padronizadas documentadas.<br>- Critérios de aceitação definidos: alerta deve ser enviado imediatamente após o limite ser ultrapassado, em todos os canais configurados.<br>- Endpoint de integração com o Telegram documentado e testado no ambiente. | - Regras de alerta implementadas e funcionando em tempo real.<br>- Notificações enviadas corretamente por e-mail, sistema e Telegram.<br>- Logs de envio registrados com status e horário de disparo.<br>- Mensagens do Telegram formatadas com título, indicador, valor e link direto para o dashboard.<br> |
| **13**<br>_Visualizar indicadores no mapa em tempo real (com radares/pings)_ | - Fonte de dados em tempo real confirmada e testável.<br>- Padrão visual dos pings e cores definido com o time de design.<br>- Atualização automática implementada sem recarregar a página.<br>- Legenda e cores aplicadas corretamente conforme o padrão de design.<br>- Logs de atualização armazenados.<br>- Documentação e endpoints revisados e aprovados. | - Indicadores exibidos corretamente no mapa em tempo real.<br>- Pings atualizados dinamicamente conforme os dados recebidos.<br>- Legenda e cores apresentadas de forma consistente com o padrão visual.<br>- Atualização fluida e sem recarregar a página.<br>- Logs de atualização registrados e acessíveis para auditoria.<br> |
| **14**<br>_Responder aos alertas e registrar logs completos_ | - Estrutura de logs definida (`alert_id`, `user_id`, `status`, `timestamp`, `response`).<br>- Fluxo de resposta a alertas mapeado (abrir, responder, encerrar).<br>- Critérios de aceitação definidos: todas as ações precisam ser rastreáveis.<br>- Acesso ao ambiente de logs configurado e testado.<br>- Integração com o sistema de autenticação confirmada. | - Sistema registra logs completos de todo o ciclo de vida do alerta.<br>- Ações de resposta salvas e exibidas no painel administrativo.<br>- Backend armazena logs com timestamps corretos.<br>- Testes unitários e de integração validados.<br>- Logs exportáveis em CSV/JSON.<br> |
| **15**<br>_Receber sugestões de dados externos para análise_ | - Fontes externas de dados definidas (ex: Waze, Google Traffic, sensores municipais, APIs públicas de mobilidade).<br>- Critérios para sugestão de dados documentados (tipo, relevância, frequência de atualização).<br>- Mockup da interface de sugestões revisado com PO.<br>- Casos de teste definidos (dados válidos, inválidos e indisponíveis). | - Sugestões externas exibidas corretamente no dashboard.<br>- Backend coleta e trata dados externos com sucesso.<br>- Sistema filtra e mostra apenas dados relevantes.<br>- Logs de integração e erros armazenados.<br> |
| **16**<br>_Visualizar mapa com cores indicando níveis de tráfego por região_ | - Mapa base da cidade configurado e carregando corretamente.<br>- Padrão de cores definido com design (verde, amarelo, vermelho, azul, roxo).<br>- Regras de classificação por nível documentadas (ex: leve, moderado, intenso, crítico).<br>- Critério de aceitação: atualização automática e fluida, sem travamentos. | - Mapa clicável colorido exibindo níveis de tráfego por região em tempo real.<br>- Backend calcula níveis e envia dados corretamente via API.<br>- Cores e legendas aplicadas conforme padrão visual aprovado.<br>- Atualização automática validada e otimizada.<br> |


</div>
</div>

</details>

---

# **TIME VORTEK**
<div align="center">

<div style="display: flex; justify-content: center; align-items: center; flex-direction: column; min-height: 100vh; gap: 20px;">
<img width="1219" height="689" alt="image" src="https://github.com/user-attachments/assets/f0f57506-cad6-41f7-b09f-56e35142531d" />


---

# Requisitos de Permanência do Grupo

1. **Comprometimento com as Reuniões**  
   Faltas nas reuniões semanais só serão aceitas com justificativa válida. A participação regular é fundamental.

2. **Responsabilidades de Aprendizado e Desenvolvimento**  
   Todos devem cumprir tarefas e entregas conforme o planejado. O Scrum Master fornecerá material de apoio.

3. **Manutenção dos Cards no Jira**  
   Todos os membros devem manter os cards atualizados para refletir o progresso.

4. **Comunicação Efetiva**  
   Utilize canais como WhatsApp, Slack ou encontros presenciais para manter todos informados.

5. **Cumprimento de Prazos**  
   É essencial cumprir os prazos estabelecidos para garantir o fluxo do projeto.

---
