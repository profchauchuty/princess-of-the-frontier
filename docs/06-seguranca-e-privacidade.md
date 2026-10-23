# 06 — Segurança, moderação e privacidade

## Contas e autenticação

Decisões registradas:
- autenticação de jogadores;
- proteção de senhas com hash seguro;
- HTTPS;
- validação de entradas;
- limitação de tentativas de login;
- gerenciamento seguro de sessões;
- autenticação em duas etapas opcional;
- logs de acesso;
- recuperação de conta.

## Autorização administrativa

O plano inicial prevê uma conta de administrador com acesso completo. A autorização precisa ser verificada no backend em cada endpoint e evento Socket.IO privilegiado. Segredos administrativos não devem ser embutidos no cliente.

## Antitrapaça

- Validação no servidor de movimentação, combate, inventário e recompensas.
- Detecção de anomalias.
- Logs de segurança.
- Revisão administrativa de ocorrências suspeitas.

## Moderação

- Filtros automáticos de chat.
- Denúncias de jogadores com categorias, descrição, registros relevantes e status.
- Análise administrativa.
- Escala progressiva de punições: advertência, silenciamento, suspensão temporária e banimento permanente.
- A decisão de planejamento não prevê recurso de punição. Antes de lançar, considerar transparência, prevenção de abuso administrativo e mecanismos mínimos de correção de erro.

## Privacidade e menores

- Coletar apenas dados necessários.
- Publicar política de privacidade.
- Permitir solicitações de exportação e exclusão de dados, conforme requisitos legais.
- A idade mínima e as regras para menores precisam ser confirmadas. O planejamento menciona classificação pretendida de 14 anos e também cadastro com declaração de idade; esses itens são distintos e devem ser formalizados separadamente.
- Verificar as obrigações aplicáveis da LGPD e às crianças/adolescentes antes da publicação.

## Backups

Foi selecionada a opção de backups automáticos diários, recuperação para um ponto no tempo quando suportada pela infraestrutura e testes periódicos de restauração.

## Checklist mínimo antes da produção

- Revisão de dependências e vulnerabilidades.
- Proteção contra força bruta.
- Validação de permissões em HTTP e Socket.IO.
- Rate limiting e limites de payload.
- Proteção contra abuso de chat e spam.
- Segredos fora do repositório.
- Teste de restauração de backup.
- Procedimento para incidentes de segurança.
