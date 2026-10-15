# Documentação do Projeto: Landing Page - COD Report

## 1. Objetivo da Atividade
Desenvolver uma landing page com tema livre para treinar habilidades de front-end básico (HTML/CSS), desenvolver repertório visual (IDV) e, principalmente, documentar a comunicação com a IA (Prompt Engineering / "Vibecode").

## 2. Tema e Escopo
* **Tema Principal:** Call of Duty, o jogo online que eu jogo.
* **Foco:** Uma vitória recente e fictícia de um esquadrão em partida Multiplayer, contada como notícia.
* **Restrição Técnica:** Dados mockados diretamente no código. Proibido o uso de API externa, JavaScript e frameworks.
* **Restrição de Conteúdo:** Sem imagens ou arte oficial do jogo. Elementos visuais só com CSS.

## 3. Decisões de Design (IDV)
* **Estilo Visual:** Dossiê militar: sóbrio, limpo e direto, sem o visual escuro padrão de jogos.
* **Referência:** Estrutura de notícia do projeto "Timão News" (manchete, placar, destaques, CTA). `[PREENCHER: referência visual do tema militar, ex.: menus de jogos de tiro, painéis de briefing]`
* **Paleta de Cores:**
  * **Fundo Principal:** Papel cáqui (`#EDE6D0`)
  * **Fundo Secundário:** Areia (`#D9CDAA`)
  * **Hero:** Verde-oliva (`#3B4A2F`)
  * **Texto, topo e rodapé:** Tinta (`#232A1B`)
  * **Destaques (botão e placar vencedor):** Laranja alerta (`#C8571B`)
* **Tipografia:** Saira Stencil One nos títulos (lembra caixas militares) e Barlow no texto.
* **Elemento de destaque:** Mira em CSS no hero. O resto fica discreto.

## 4. Estrutura da Página e Decisões Técnicas
**HTML5 Semântico** e **CSS3 puro**.

**Mapeamento de Seções:**
1. `<header>`: Marca "COD Report".
2. `<main>`:
   * `<section id="hero">`: Manchete sobre a virada e parágrafo curto sobre o clima da partida.
   * `<section id="detalhes">`: Placar centralizado (Meu Esquadrão 200 x 168 Equipe Rival) e lista `<dl>` com destaques de cada jogador.
3. `<footer>`: Botão CTA "Entrar no esquadrão" e créditos do projeto.

## 5. Estratégia de Comunicação com a IA (Vibecode)
* **Entrevista primeiro:** a IA me fez perguntas para o tema sair de mim.
* **Spec-driven:** a conversa virou um `.md` com requisitos, estrutura e instruções para outro bot.
* **Contexto zero:** passei só a spec para o Copilot, para testar se o documento bastava.
* **Revisão crítica:** comparei o resultado com um projeto anterior (Corinthians) e corrigi o foco.

Os textos completos estão em `PROMPTS.md`.

## 6. Revisão crítica e correções
| O que saiu errado | Como percebi | Correção |
|---|---|---|
| Textos genéricos, sem falar do jogo | Li cada seção e nada citava o que eu jogo | Pedi textos sobre o Call of Duty que eu jogo |
| Página com seções demais (modos, loadout, processo, registros) e sem história | Comparei com o projeto do Corinthians, que conta uma única notícia | Reduzi para hero + detalhes + CTA. Processo e registros ficaram só em `docs/` |
| Botão sem fechamento claro | O botão do hero só rolava a página | Criei CTA no rodapé: "Entrar no esquadrão" |

## 7. Pontos de atenção
* Dados fictícios (nomes, abates e placar).
* Fonte do Google Fonts; sem internet, usa Impact.
* Responsivo até 360px. Foco visível no teclado. Animação desativada para quem prefere menos movimento.
