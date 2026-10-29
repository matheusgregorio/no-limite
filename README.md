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

## Publicar no Netlify

No [painel do Netlify](https://app.netlify.com/), escolha criar um novo projeto com origem no GitHub, autorize o acesso ao repositório `matheusgregorio/no-limite`, escolha a branch `main` e publique. O arquivo `netlify.toml` configura a pasta pública como a raiz do repositório. Depois, pushes na `main` podem gerar novos deploys automaticamente.

## Privacidade e backup

Os lançamentos ficam **somente no armazenamento local deste navegador** (localStorage). Não são enviados a servidores e não sincronizam entre dispositivos. Apagar os dados do site/navegador pode apagar seu histórico. Use **Exportar backup** regularmente e guarde o arquivo em local seguro.

## iPhone

Depois de publicar em HTTPS: Safari → Compartilhar → Adicionar à Tela de Início.
