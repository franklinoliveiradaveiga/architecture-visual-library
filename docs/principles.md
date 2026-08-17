# Princípios de Design da Biblioteca

Este documento define as regras que devem ser seguidas ao criar ou evoluir componentes, para garantir consistência visual e semântica ao longo do tempo.

## 1. Conceito antes de ferramenta

- Prefira formas que representem **conceitos de arquitetura** (ex: API Gateway, Event Bus, Bounded Context, Data Store) em vez de logos de produtos específicos.
- Quando for necessário representar uma tecnologia concreta, mantenha uma versão “genérica” e outra “específica” sempre que possível.

## 2. Consistência visual

- **Tamanho base**: use dimensões padrão (ex: 120x60, 160x80, 80x80) para facilitar alinhamento.
- **Espaçamento**: mantenha padding e margens consistentes entre elementos.
- **Cores**:
  - Use uma paleta limitada e bem definida.
  - Prefira cores com bom contraste (modo claro e escuro).
  - Evite gradientes e efeitos desnecessários.
- **Tipografia**: use fontes padrão do Draw.io ou defina um estilo único e documente-o.
- **Estilo de linhas e conectores**: padronize espessura, estilo (sólido/tracejado) e setas.

## 3. Baixo ruído visual

- Priorize legibilidade em diferentes escalas (zoom out / impressão).
- Evite detalhes excessivos que só aparecem em zoom alto.
- Mantenha o visual limpo o suficiente para ser usado em apresentações para stakeholders de negócio.

## 4. Nomenclatura

- Use nomes claros e em inglês (padrão da indústria) ou português, mas **mantenha consistência** em todo o repositório.
- Prefira nomes descritivos: `api-gateway`, `message-broker`, `domain-service` em vez de abreviações obscuras.
- Para bibliotecas Draw.io: use nomes de arquivo em kebab-case (`core-components.xml`, `integration-patterns.xml`).

## 5. Organização

- Separe bibliotecas por responsabilidade ou domínio quando começarem a ficar grandes.
- Mantenha templates e exemplos separados das bibliotecas de shapes.
- Sempre que adicionar um novo componente relevante, inclua:
  - Preview em `assets/previews/`
  - Entrada no `docs/catalog.md`

## 6. Evolução e versionamento

- Mudanças que quebram compatibilidade visual devem ser comunicadas (changelog ou release notes).
- Prefira evoluir componentes existentes em vez de criar duplicatas.

## 7. Público-alvo

 Os diagramas serão usados por:
- Arquitetos e desenvolvedores
- Pessoas de negócio / product
- Times de operação e segurança

Por isso, clareza e consistência têm prioridade sobre “beleza excessiva”.
