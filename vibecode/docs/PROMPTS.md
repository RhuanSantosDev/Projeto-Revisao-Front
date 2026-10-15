# Registro de Prompts: Landing Page "Meu Lobby" (Call of Duty)

## Registro bruto, na ordem enviada

### Gemini / Claude (chat)

#### 1.prompt
```
Faça uma entrevista comigo para entendermos o que posso fazer para essa atividade de front-end básico

Desenvolvam uma landing page, com tema livre, para treinar e explorar os benefícios do vibecode.

O foco não é só o resultado final.
Quero ver como você pensou, como se comunicou com a IA e como corrigiu o caminho quando algo não saiu como esperado.

Para registros da atividade, além da página gerada, quero na pasta do projeto todos os registros dos prompts, as pesquisas, decisões de design, referências visuais, paleta de cores, tudo o que direcionou a resolução final da página.

O objetivo é desenvolver repertório visual, tomada de decisão em identidade visual (IDV) e clareza na comunicação com ferramentas de IA, aprendendo a escrever prompts específicos e a revisar o que a IA entrega com olhar crítico.
```

#### 2.prompt
```
Entrevista
```

#### 3.prompt
```
Faça um último arquivo .md para auxílio de outro bot utilizando o conceito de spec-driven

## Requisito
Estruturas do projeto:
index.html
css/style.css
```

### Copilot: janela com contexto zero
```
Você é um dev iniciando na área de front-end
Siga o arquivo spec_implementation.md para criarmos um site temático.
```

### Correções
```
- alguns textos
  fala de algo sei lá, do COD, jogo online que eu jogo
```

#### Correção 2 (após comparar com o projeto do Corinthians)
```
Quero o projeto do Call of Duty no mesmo patamar do do Corinthians, nada muito complexo.
```
Resultado: página reduzida a uma única história (vitória fictícia), com hero, placar, destaques e CTA.

---

# Anotações de cada etapa

1. **Entrevista (1.prompt):** colei o enunciado inteiro para a IA conhecer os critérios (processo, não só resultado). Avaliei se as perguntas eram sobre mim. `[PREENCHER: perguntas e respostas]`
2. **"Entrevista" (2.prompt):** comando curto para iniciar as perguntas. Decisão: tema Call of Duty, jogo que eu jogo.
3. **Spec (3.prompt):** transformei a conversa em documento para outro bot. Avaliei se tinha tema, seções, paleta e regras claras.
4. **Copilot, contexto zero:** janela nova, só com a spec, para testar se o documento bastava. Avaliei estrutura de pastas, seções e visual.
5. **Correção 1:** textos genéricos. O prompt foi vago ("alguns textos").
6. **Correção 2:** ao comparar com o projeto do Corinthians, vi que a página tinha seções demais e nenhuma história. Pedi o mesmo patamar, sem complexidade.

## Comparação: prompt único vs. fluxo em etapas

| | Prompt único (Corinthians) | Fluxo em etapas (Call of Duty) |
|---|---|---|
| Velocidade | Rápido | Mais lento |
| Origem do tema | Eu já chego com a ideia | A IA descobre comigo |
| Onde o erro aparece | No código final | Na spec, antes do código |
| O que aprendo | Escrever um prompt completo | Transformar conversa em documento |

## Como eu escreveria hoje o prompt de correção

```
Reescreva os textos do hero e dos destaques. Estão genéricos.
Fale em primeira pessoa de uma partida de Call of Duty Multiplayer:
cite o modo, o placar e o que cada jogador fez. Frases curtas.
Mantenha o HTML e o CSS como estão.
```

Lição: dizer **onde** corrigir, **o que** está errado e **o que não mexer** evita que a IA reescreva a página inteira.
