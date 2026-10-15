# Spec de Desenvolvimento: Landing Page "COD Report"

## 1. Visão Geral
Este documento especifica os requisitos para a criação de uma landing page responsiva, focada em uma notícia de vitória fictícia de um esquadrão em **Call of Duty**, o jogo online que o autor joga. O objetivo é aplicar conhecimentos de HTML5 e CSS3 puro.

## 2. Estrutura de Arquivos Exigida
O projeto deve estritamente seguir a seguinte estrutura de diretórios e arquivos:
```text
/ (raiz do projeto)
├── index.html
└── css/
    └── style.css
```

## 3. Requisitos Técnicos
*   **HTML:** Utilizar HTML5 Semântico (`<header>`, `<main>`, `<section>`, `<footer>`, `<dl>`).
*   **CSS:** CSS3 puro, sem frameworks (como Tailwind ou Bootstrap) e sem JavaScript.
*   **Responsividade:** O layout deve se adaptar a celular e desktop usando Media Queries e flexbox/grid (funcionar em 360px sem rolagem horizontal).
*   **Dados:** Todo o conteúdo deve ser *mockado* (inserido estaticamente no HTML). Nenhuma API externa deve ser consumida.
*   **Imagens:** Não usar logos, imagens ou arte oficial do jogo. Elementos visuais apenas com CSS.
*   **Fontes:** Saira Stencil One (títulos) e Barlow (texto), via Google Fonts, com Impact e system-ui como reserva.

## 4. Identidade Visual (IDV) e Paleta de Cores
O design deve seguir o conceito de **dossiê militar**: sóbrio, limpo e legível, evitando o visual escuro padrão de jogos de tiro.

*   **Cor de Fundo Principal:** Papel cáqui (`#EDE6D0`)
*   **Cor de Fundo Secundária/Containers:** Areia (`#D9CDAA`)
*   **Cor de Estrutura (hero):** Verde-oliva (`#3B4A2F`)
*   **Cor do Texto Principal, topo e rodapé:** Tinta (`#232A1B`)
*   **Cor de Destaque (Ações/Botões/Pontuação vencedora):** Laranja alerta (`#C8571B`)

**Regra de destaque:** um único elemento marcante, a mira (círculo com cruz) em CSS no hero.

## 5. Estrutura de Conteúdo (Wireframe Lógico)

### 5.1 `index.html`
1.  **`<header>`**
    *   Marca em texto: "COD Report".
2.  **`<main>`**
    *   **`<section id="hero">`**: Manchete em `<h1>` sobre a virada do esquadrão na última rodada. Um parágrafo curto (`<p>`) descrevendo o clima da partida. Mira em CSS ao fundo.
    *   **`<section id="detalhes">`**:
        *   Um placar centralizado e em destaque (ex: Meu Esquadrão 200 x 168 Equipe Rival), modo Multiplayer, Dominação, com a pontuação vencedora em cor de destaque.
        *   Uma lista de descrição `<dl>` com os destaques de cada jogador (nome fictício e abates).
3.  **`<footer>`**
    *   Botão de CTA (Call to Action) chamativo com o texto "Entrar no esquadrão".
    *   Créditos do projeto em texto menor, com aviso de dados fictícios e de marca registrada.

## 6. Instruções para o Bot Desenvolvedor
1. Leia esta especificação completamente.
2. Gere o código finalizado para `index.html` e `css/style.css` garantindo a ligação correta (`<link rel="stylesheet" href="css/style.css">`).
3. Defina as cores da paleta como variáveis CSS em `:root`.
4. Assegure que as cores de contraste atendam a requisitos básicos de acessibilidade visual.
5. Mantenha o código indentado e comentado onde achar necessário.
