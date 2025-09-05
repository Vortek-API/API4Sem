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
<img src="https://go-skill-icons.vercel.app/api/icons?i=java,vue,nuxt,oracle,git,github,figma,vscode,spring" width="600" />
</p>

---
# O PRODUTO

<details>
<summary>Backlog</summary>

| Ranking   | Sprint | User Story | Critérios de Aceitação | Prioridade | Estimativa (pts) | Requisito do Cliente |
|------|--------|------------|----------------------|------------|-----------------|--------------------|
| 1 | Sprint 1 | Como cliente, quero cadastrar indicadores de tráfego para monitoramento automático. | Indicadores cadastrados corretamente com todos os campos obrigatórios preenchidos. | Alta | 5 | Criação de indicadores de acompanhamento de tráfego na cidade |
| 2 | Sprint 1 | Como sistema, quero processar e tratar os dados de tráfego para que fiquem prontos para análise. | Dados tratados e disponíveis para visualização no dashboard. | Alta | 8 | Tratamento dos dados |
| 3 | Sprint 1 | Como cliente, quero visualizar o nível geral de tráfego da cidade e por regiões. | Dashboard mostra claramente os níveis gerais e por região. | Alta | 8 | Criação de níveis de monitoramento |
| 4 | Sprint 1 | Como cliente, quero visualizar um mapa da cidade com cores indicando níveis de tráfego por região. | Mapa colorido de acordo com os níveis, atualizado com os dados disponíveis. | Média | 5 | Dashboard com georreferenciamento |
| 5 | Sprint 1 | Como sistema, quero registrar logs de criação e atualização dos indicadores. | Logs armazenados com usuário, data e ação realizada. | Média | 3 | Registro de dados para auditoria |
| 6 | Sprint 2 | Como cliente, quero cadastrar dados de tráfego de ônibus. | Inserção de rotas e horários realizada; dados disponíveis para análise. | Alta | 5 | Criação de indicadores de tráfego |
| 7 | Sprint 2 | Como sistema, quero classificar o tráfego em níveis automáticos com base nos dados. | Sistema classifica corretamente o tráfego em Intenso, Moderado, Ok ou Suspeito. | Alta | 8 | Criação de níveis de monitoramento |
| 8 | Sprint 2 | Como cliente, quero visualizar gráficos de velocidade de tráfego de ônibus e carros. | Dashboard mostra gráficos claros e fáceis de interpretar. | Alta | 5 | Dashboard simples e lúdico |
| 9 | Sprint 2 | Como cliente, quero pesquisar por endereço ou ponto de ônib  no mapa. | Campo de b ca retorna a localização correta e exibe dados relacionados. | Média | 5 | Dashboard com georreferenciamento |
| 10 | Sprint 2 | Como sistema, quero enviar alertas automáticos quando os indicadores ultrapassarem limites. | Alertas disparados automaticamente; mensagem vinculada ao protocolo de ação. | Alta | 10 | Sistema de alertas acionando protocolos |
| 11 | Sprint 3 | Como cliente, quero visualizar os alertas recebidos e stat  dos chamados. | Tela exibe lista de alertas com stat  aberto, respondido ou encerrado. | Alta | 5 | Sistema de alertas |
| 12 | Sprint 3 | Como cliente, quero responder aos alertas e que o sistema registre a resposta. | Resposta registrada corretamente; stat  do alerta atualizado; log gerado. | Alta | 10 | Sistema de alertas acionando protocolos |
| 13 | Sprint 3 | Como sistema, quero armazenar logs de envio, resposta e encerramento dos alertas. | Logs persistidos corretamente com todas as informações necessárias. | Alta | 5 | Registro de dados para auditoria |
| 14 | Sprint 3 | Como cliente, quero visualizar histórico de alertas e ações tomadas. | Dashboard mostra histórico completo com filtros por período. | Média | 8 | Sistema de alertas e monitoramento histórico |
| 15 | Sprint 3 | Como cliente, quero visualizar indicadores no mapa em tempo real, incluindo pings representando radares. | Mapa atualizado em tempo real com informações visuais de tráfego. | Alta | 8 | Dashboard com georreferenciamento |
| 16 | Sprint 3 | Como cliente, quero receber sugestões de dados externos que possam complementar a análise do tráfego. | Sugestões apresentadas de forma clara, permitindo avaliar possíveis integrações futuras. | Média | 5 | Sugestões de dados externos |


</details>

---

<details>
<summary>Sprint 1</summary>

# Backlog da Sprint 1

| Ranking   | Sprint   | User Story | Critérios de Aceitação | Prioridade | Estimativa (pts) | Requisito do Cliente |
|------|----------|------------|----------------------|------------|-----------------|--------------------|
| 1 | Sprint 1 | Como cliente, quero cadastrar indicadores de tráfego para monitoramento automático. | Indicadores cadastrados corretamente com todos os campos obrigatórios preenchidos; possibilidade de cadastrar múltiplos indicadores. | Alta | 5 | Criação de indicadores de acompanhamento de tráfego na cidade |
| 2 | Sprint 1 | Como sistema, quero processar e tratar os dados de tráfego para que fiquem prontos para análise. | Dados tratados e disponíveis para visualização no dashboard; atualização automática sempre que novos indicadores forem cadastrados ou alterados. | Alta | 8 | Tratamento dos dados |
| 3 | Sprint 1 | Como cliente, quero visualizar o nível geral de tráfego da cidade e por regiões. | Dashboard mostra claramente os níveis gerais e por região; atualização automática sempre que houver alteração de indicadores. | Alta | 8 | Criação de níveis de monitoramento |
| 4 | Sprint 1 | Como cliente, quero visualizar um mapa da cidade com cores indicando níveis de tráfego por região. | Mapa colorido de acordo com os níveis de tráfego; todas as regiões cadastradas estão representadas; atualização automática a cada alteração de indicador. | Média | 5 | Dashboard com georreferenciamento |
| 5 | Sprint 1 | Como sistema, quero registrar logs de criação e atualização dos indicadores. | Logs armazenados corretamente com usuário, data e ação realizada; todos os indicadores cadastrados ou alterados devem gerar log. | Média | 3 | Registro de dados para auditoria |

<br>
<br>

<div align="center">
<div style="display: flex; justify-content: center; align-items: center; flex-direction: column; min-height: 100vh; gap: 20px;">

  
| Critério| Sprint 
|------|-------------
| Capacidade estimada da Equipe por Sprint: |--------| 
| Meta da Sprint: |--------|
|Previsão da Sprint (extras, sem compromisso de entrega)| --------| 
</div>
</div>


</details>

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
