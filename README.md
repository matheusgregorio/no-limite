# No Limite

Controle de gastos simples e responsivo para acompanhar orçamentos mensais, especialmente no iPhone.

## Recursos

- Define limites de gastos por categoria, começando com Uber/99 (R$ 600), restaurantes/delivery (R$ 650) e mercado (R$ 450).
- Registra gastos com valor, data, categoria e descrição.
- Mostra quanto resta gastar, com alertas visuais aos 80% e 100% do orçamento.
- Permite editar/excluir despesas e criar categorias.
- Exibe histórico por mês e exporta/importa backup em JSON.
- Pode ser instalado na Tela de Início do iPhone e funciona offline após a primeira visita.

## Executar

É um site estático, sem backend nem etapa de build. Abra `index.html` no navegador ou publique o conteúdo da raiz do repositório em um serviço HTTPS.

## Publicar no GitHub Pages (recomendado)

O No Limite é um site estático e pode ser hospedado gratuitamente no GitHub Pages, sem marca d'água e sem serviço de build externo.

Abra [Settings → Pages](https://github.com/matheusgregorio/no-limite/settings/pages), selecione **Deploy from a branch**, escolha a branch **main** e a pasta **/(root)** e clique em **Save**. O site será publicado em https://matheusgregorio.github.io/no-limite/ depois que o GitHub concluir a implantação.

Mudanças na branch `main` serão publicadas pelo GitHub Pages automaticamente.

## Hospedagem alternativa: Netlify

O projeto também pode ser servido pelo Netlify usando `netlify.toml`. Se houver um selo “Powered by Netlify”, ele pode ser desligado em **Project configuration → General → Powered by Netlify badge**.

## Privacidade e backup

Os lançamentos ficam **somente no armazenamento local deste navegador** (localStorage). Não são enviados a servidores e não sincronizam entre dispositivos. Apagar os dados do site/navegador pode apagar seu histórico. Use **Exportar backup** regularmente e guarde o arquivo em local seguro.

## iPhone

Depois de publicar em HTTPS: Safari → Compartilhar → Adicionar à Tela de Início.
