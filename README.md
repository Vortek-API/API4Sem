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


| Ranking | DoR | DoD |
|---------|-----|-----|
| 7 | Estrutura de dados da frota disponível; acesso ao banco de horários | Rotas e horários carregados corretamente no sistema, visíveis e pesquisáveis |
| 8 | Dados da frota carregados e validados | Indicadores no dashboard refletem corretamente os dados da frota, integrados aos demais indicadores de tráfego |
| 9 | Regras de classificação de tráfego definidas | Tráfego classificado automaticamente em níveis, com atualizações visíveis no dashboard em tempo real |
| 10 | Dados de velocidade de ônibus e carros disponíveis | Gráficos de velocidade de tráfego gerados corretamente, permitindo comparação e análise da fluidez |
| 11 | Base de endereços e pontos de ônibus disponível no mapa | Funcionalidade de busca implementada; pesquisa retorna resultados corretos e destacados no mapa |

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
