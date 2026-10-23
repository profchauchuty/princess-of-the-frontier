# 04 — Arquitetura técnica

## Componentes

### Cliente Godot Web
- Godot com GDScript.
- Exportação para Web.
- Renderização 2D isométrica, interface, câmera, animações, controles e editor educacional.
- Cliente nunca é autoridade para recompensas, inventário, combate ou progressão.

### Backend
- Node.js + TypeScript.
- Express.js para API HTTP.
- Socket.IO para comunicação em tempo real.
- Backend modular por funcionalidade: autenticação, personagens, instâncias, mundo, combate, robôs, missões, inventário, progressão, moderação e administração.

### Banco de dados
- PostgreSQL para persistência.
- Prisma ORM para modelos, migrações e consultas tipadas.

### Painel administrativo
- React + Vite.
- Acesso exclusivo a uma conta de administrador na política inicial.
- API protegida por autorização no servidor; ocultar telas no frontend não é controle de segurança suficiente.

## Comunicação

A opção selecionada para tempo real é Socket.IO. O cliente Godot precisa usar um cliente compatível com o protocolo Socket.IO. Uma conexão WebSocket genérica não é automaticamente equivalente ao protocolo Socket.IO; validar uma biblioteca compatível em prova técnica antes de fechar a implementação.

## Autoridade do servidor

O servidor deve validar:
- movimento e limites físicos;
- resultados de combate;
- consumo e aquisição de itens;
- recompensas e experiência;
- conclusão de missões;
- capacidade e entrada em instâncias;
- transações econômicas.

## Execução segura de algoritmos

**Risco técnico prioritário:** código de jogadores não pode ser executado diretamente com acesso irrestrito ao processo Node.js, ao sistema de arquivos, às credenciais ou à rede.

Antes de permitir programação textual arbitrária, definir um runtime restrito (por exemplo, uma linguagem própria/DSL ou sandbox isolada), limites de tempo e memória, ausência de acesso à rede e testes de abuso. A execução segura dos programas é requisito de arquitetura, não apenas uma funcionalidade educacional.

## Decisões técnicas ainda pendentes

- Biblioteca Socket.IO compatível com Godot Web.
- Protocolo e versionamento das mensagens.
- Frequência de atualização e interpolação de movimento.
- Modelo de autoridade e resolução de conflitos.
- Runtime seguro de algoritmos.
- Estratégia para migrações e compatibilidade de versões.
- Limites de capacidade por instância.
