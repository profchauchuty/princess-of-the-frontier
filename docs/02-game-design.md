# 02 — Game design

## Mundo e exploração

- Mundo dividido em mapas e instâncias.
- O jogador pode escolher manualmente uma instância ao entrar em um mapa.
- A troca de instância é livre pelo menu, respeitando a capacidade da instância.
- A câmera de exploração e o zoom foram escolhidos em decisões anteriores; os valores finais e as regras de transição precisam ser formalizados durante o protótipo.
- Navegação entre mapas, minimapa, inventário, HUD, NPCs e apresentação de missões fazem parte do desenho geral.
- A sincronização do mundo é controlada pelo servidor, incluindo movimentação, combate, robôs, inimigos, itens coletados e eventos compartilhados.

## Personagens e social

O planejamento contempla contas, personagens, progressão, amizades, grupos, guildas, comunicação entre jogadores, trocas de itens, morte e pontos seguros de renascimento. Regras exatas, limites e telas devem ser detalhados antes de implementar cada sistema.

## Robôs

Os robôs podem ser fabricados e montados com componentes, projetos e atributos computacionais. A programação influencia o comportamento durante as batalhas. O jogador deve poder testar algoritmos e acompanhar o desempenho do robô.

### Requisitos mínimos de combate do MVP

- Um robô controlado pelo jogador.
- Um cenário de combate simples.
- Um conjunto limitado de componentes e atributos.
- Algoritmo executado em ambiente controlado.
- Resultado do combate validado pelo servidor.
- Registro de resultado para a missão e a progressão.

## Economia

A economia foi definida como parte do design, mas os valores, fontes e sumidouros de recursos, limites de troca e medidas contra exploração econômica ainda precisam de especificação numérica.

## Narrativa

- Campanha principal dividida em capítulos progressivos.
- Apresentação híbrida por diálogos, cenas animadas e narrativa ambiental.
- Narrativa social e política crítica e interativa, com diferentes perspectivas e consequências locais.
- Enredo principal linear: as escolhas alteram diálogos, sem ramificar os acontecimentos centrais.

## Áudio

Músicas e efeitos serão produzidos por um processo híbrido, com IA para conceitos ou materiais iniciais e edição/mixagem manual. Devem ser usados apenas materiais com direitos compatíveis com a distribuição do jogo.
