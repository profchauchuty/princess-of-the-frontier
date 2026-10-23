# 08 — Plano de implementação do MVP

## Objetivo

Entregar um ciclo jogável completo: exploração multiplayer, combate com robôs, programação funcional, missões educacionais e progressão inicial.

## Fase 0 — Provas técnicas

- Exportar uma cena simples do Godot para Web.
- Confirmar compatibilidade de cliente Socket.IO com Godot Web.
- Conectar cliente e servidor com autenticação de teste.
- Sincronizar movimento de dois clientes.
- Validar build e execução na PaaS pretendida.
- Definir o modelo seguro de execução de programas.

**Saída:** relatório curto com escolhas técnicas confirmadas e riscos.

## Fase 1 — Fundação

- Criar monorepo e scripts de desenvolvimento.
- Configurar TypeScript, Express, Socket.IO, Prisma e PostgreSQL.
- Configurar migrations e testes.
- Criar estrutura básica do projeto Godot.
- Criar pipeline de validação.

**Critério de conclusão:** cliente conecta ao backend; backend grava e lê dados; testes básicos executam.

## Fase 2 — Mundo mínimo multiplayer

- Um mapa isométrico.
- Movimentação e câmera.
- Colisões e interações básicas.
- Uma instância com capacidade configurável.
- Reconexão com restauração do estado validado pelo servidor.

**Critério de conclusão:** dois ou mais jogadores veem movimentos consistentes na mesma instância.

## Fase 3 — Robô e combate

- Um robô e um conjunto limitado de componentes.
- Um inimigo controlado pelo servidor.
- Uma arena.
- Um formato inicial de programa.
- Runtime restrito para execução.
- Testes automatizados do comportamento.
- Resultado do combate persistido.

**Critério de conclusão:** o jogador programa o robô, executa o algoritmo e conclui um combate validado pelo servidor.

## Fase 4 — Missão educacional

- Uma missão guiada.
- Editor de programação.
- Testes com casos predefinidos.
- Feedback progressivo.
- Registro de tentativas e competências.

**Critério de conclusão:** uma missão educacional é completada e o progresso permanece após novo login.

## Fase 5 — Progressão e interface

- Personagem e experiência.
- Inventário mínimo.
- Uma recompensa.
- HUD e painel de missão.
- Interface responsiva básica.

**Critério de conclusão:** o ciclo de jogar, programar, combater, receber recompensa e salvar progresso funciona de ponta a ponta.

## Fase 6 — Administração e operação

- Painel React mínimo.
- Consulta de contas e personagens.
- Registros administrativos.
- Monitoramento e status do serviço.
- Backups e teste de restauração.
- Revisão de segurança.

## Fora do primeiro corte

Para reduzir risco, deixar para depois do ciclo mínimo:
- muitas regiões e capítulos;
- economia complexa;
- guildas completas;
- troca livre de itens;
- certificados públicos avançados;
- ferramentas próprias de edição de mapas;
- escalabilidade multi-região;
- detecção antitrapaça baseada em IA.

## Regra de execução

Cada fase deve gerar uma entrega testável antes de ampliar o escopo. Não começar a produzir dezenas de mapas e sprites antes de provar a conexão multiplayer e a execução segura dos programas.
