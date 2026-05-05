# Roadmap: Scaling to Production (Phase 2+)

## Integração Real-Time
- [ ] **Webhook Service:** Implementar escuta ativa para disparar análise assim que um PR é aberto.
- [ ] **Jira App Integration:** Criar um widget dentro do Jira que dá uma "Nota de Qualidade" à história antes de ela ir para o desenvolvedor.

## Inteligência Avançada
- [ ] **Análise de Sentimento/Esforço:** Identificar sinais de falta de comprometimento através da verbosidade e clareza nos comentários de commit.
- [ ] **Auto-Ticket Generation:** Se a IA detectar um bug recorrente no código, sugerir automaticamente a criação de um ticket de débito técnico.
- [ ] **Custom Style Guides:** Permitir que cada projeto carregue o seu próprio ficheiro de regras (ex: "Neste projeto usamos Clean Architecture estrita").

## Governação e Dashboards
- [ ] **Manager View:** Dashboard para gestores com métricas de "Qualidade Evolutiva" do projeto.
- [ ] **Feedback Loop:** Permitir que o humano diga "IA, este alerta foi um falso positivo", treinando o modelo local.