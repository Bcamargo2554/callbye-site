# Site do CallBye para GitHub Pages

Este repositório publica a página de suporte do CallBye e o arquivo `app-ads.txt` exigido pela AdMob. O domínio público pretendido é `https://callbye.online/`.

## Publicação

1. Publique `index.html`, `app-ads.txt`, `CNAME` e `.nojekyll` na raiz de um repositório público.
2. No repositório, em **Settings → Pages**, configure **Deploy from a branch**, a branch principal e a pasta **/(root)**. Configure o domínio personalizado `callbye.online` e aguarde a confirmação do GitHub. Recomenda-se verificar o domínio na conta do GitHub por registro TXT antes de apontar o DNS.
3. Na GoDaddy, substitua os registros A do domínio raiz pelos quatro IPs oficiais do GitHub Pages: `185.199.108.153`, `185.199.109.153`, `185.199.110.153` e `185.199.111.153`. Configure `www` como CNAME para o endereço `<usuario>.github.io` da conta que publica o repositório. Remova registros conflitantes somente depois de verificar os alvos exatos.
4. Quando o HTTPS estiver ativo, confira se `https://callbye.online/app-ads.txt` responde diretamente com HTTP 200 e contém exatamente a linha:

   `google.com, pub-3202719333046472, DIRECT, f08c47fec0942fa0`

5. Na ficha do CallBye no Google Play Console, defina **Site do desenvolvedor** como `https://callbye.online/` e publique a alteração. O AdMob usa o domínio dessa ficha para encontrar o arquivo. Depois, em AdMob, use **Verificar app → Verificar atualizações**. A indexação pode demorar.

Não basta registrar o domínio ou subir o arquivo ao GitHub: DNS, GitHub Pages e URL da Play Store precisam apontar para o mesmo site público.

