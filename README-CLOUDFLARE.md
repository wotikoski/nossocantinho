# Publicar no Cloudflare Pages

Este projeto ja esta pronto para ser hospedado como site estatico no Cloudflare Pages.

## Estrutura publicada

- `index.html`
- `amanda-leonardo.jpg`
- `pix-qrcode.png`
- `_headers`

## Opcao mais simples: upload direto

1. Entre em [Cloudflare Pages](https://dash.cloudflare.com/).
2. Abra `Workers & Pages`.
3. Clique em `Create application`.
4. Escolha `Pages`.
5. Clique em `Upload assets`.
6. Envie a pasta `D:\Users\Leonardo\OneDrive\Documents\Cantinho`.
7. Defina um nome para o projeto.
8. Publique.

Como o site e estatico, nao precisa configurar:

- Build command
- Framework preset
- Output directory

## Conectar o dominio

1. Dentro do projeto publicado, abra `Custom domains`.
2. Clique em `Set up a custom domain`.
3. Informe o dominio ou subdominio desejado.
4. Confirme. Como o dominio ja esta no Cloudflare, o ajuste de DNS costuma ser automatico.

Exemplos:

- `cantinho.seudominio.com.br`
- `lista.seudominio.com.br`
- `seudominio.com.br`

## Configuracao recomendada

- Se usar o dominio raiz, configure tambem o `www` para redirecionar para o endereco principal, ou o contrario.
- Aguarde o certificado SSL ficar como ativo antes de divulgar o link.
- Teste no celular depois da publicacao.

## Observacao importante sobre compartilhamento

Os metadados de compartilhamento ja foram adicionados no `index.html`, mas se voce quiser que WhatsApp e redes sociais exibam a URL canonica correta, vale incluir depois o dominio final nas tags `og:url` e `canonical`.
