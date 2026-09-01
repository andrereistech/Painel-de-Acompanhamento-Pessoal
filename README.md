# Painel de Acompanhamento Pessoal

Aplicativo web de página única (single-file) para acompanhamento diário de rotina de saúde: hidratação, treinos, check-ins semanais e evolução de indicadores ao longo do tempo.

## Funcionalidades

- **Painel principal** — indicadores de saúde com semáforo visual (verde / amarelo / vermelho conforme faixas de referência) e o treino programado para o dia atual.
- **Cronograma semanal** — controle de treino e consumo de água dia a dia, com meta calculada automaticamente.
- **Check-in semanal** — registro de peso, medidas e sintomas, feito uma vez por semana.
- **Registro de exames** — upload de laudo em PDF com extração automática dos valores, ou preenchimento manual.
- **Evolução** — comparação entre a medição inicial e cada nova medição, com gráficos de tendência.
- **Exportação** — geração de planilha `.xlsx` com os dados registrados.

## Privacidade

Este projeto **não tem back-end e não envia dados para nenhum servidor**. Todas as informações digitadas ficam salvas apenas no navegador de quem está usando o app (armazenamento local do navegador). Nada é compartilhado com terceiros nem com quem hospeda o site.

Por ser um site estático hospedado publicamente, o **código-fonte** é visível a quem acessar o repositório — mas nenhum dado pessoal é armazenado nele.

## Como usar

Basta abrir o link publicado, ou baixar o arquivo `index.html` e abrir localmente em qualquer navegador — funciona offline, exceto pelo carregamento inicial de três bibliotecas usadas para gráficos, exportação de planilha e leitura de PDF.

## Tecnologias

- HTML, CSS e JavaScript puros (sem frameworks, sem build)
- [Chart.js](https://www.chartjs.org/) — gráficos de evolução
- [SheetJS (xlsx)](https://sheetjs.com/) — exportação de planilha
- [PDF.js](https://mozilla.github.io/pdf.js/) — leitura automática de exames em PDF

## Estrutura do repositório

```
index.html    → aplicativo completo (interface + lógica)
robots.txt    → impede indexação do site por buscadores
```

## Licença

Uso pessoal.
