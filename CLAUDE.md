# gliamedpropostas — orientação para sessões de IA neste repo

Site estático de **propostas comerciais**, servido em `marketing.glia.med.br`
(ver `CNAME`). HTML puro, sem build e sem dependências.

## Estrutura

```
index.html            índice
propostas/<cliente>/  uma pasta por cliente (ex.: institutomoura, nutrimarianamarins)
CNAME                 marketing.glia.med.br
```

Cada proposta é uma página independente. Não há template compartilhado nem
sistema de componentes — e isso é adequado ao propósito: uma proposta é feita
uma vez, enviada, e não volta a mudar.

## Relação com o resto

Este repo **não faz parte do produto Gliamed**. É material comercial da
operação de marketing médico, irmão de `landingpage-maker` (a ferramenta que
prospecta e gera as páginas).

Visão geral da plataforma de produto: `../MPfSMI/WHOAMI.md`.

## Regras ao mexer aqui

1. **Conteúdo de cliente é conteúdo real.** Nome, serviços, depoimentos e
   contato de um negócio real não podem ser inventados nem "melhorados" com
   informação que o cliente não forneceu.

2. **Sem build.** Não introduza bundler ou framework. O valor é ser HTML que
   qualquer servidor estático publica.

3. **Uma pasta por cliente.** Não crie abstração entre propostas — elas não
   compartilham ciclo de vida.

4. **Não publique dado sensível.** Preço fechado, contrato e dados pessoais do
   cliente não vão para um repositório que serve página pública.
