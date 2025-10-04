# Fit Shopper - Exemplo para GitHub Pages

Este é um exemplo mínimo de site estático — pronto para ser enviado ao GitHub e publicado com GitHub Pages. O arquivo `index.html` já contém a tag do Google Ads (gtag.js) com o ID AW-11423608709 como exemplo.

Passos rápidos para publicar:

1. Inicialize o Git e conecte ao repositório GitHub:

```bash
cd fit-shopper-example
git init
git remote add origin https://github.com/SEU-USUARIO/fit-shopper.git
git add .
git commit -m "Primeira versão do site"
git push -u origin main
```

2. No repositório no GitHub, vá em Settings → Pages e selecione a branch `main` e pasta `/root`.
3. Aguarde alguns minutos e acesse: `https://SEU-USUARIO.github.io/fit-shopper/`.

Para usar domínio próprio, adicione um arquivo `CNAME` com seu domínio e crie registros DNS adequados no registrador.

Notas:
- Substitua os arquivos exportados do Canva por estes (ou mantenha este `index.html` como modelo).
- Verifique se o `gtag.js` foi carregado no Network do DevTools para confirmar que a tag do Google Ads está ativa.

Guia passo-a-passo (detalhado)

1. Crie um repositório no GitHub (público) chamado `fit-shopper` ou outro nome à sua escolha.
2. No terminal, envie os arquivos:

```bash
cd fit-shopper-example
git init
git add .
git commit -m "Primeira versão do site"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/fit-shopper.git
git push -u origin main
```

3. No GitHub: vá ao repositório → Settings → Pages. Em "Source" selecione `main` e pasta `/ (root)` e salve.
4. Aguarde alguns minutos. O GitHub mostrará o link do seu site (algo como `https://SEU-USUARIO.github.io/fit-shopper/`).
5. Para adicionar um domínio personalizado: crie um arquivo chamado `CNAME` na raiz do repositório contendo apenas `seu-dominio.com` e configure o DNS no seu registrador apontando um CNAME para `SEU-USUARIO.github.io`.

Dica de verificação do Google Ads:
- Abra o DevTools (F12) → aba Network → filtre por "gtag" ou "googletagmanager" e recarregue a página para ver se o script foi baixado.
- Na aba Console, execute `window.gtag` para confirmar que a função existe.

Domínio personalizado (resumo rápido):

- Crie um arquivo `CNAME` na raiz do repositório com seu domínio (por exemplo `fit-shopper.com`).
- No painel do seu registrador, adicione um registro CNAME apontando o seu domínio para `SEU-USUARIO.github.io`.
- Aguarde propagação DNS (pode levar algumas horas).


