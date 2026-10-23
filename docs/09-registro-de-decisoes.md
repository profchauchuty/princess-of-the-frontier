# 09 — Registro de decisões recuperáveis

Este registro consolida as decisões que podem ser recuperadas do histórico disponível. Ele **não pretende reconstruir palavra por palavra todas as 150 perguntas**. Quando uma opção foi revisada posteriormente, prevalece a decisão mais recente.

## Decisões de produto e jogo

- Movimentação de personagens: opção A escolhida no planejamento inicial.
- Interação multiplayer: B.
- Missões cooperativas de programação: C.
- Organização dos conteúdos de programação: C.
- Ajuda educacional: C.
- Avaliação de aprendizado: C.
- Evolução do conhecimento: C.
- Economia: A.
- Narrativa principal: C; posteriormente detalhada como campanha linear por capítulos.
- Papel das muralhas na progressão: C.
- Cidade inicial: D.
- Atmosfera visual predominante: B.
- Passagem do tempo: C; posteriormente fixada como ciclo global de 24 horas reais.
- Inimigos de IA: A.
- Chefes: C.
- Programação de robôs em batalhas: A.
- Acompanhamento do desempenho dos robôs: C.
- Fabricação e montagem: C.
- Obtenção de projetos de componentes: A.
- Energia dos robôs: C.
- Atributos dos robôs: C.
- Influência dos atributos computacionais: C.
- Interface de programação: C.
- Testes de algoritmos: C.
- Missões educacionais e recompensas: C.
- Progressão social: C.
- Estrutura política das cidades: D.
- Relação corporações/jogadores: D.
- Papel dos jogadores diante do regime corporativo: D.
- Resistência tecnológica: C.
- Ingresso na resistência: C.
- Início da história: C.
- Primeiro objetivo: B.
- Primeira missão de programação: B.
- Apresentação do primeiro desafio: C.
- Interface de programação por blocos: B.
- Câmera de exploração: A.
- Zoom: houve respostas conflitantes; a decisão mais recente registrada antes da sequência de arquitetura foi A.
- HUD principal: A.
- Inventário: B.
- Interação com NPCs: A.
- Apresentação de missões: B.
- Navegação entre mapas: A.
- Minimapa: B.
- Comunicação entre jogadores: C.
- Formação de grupos: C.
- Distribuição de recompensas em grupo: C.
- Amizades: C.
- Guildas: D.
- Troca de itens: B.
- Morte do personagem: B.
- Pontos seguros de renascimento: B.
- Salvamento de progresso: B.
- Criação de personagens por conta: A.
- Exclusão e recriação de personagens: B.
- Autenticação: A.
- Infraestrutura multiplayer: B.
- Distribuição de jogadores por instância: B, com seleção manual.
- Troca de instância: A, livre pelo menu.
- Sincronização multiplayer: C, estado autoritativo no servidor.
- Comunicação em tempo real: B, Socket.IO.
- Renderização: Godot Web.
- Linguagem do cliente: GDScript.
- Backend: Node.js + TypeScript.
- Banco: PostgreSQL.
- ORM: Prisma.
- API: Express.js.
- Arquitetura backend: modular.
- Código: monorepo.
- Desenvolvimento local: execução manual, sem Docker obrigatório.
- Publicação: PaaS.
- Ambientes: desenvolvimento e produção, com bancos separados.
- Deploy: automático a partir da branch principal, após aprovação.
- Testes: unitários, integração, multiplayer e fluxos principais do cliente.
- Execução de testes: opção PaaS escolhida; confirmar capacidade real do provedor.
- Monitoramento: logs, erros, recursos e disponibilidade em painel centralizado.
- Administração: painel Web em React + Vite.
- Acesso administrativo: uma conta de administrador.
- Mapas: editor do Godot.
- Recursos visuais: IA para conceitos e edição manual.
- Animações: esqueléticas 2D.
- Iluminação: sistema híbrido.
- Clima: efeitos visuais simples, sem impacto mecânico.
- Ciclo de dia/noite: sincronizado pelo servidor; 24 horas reais; horário de Brasília UTC−3; horários fixos 6h amanhecer, 7h dia, 18h entardecer e 19h noite.
- Música: sistema híbrido por região e contexto.
- Estilo musical: ambient sombrio, industrial nas cidades e orquestral em combate.
- Produção sonora: IA mais edição e mixagem manual.
- Áudio: volume geral, música e efeitos separados.
- Controles: teclas personalizáveis.
- Acesso móvel: decisão final indica PWA instalável e interface responsiva; verificar compatibilidade real de exportação e requisitos de áudio/armazenamento no navegador.
- Movimentação móvel: joystick virtual.
- Interação móvel: toque direto ou botão contextual.
- Editor móvel: interface dedicada em tela cheia, com programação por blocos e teclado adaptado.
- Conexão instável: reconexão e restauração de estado validado pelo servidor.
- Offline: exclusivamente online.
- Atualizações: detecção automática de nova versão.
- Manutenção: programada e emergencial.
- Avisos: tela inicial, notificações in-game e página de status.
- Backups: automáticos diários, recuperação pontual quando disponível e testes de restauração.
- Gestão de contas: consulta, suspensão, advertências e histórico administrativo.
- Moderação: filtros, denúncias e análise administrativa.
- Denúncias: categorias, descrição, registros e status.
- Punições: escala progressiva.
- Recursos/contestação: não previstos no desenho inicial; revisar antes do lançamento.
- Antitrapaça: validação no servidor, detecção de anomalias, logs e análise administrativa.
- Segurança: HTTPS, hash de senha, validação, limitação de tentativas, sessão segura, 2FA opcional, logs e recuperação.
- Privacidade: coleta mínima, política, exportação e solicitação de exclusão conforme LGPD.
- Menores: há uma decisão de cadastro por declaração de idade e uma intenção de classificação etária de 14 anos; separar idade mínima de classificação de conteúdo antes do lançamento.
- Violência: estilizada, dano mecânico, sem sangue.
- Temas sociais/políticos: narrativa crítica e interativa.
- Impacto das escolhas: história principal linear; diálogos podem mudar.
- História: diálogos, cenas animadas e narrativa ambiental.
- Campanha: capítulos progressivos.
- Conteúdo educacional: progressão por competências.
- Avaliação de código: testes, lógica, eficiência e objetivos.
- Orientação de erros: dicas progressivas.
- Progresso: dashboard educacional.
- Conquistas: medalhas/títulos e certificados digitais internos.
- Distribuição: gratuito com doações voluntárias.
- Divulgação: site oficial com informações, novidades e acesso.
- MVP: ciclo completo — exploração multiplayer, combate com robôs, programação funcional, missões educacionais e progressão inicial.

## Itens a confirmar antes de implementar

1. Protocolo e biblioteca de Socket.IO compatíveis com Godot Web.
2. Sandbox para execução segura de código de jogadores.
3. Regras exatas de instâncias, capacidade, movimento e combate.
4. Schema Prisma e modelo de persistência.
5. Fuso e regra de horário de verão/fuso global: manter uma referência IANA de `America/Sao_Paulo` em vez de codificar UTC−3 permanentemente, caso o objetivo seja acompanhar o horário civil brasileiro.
6. Regras de idade mínima, consentimento e privacidade de menores.
7. Política de contestação e salvaguardas contra erro administrativo.
8. Capacidades reais do PaaS para deploy, testes, WebSocket e PostgreSQL.
9. Limites concretos do MVP e critérios mensuráveis de desempenho.
