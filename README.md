# AI API Cost Dashboard

Dashboard interativo, em arquivo único, sobre **custos de APIs de IA**.

## O que tem dentro

- **Visão geral de tokens** — 12 modelos com preço de entrada/saída por 1M de tokens, gráfico comparativo (escala linear/logarítmica), tabela completa com economia frente ao modelo mais caro e tooltip explicando cada conceito.
- **APIs por créditos** — 8 plataformas (Poe, OpenRouter, Perplexity, You.com, xAI, Groq, Cohere e Google Gemini API) que vendem **crédito pré-pago ou pontos de computação** em vez de cobrar por token: planos, taxas embutidas, validade do saldo e regras de expiração.
- **Calculadora de custo mensal** — informe os tokens de entrada e saída por mês e compare o custo de todos os modelos, com toggle de Batch API.
- **Central de chaves de API** — links diretos para a página de criação de chaves de 16 provedores, com a base URL da API e a variável de ambiente correspondente, prontas para copiar.
- **Três conceitos-chave** — DeepSeek Cache ($1,32 → $0,003), Horário de Pico do DeepSeek (01h–04h e 06h–10h UTC = 2×) e Batch API (−50% assíncrono em 24h).
- **Temas** — escuro, claro e alto contraste, com persistência em `localStorage`.

## Como usar

Abra o `index.html` direto no navegador. Não há build nem dependência de servidor: todo o CSS e o JavaScript estão embutidos no arquivo. O único recurso externo é o Chart.js, carregado por CDN (o painel tem fallback para canvas 2D caso o CDN falhe).

## Publicação via GitHub Pages

O repositório publica o `index.html` da raiz em:

```
https://hodhreego.github.io/ai-api-cost-dashboard/
```

## Aviso sobre os dados

Os **preços dos 12 modelos** são ilustrativos, fornecidos como referência de estudo. Os **dados da seção de créditos** (planos, taxas, validades) foram levantados em 28/10/2026 e podem mudar — consulte sempre a página oficial de cada provedor antes de decidir.
