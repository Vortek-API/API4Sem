# API4Sem

Parent repo

---

# **DESCRIÇÃO DO PRODUTO**

Projeto de análise de dados coletados pelos radares de trânsito da cidade de São José dos Campos.  
O objetivo é construir indicadores e, a partir destes, estabelecer padrões de definição dos níveis de eficiência, ou não, da gestão de trânsito na cidade.

---

# TECNOLOGIAS UTILIZADAS

<p align="center">
  <img src="https://skillicons.dev/icons?i=java&color=green" width="50" />
  <img src="https://skillicons.dev/icons?i=vue&color=green" width="50" />
  <img src="https://skillicons.dev/icons?i=github&color=green" width="50" />
  <img src="https://skillicons.dev/icons?i=vscode&color=green" width="50" />
  <img src="https://skillicons.dev/icons?i=git&color=green" width="50" />
  <img src="https://skillicons.dev/icons?i=figma&color=green" width="50" />
  <img src="https://skillicons.dev/icons?i=oracle&color=green" width="50" />
  <img src="https://raw.githubusercontent.com/tandpfun/skill-icons/main/icons/Spring-Dark.svg" width="50" />
</p>

---

# O PRODUTO

<details>
<summary>Product Backlog</summary>

| ID  | Sprint Envolvidas | User Story | Critérios de Aceitação | Prioridade | Estimativa (pts) | Requisito do Cliente |
|-----|------------------|------------|-----------------------|------------|-----------------|--------------------|
| US01 | Sprint 1 | Como gestor, quero cadastrar indicadores no sistema para que sejam usados no monitoramento automático. | Inserção de indicadores com nome, unidade, limite e tipo; validação obrigatória; persistência no banco. | Alta | 5 | Criação de indicadores |
| US02 | Sprint 1 | Como sistema, quero processar os dados armazenados no banco relacional para disponibilizar via API. | API RESTful em Spring Boot com endpoints GET/POST/PUT/DELETE; retorno em JSON. | Alta | 8 | Manipulação de dados no banco |
| US03 | Sprint 1 | Como gestor, quero visualizar em uma dashboard inicial os níveis gerais da cidade e por regiões. | Dashboard com status geral, blocos por região e cores de alerta; integração via API. | Alta | 8 | Dashboard com níveis |
| US04 | Sprint 1 | Como gestor, quero visualizar um mapa da cidade com cores por região. | Mapa Leaflet integrado, regiões coloridas conforme níveis da API. | Média | 5 | Georreferenciamento |
| US05 | Sprint 1 | Como sistema, quero registrar logs de criação e atualização de indicadores para auditoria. | Logs salvos no banco com usuário, data e ação. | Média | 3 | Registro de logs |
| US06 | Sprint 2 | Como gestor, quero cadastrar dados de tráfego de ônibus. | Inserção de rota, velocidade média e horários no banco Oracle. | Alta | 5 | Indicadores de ônibus |
| US07 | Sprint 2 | Como sistema, quero calcular velocidade média e classificar trânsito em níveis. | API retorna status calculado (Intenso, Moderado, Ok, Suspeito). | Alta | 8 | Níveis de monitoramento |
| US08 | Sprint 2 | Como gestor, quero visualizar gráficos de velocidade de ônibus e carros. | Dashboard com Chart.js; dados da API atualizados. | Alta | 5 | Dashboard lúdico |
| US09 | Sprint 2 | Como gestor, quero pesquisar no mapa por endereço/ponto de ônibus. | Campo de busca; mapa retorna localização e dados relacionados. | Média | 5 | Pesquisa por endereço |
| US10 | Sprint 2 | Como sistema, quero enviar alertas automáticos no WhatsApp quando indicadores ultrapassarem limites. | Integração com API de mensagens; envio com texto e protocolo. | Alta | 13 | Sistema de alertas |
| US11 | Sprint 3 | Como gestor, quero receber alertas no painel e visualizar status dos chamados. | Tela com lista de alertas, status (aberto, respondido, encerrado). | Alta | 5 | Monitoramento de status |
| US12 | Sprint 3 | Como gestor, quero responder ao alerta via WhatsApp e que o sistema registre a resposta. | Resposta recebida, status atualizado no banco, log gerado. | Alta | 13 | Encerramento de chamados |
| US13 | Sprint 3 | Como sistema, quero armazenar logs de envio, resposta e encerramento dos alertas. | Logs persistidos no banco com ID, usuário, mensagem e timestamps. | Alta | 5 | Registro de logs |
| US14 | Sprint 3 | Como gestor, quero visualizar histórico de alertas e ações tomadas. | Dashboard com listagem e filtros. | Média | 8 | Histórico de monitoramento |
| US15 | Sprint 3 | Como sistema, quero exportar relatórios em PDF/CSV. | API gera relatório consolidado com dados de indicadores e alertas. | Média | 8 | Relatórios |
| US16 | Sprint 3 | Como gestor, quero visualizar comparativos históricos de tráfego em gráficos. | Gráficos interativos com períodos (semana, mês, ano). | Média | 5 | Comparativos históricos |
| US17 | Sprint 3 | Como sistema, quero integrar dados externos (ex: clima) para enriquecer análise. | API integrada, dados combinados. | Baixa | 8 | Dados externos complementares |
| US18 | Sprint 3 | Como gestor, quero visualizar indicadores no mapa em tempo real, com pings representando radares. | Mapa com ícones (radares/ônibus) atualizados em tempo real. | Alta | 8 | Visualização em tempo real |

</details>

---

<details>
<summary>Backlog da Sprint 1</summary>

| ID  | Envolvidas | User Story | Critérios de Aceitação | Prioridade | Estimativa (pts) | Requisito do Cliente |
|-----|------------|------------|-----------------------|------------|-----------------|--------------------|
| US01 | BD | Como gestor, quero cadastrar indicadores no sistema para que sejam usados no monitoramento automático. | Inserção de indicadores com nome, unidade, limite e tipo; validação obrigatória; persistência no banco. | Alta | 5 | Criação de indicadores |
| US02 | Back | Como sistema, quero processar os dados armazenados no banco relacional para disponibilizar via API. | API RESTful em Spring Boot com endpoints GET/POST/PUT/DELETE; retorno em JSON. | Alta | 8 | Manipulação de dados no banco |
| US03 | Front | Como gestor, quero visualizar em uma dashboard inicial os níveis gerais da cidade e por regiões. | Dashboard com status geral, blocos por região e cores de alerta; integração via API. | Alta | 8 | Dashboard com níveis |
| US04 | Front | Como gestor, quero visualizar um mapa da cidade com cores por região. | Mapa Leaflet integrado, regiões coloridas conforme níveis da API. | Média | 5 | Georreferenciamento |
| US05 | Back/BD | Como sistema, quero registrar logs de criação e atualização de indicadores para auditoria. | Logs salvos no banco com usuário, data e ação. | Média | 3 | Registro de logs |

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
