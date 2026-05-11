# Papéis da Equipe (Versão Hackathon) - AI/Quality Sentinel

Este guia simplifica a estrutura de equipe para um hackathon com no máximo 3 pessoas.
O objetivo e acelerar decisões, reduzir overhead e focar em entrega de valor.

## Pagina Principal do Projeto

Para visao geral do AI/Quality Sentinel (problema, solucao e objetivos), use:
- [README do projeto (pt-BR)](../README.md)

## Estrutura Recomendada (ate 3 pessoas)

Em hackathon, uma pessoa acumula mais de um papel. A distribuicao abaixo funciona bem para tirar o POC do papel sem depender de especializacao FE/BE:

| Pessoa | Foco principal | Acumula papeis |
|---|---|---|
| Pessoa 1 | Produto e priorizacao | Product Owner + Scrum Master |
| Pessoa 2 | Desenvolvimento (generalista) | Implementacao de core + integracoes |
| Pessoa 3 | Desenvolvimento (generalista) | Implementacao de core + QA pratico |

## Responsabilidades Minimas por Frente

### 1. Produto e Prioridade
- Definir escopo minimo do hackathon (MVP).
- Priorizar backlog por impacto de demonstracao.
- Garantir alinhamento entre problema, solucao e demo final.

Referencias:
- [Product Owner](product-owner.md)
- [Scrum Master](scrum-master.md)

### 2. Desenvolvimento Core (Pessoa 2)
- Implementar os servicos e regras principais do POC.
- Integrar com os dados e fluxos necessarios para a demo.
- Garantir funcionamento ponta a ponta dos casos criticos.

Referencias:
- [Backend (.NET)](backend-dotnet.md)

### 3. Desenvolvimento Core + Qualidade (Pessoa 3)
- Dividir implementacao do core com a Pessoa 2 (sem fronteira fixa FE/BE).
- Definir e executar checklist rapido de qualidade para fluxos criticos.
- Cobrir o essencial com testes (ou roteiro de teste) para reduzir risco na apresentacao.

Referencias:
- [QA](qa.md)
- [Frontend (React/Angular)](frontend-react-angular.md)

## Mapa de Contribuicao por Papel

Esta secao detalha como cada papel pode acelerar o AI/Quality Sentinel no contexto de hackathon.

### Product Owner (PO)
- Traduz o problema de qualidade em objetivos claros para o MVP.
- Define criterios de sucesso da demo (o que precisa funcionar para gerar impacto).
- Mantem foco no valor de negocio e evita escopo que nao sera demonstrado.

Referencia:
- [Product Owner](product-owner.md)

### Scrum Master (SM)
- Remove bloqueios rapidamente (dependencias, decisoes pendentes, alinhamentos).
- Organiza o fluxo de trabalho para manter a equipe produtiva com pouco overhead.
- Garante cadencia curta de acompanhamento e ajuste de plano.

Referencia:
- [Scrum Master](scrum-master.md)

### Quality Assurance (QA)
- Define checklist minimo de qualidade para os fluxos mais criticos.
- Valida se os criterios de aceite do MVP estao realmente atendidos.
- Ajuda a reduzir risco de falha na apresentacao final com validacao orientada a cenarios.

Referencia:
- [QA](qa.md)

### Desenvolvedor Backend (.NET)
- Implementa servicos e regras centrais da solucao.
- Conecta integracoes necessarias para demonstrar o ciclo completo (intencao -> execucao -> padrao).
- Estrutura base tecnica para escalar o POC apos o hackathon.

Referencia:
- [Backend (.NET)](backend-dotnet.md)

### Desenvolvedor Frontend (React/Angular)
- Cria uma experiencia minima para demonstrar valor de forma clara.
- Traduz resultados tecnicos em visualizacao compreensivel para avaliadores e stakeholders.
- Apoia a narrativa da demo quando houver tempo para evolucao de interface.

Referencia:
- [Frontend (React/Angular)](frontend-react-angular.md)

### Especialistas Adicionais (quando disponivel)
- DevOps: acelera setup, automacao e estabilidade de ambiente.
- Dados: melhora a qualidade dos insumos e a leitura dos resultados.
- Seguranca: reduz riscos de exposicao e ajuda com boas praticas desde o POC.

Referencia:
- [Especialistas Adicionais](additional-specialists.md)

## Referencias Rapidas de Todos os Papéis

- [Product Owner](product-owner.md)
- [Scrum Master](scrum-master.md)
- [QA](qa.md)
- [Backend (.NET)](backend-dotnet.md)
- [Frontend (React/Angular)](frontend-react-angular.md)
- [Especialistas Adicionais](additional-specialists.md)

## Rito Leve de Trabalho (Sugestao)

- Daily curta: 10 minutos para alinhar bloqueios e proximas tarefas.
- Checkpoint tecnico: 1 ou 2 vezes ao dia para integrar frontend + backend.
- Revisao final: validar roteiro da demo e plano B para falhas.

## O Que Nao Priorizar no Hackathon

- Processos pesados de cerimonia.
- Cobertura de teste ampla fora dos fluxos criticos.
- Escopo grande sem validacao de valor na demo.

## Interface no Contexto do Hackathon

- A interface pode ser minima ou ate substituida por fluxo via API/CLI na primeira iteracao.
- Priorize primeiro: regra de negocio, integracoes e evidencia de valor funcionando.
- Se sobrar tempo, evolua a interface para melhorar narrativa da apresentacao.

## Equipe Atual

- [Matheus Costa Vieira](mailto:matheus.vieira@thoughtworks.com) - Desenvolvimento Backend (.NET)

## Proximo Passo

Depois de validar este formato em pt-BR, podemos replicar a mesma estrutura para en-US e es-ES.
