# Indo por Aí — correção definitiva do logo

Mantive a última versão do aplicativo e alterei somente a forma de carregar a marca.

## O que foi corrigido
- O logo foi reduzido e otimizado.
- O PNG foi inserido literalmente no `index.html`.
- O mesmo PNG foi inserido literalmente em cada página dinâmica do `app.js`.
- Não existe mais variável `${BRAND_LOGO}`.
- Nenhuma página depende de `assets/logo.png`.
- CSS e JavaScript receberam versão no endereço para evitar cache antigo.
- O Service Worker agora busca primeiro a versão online dos arquivos principais.
- O arquivo `_headers` impede o Netlify de manter HTML, CSS e JS antigos em cache.

## Como publicar
Suba todos estes arquivos para a raiz do GitHub, incluindo o arquivo `_headers`.

Depois:
1. Aguarde o deploy do Netlify.
2. Abra o endereço em uma aba privada do Safari para confirmar.
3. Remova o app antigo da tela inicial.
4. Adicione o app novamente.

Esta correção não altera o layout ou as funcionalidades.
