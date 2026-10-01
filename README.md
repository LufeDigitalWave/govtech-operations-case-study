# Operação de atendimento e demandas

Case técnico anonimizado sobre sistemas de atendimento, registro de demandas e acompanhamento operacional.

> Publicação documental para avaliação técnica. Não contém aplicação executável, código de cliente, integrações ativas ou dados reais. A arquitetura é uma abstração didática, não um mapa de infraestrutura.

## Problema

Uma solicitação pode começar em um canal de conversa, virar uma demanda operacional e precisar de acompanhamento por pessoas diferentes. Sem uma separação clara dessas etapas, o histórico se fragmenta e mensagens repetidas podem gerar trabalho duplicado.

## Escopo representado

O case reúne interfaces de operação, serviços de atendimento e processamento de eventos. A leitura técnica se concentra no percurso entre entrada, classificação, persistência e acompanhamento, mantendo as integrações fora da descrição pública.

## Stack identificada

Python, FastAPI, Pydantic, SQLAlchemy e Alembic no backend; React, TypeScript e Vite na interface; componentes em TypeScript/Express. A presença dessas tecnologias foi identificada nos manifests e na estrutura dos projetos de origem; isso não constitui validação do ambiente de produção.

## O que discutir numa entrevista

- Como distinguir uma mensagem recebida de uma demanda registrada.
- Onde colocar validação, controle de acesso e deduplicação.
- Como preservar o contexto durante a transferência para atendimento humano.
- Como apresentar status operacional sem divulgar conteúdo sensível.

Consulte a [arquitetura e o roteiro de validação](ARCHITECTURE.md).

## Limites

Não são publicados órgãos, localidades, pessoas, regras internas, prompts, métricas, canais, endpoints ou configurações. Não há alegação de disponibilidade, escala ou conformidade certificada.
