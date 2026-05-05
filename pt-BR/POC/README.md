# Proof of Concept (POC): The Context Bridge

## 1. Escopo da POC
O objetivo da POC é demonstrar que uma IA consegue identificar quando um código enviado via Pull Request (PR) **não cumpre** os critérios de aceitação definidos numa tarefa do Jira.

## 2. Cenário de Teste
- **Input A:** Um ticket do Jira (ex: "Criar endpoint de login com validação de 2FA").
- **Input B:** Um diff de código (ex: Código que cria o login, mas esquece o 2FA).
- **Output esperado:** Um relatório da IA apontando: "Risco de Qualidade: O código implementa o login, mas falta a lógica de 2FA mencionada no critério de aceitação 2".

## 3. Arquitetura Simplificada
1. **Mock Data:** JSONs simulando a API do Jira e do GitHub.
2. **LLM Prompting:** Uso de *Few-Shot Prompting* para ensinar à IA como comparar requisitos vs. código.
3. **Interface:** Um dashboard simples (Streamlit ou Markdown estático) comparando o "Esperado" vs. "Entregue".

## 4. Métricas de Sucesso da POC
- Precisão na identificação de "Gaps de Requisito" acima de 80%.
- Tempo de análise inferior a 30 segundos por ticket/PR.