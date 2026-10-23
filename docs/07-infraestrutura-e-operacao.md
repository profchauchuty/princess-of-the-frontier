# 07 — Infraestrutura e operação

## Organização

- Monorepo no GitHub.
- Cliente Godot, backend Node.js e painel React no mesmo repositório.
- Desenvolvimento local manual, com serviços iniciados separadamente; Docker não é requisito do fluxo inicial.
- Ambientes separados de desenvolvimento e produção, incluindo bancos PostgreSQL distintos.

## Hospedagem

- Cliente Godot Web hospedado como site estático.
- Backend hospedado em PaaS com suporte a conexões persistentes/WebSocket.
- PostgreSQL em serviço compatível com a aplicação.
- Confirmar limites da plataforma escolhida: conexões WebSocket, suspensão por inatividade, memória, CPU, tráfego, conexões de banco e política de deploy.

## CI/CD

A intenção é realizar deploy automático após atualizações aprovadas na branch principal. Os testes precisam passar antes da publicação.

Uma decisão anterior selecionou a execução dos testes pela plataforma PaaS; essa capacidade varia entre provedores. Se o PaaS não oferecer um gate confiável, usar GitHub Actions para executar os testes e impedir o deploy quando falharem.

## Testes

- Unitários.
- Integração com PostgreSQL e API.
- Testes de eventos Socket.IO.
- Testes de fluxo do cliente Godot.
- Testes de reconexão.
- Testes de segurança para programas de robôs.
- Testes básicos de carga e de múltiplos jogadores.

## Monitoramento

Painel centralizado com:
- logs;
- erros;
- consumo de recursos;
- disponibilidade dos serviços.

## Manutenção

- Manutenções programadas para atualizações importantes.
- Intervenções emergenciais quando necessário.
- Avisos na tela inicial e dentro do jogo.
- Página pública de status dos servidores.

## Deploy inicial

1. Criar o repositório e configurar segredos.
2. Configurar PostgreSQL de desenvolvimento e produção.
3. Preparar build de exportação Web do Godot.
4. Publicar backend com Socket.IO.
5. Configurar HTTPS e CORS de acordo com os domínios reais.
6. Aplicar migrações do Prisma com processo seguro.
7. Configurar pipeline de testes e deploy.
8. Validar login, conexão, reconexão, persistência e monitoramento.
