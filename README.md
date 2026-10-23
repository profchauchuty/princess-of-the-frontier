# Princess of the Frontier

MMORPG educacional 2D isométrico com exploração multiplayer, combate com robôs programáveis e aprendizagem de programação.

> **Status:** planejamento inicial consolidado. Esta documentação organiza as decisões registradas durante a definição do projeto; não representa uma implementação já existente.

## Objetivo do MVP

Entregar um ciclo jogável completo contendo:
- exploração multiplayer;
- movimentação e interação com NPCs;
- combate com robôs;
- programação e teste de algoritmos dos robôs;
- missões educacionais com avaliação automatizada;
- progressão inicial e salvamento persistente.

## Stack escolhida

| Camada | Tecnologia |
|---|---|
| Cliente do jogo | Godot Web + GDScript |
| Renderização | Godot, mundo 2D isométrico |
| Backend | Node.js + TypeScript |
| API HTTP | Express.js |
| Multiplayer | Socket.IO |
| Banco de dados | PostgreSQL |
| Acesso ao banco | Prisma ORM |
| Painel administrativo | React + Vite |
| Repositório | Monorepo |
| Desenvolvimento local | Execução manual, sem Docker obrigatório |
| Hospedagem | PaaS; cliente como site estático e backend como serviço gerenciado |
| Repositório remoto | GitHub |
| Deploy | Automático após alterações aprovadas na branch principal, sujeito às capacidades da plataforma |

## Estrutura proposta

```text
princess-of-the-frontier/
├── README.md
├── docs/
├── client/       # Projeto Godot
├── server/       # Node.js + TypeScript
├── admin/        # React + Vite
├── shared/       # Contratos compartilhados, se necessário
├── .gitignore
└── .github/
    └── workflows/
```

A estrutura acima é um alvo organizacional. Pastas de aplicação podem ser criadas incrementalmente quando cada etapa começar.

## Documentos

- `docs/01-visao-geral.md` — conceito, público e pilares.
- `docs/02-game-design.md` — exploração, combate, mundo e progressão.
- `docs/03-sistema-educacional.md` — programação, avaliação e competências.
- `docs/04-arquitetura.md` — componentes e comunicação.
- `docs/05-modelagem-dados.md` — entidades iniciais e relações.
- `docs/06-seguranca-e-privacidade.md` — autenticação, moderação e dados.
- `docs/07-infraestrutura-e-operacao.md` — ambientes, testes, deploy e monitoramento.
- `docs/08-plano-mvp.md` — fases de implementação e critérios de conclusão.
- `docs/09-registro-de-decisoes.md` — decisões recuperáveis do planejamento.

## Identidade do projeto

- **Nome:** Princess of the Frontier
- **Tradução livre:** Princesa da Fronteira
- **Gênero:** MMORPG educacional com exploração, robôs e programação.
- **Direção visual:** fantasia tecnológica, pixel art isométrica e atmosfera de exploração.

## Próximo passo

Revisar os pontos marcados como **a definir**, validar a arquitetura de execução de código de robôs e construir o MVP em entregas pequenas, começando por uma prova técnica de Godot Web + Socket.IO.
