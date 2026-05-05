# Roadmap: Building the POC (Phase 1)

## Setup & Design (Dia 1-2)
- [ ] **Definição de Personas:** Criar o perfil do "Revisor Detalhista" (tom de voz da IA).
- [ ] **Dataset de Teste:** Selecionar 5 exemplos reais (anonimizados) de tickets bons/maus e códigos correspondentes.
- [ ] **Escolha do Modelo:** Configurar acesso ao modelo via AI/works™ (ou GPT-4/Claude para testes iniciais).

## Desenvolvimento (Dia 3-5)
- [ ] **Módulo de Extração:** Script para ler texto de tickets (Markdown/JSON).
- [ ] **Módulo de Análise de Código:** Script para processar arquivos `.diff` ou `.py/.js`.
- [ ] **Engenharia de Prompt:** Criar o "System Prompt" que instrui a IA a ser um auditor de qualidade rigoroso.
- [ ] **Validação de Output:** Criar um template de resposta (ex: Semáforo de Qualidade - Verde/Amarelo/Vermelho).

## Demonstração (Dia 6-7)
- [ ] **Gravação de Vídeo:** Demo comparando uma revisão humana rápida vs. a análise profunda da IA.
- [ ] **Documentação de Resultados:** Tabela de "Antes vs Depois" do uso da ferramenta.
