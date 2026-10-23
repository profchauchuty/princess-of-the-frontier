# 05 — Modelagem de dados inicial

Este documento apresenta entidades candidatas; não é um schema Prisma definitivo.

## Entidades candidatas

| Entidade | Responsabilidade |
|---|---|
| `Account` | Credenciais, estado da conta, idade declarada e preferências |
| `Character` | Nome, atributos, nível, experiência e localização persistida |
| `Session` | Sessões autenticadas e recuperação de conexão |
| `Map` | Metadados e configuração de mapas |
| `Instance` | Instância ativa de um mapa e limite de capacidade |
| `Robot` | Robô associado ao personagem |
| `RobotComponent` | Componentes montados e seus atributos |
| `RobotBlueprint` | Projetos de componentes disponíveis |
| `RobotProgram` | Programa versionado associado a um robô |
| `Mission` | Definição de missão e requisitos |
| `MissionProgress` | Estado de conclusão e tentativas por personagem |
| `AssessmentRun` | Casos de teste, resultado e métricas de avaliação |
| `InventoryItem` | Itens possuídos e quantidades |
| `Achievement` | Definição de conquista |
| `CharacterAchievement` | Conquistas obtidas |
| `EducationalCompetency` | Competências e critérios |
| `CompetencyProgress` | Progresso do personagem por competência |
| `ModerationReport` | Denúncias de jogadores |
| `ModerationAction` | Advertências, silenciamentos e suspensões |
| `AuditLog` | Registro de ações administrativas e eventos de segurança |

## Princípios

- Usar identificadores estáveis e chaves estrangeiras.
- Definir restrições e índices para consultas frequentes.
- Não confiar em dados de progressão enviados pelo cliente.
- Registrar alterações administrativas sensíveis.
- Evitar armazenar dados pessoais desnecessários.
- Não guardar senhas em texto puro; usar hash de senha apropriado.
- Definir política de retenção, exportação e exclusão de dados antes do lançamento.

## Próxima etapa

Criar um diagrama entidade-relacionamento e o schema Prisma apenas depois de validar os fluxos do MVP e as regras de propriedade, exclusão e retenção.
