# No Limite

Controle de gastos simples e responsivo para acompanhar orçamentos mensais e metas, especialmente no iPhone.

## Recursos

### Gastos
- Limites mensais por categoria, começando com Uber/99 (R$ 600), restaurantes/delivery (R$ 650), mercado e conveniência (R$ 200) e compras online (R$ 350).
- Mostra quanto ainda pode gastar **nesta semana** (segunda a domingo), no total e em cada categoria. O valor da semana é o que sobrava do mês na segunda-feira dividido pelos dias restantes: um dia caro se dilui, e uma semana estourada deixa as próximas menores. Em Uber/99, mostra também quantas corridas cabem.
- No mês em que você começa a usar o app, os limites são proporcionais aos dias que faltam a partir do primeiro uso.
- Avisa quando você está gastando mais rápido do que o mês permite. A marca branca na barra mostra até onde você deveria ter chegado hoje.
- **Valores rápidos**: em + Gasto, um toque num valor já salva o gasto. Os botões aprendem os valores que você mais usa em cada categoria, e dá para desfazer pela notificação.
- Aceita valores como `28,90`, `28.90`, `1.500` e `1.500,00`.
- **Remanejar**: move parte do limite de uma categoria para outra só no mês atual, sem mudar o limite fixo nem o total do mês. Dá para desfazer.
- Alertas visuais aos 80% e 100% do limite, histórico por mês, edição e exclusão de gastos.

### Economia
- Em ⚙ Limites, informe quanto gastava por mês **antes** do app em cada categoria.
- O app mostra quanto você já economizou desde o primeiro registro, o ritmo deste mês contra o de antes, quanto isso dá por ano e quanto representa das suas metas.
- A economia só é real se você registrar todos os gastos.

### Metas
- Aba própria com metas como apartamento e viagem: valor da meta, quanto guardar por mês, quanto já guardou e a previsão de quando chega lá.
- **Plano do mês**: renda líquida − contas fixas − limites de gastos − metas = quanto fica livre para gastar.
- No começo do mês, oferece guardar numa meta o que sobrou dos limites no mês anterior.

### Dados
- Os dados ficam **somente no armazenamento local do aparelho** (localStorage). Não vão para servidor nenhum e não sincronizam entre dispositivos.
- No iPhone, os dados do Safari e os do app instalado na Tela de Início ficam separados. O app avisa quando está aberto no Safari.
- Use **Exportar backup** regularmente. O rodapé avisa quando o último backup tem mais de 30 dias.

## Executar

É um site estático, sem backend nem etapa de build. Abra `index.html` no navegador ou sirva a pasta com qualquer servidor HTTP.

## Publicação e previews (GitHub Pages)

O GitHub Actions publica tudo na branch `gh-pages`:

| Origem | Endereço |
|---|---|
| `main` (produção) | https://matheusgregorio.github.io/no-limite/ |
| `dev` | https://matheusgregorio.github.io/no-limite/dev/ |
| Cada pull request | https://matheusgregorio.github.io/no-limite/pr-preview/pr-NÚMERO/ |

O link do preview aparece num comentário do PR e é removido quando o PR fecha.

**Configuração única:** em [Settings → Pages](https://github.com/matheusgregorio/no-limite/settings/pages), escolha **Deploy from a branch**, branch **gh-pages**, pasta **/(root)**, e salve.

Os previews (`/dev/` e `/pr-preview/…`) guardam dados separados do app de produção e mostram uma faixa roxa no topo. Dá para testar à vontade sem mexer nos seus lançamentos.

## iPhone

Abra o endereço de produção no Safari → Compartilhar → Adicionar à Tela de Início, e use sempre pelo ícone.
