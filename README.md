# Laboratório Cloudflare Pages

Projeto Astro mínimo sobre as 10 heurísticas de usabilidade de Jakob Nielsen. Seu objetivo é testar, de ponta a ponta, o fluxo **Codex → GitHub → Cloudflare Pages**.

## Executar localmente

Requisitos: Node.js 20 ou superior e pnpm (via Corepack).

```sh
corepack enable
pnpm install
pnpm dev
```

O servidor local informa a URL no terminal, normalmente `http://localhost:4321`.

## Validar a versão de produção

```sh
pnpm build
pnpm preview
```

Os arquivos estáticos são gerados em `dist/`.

## Deploy no Cloudflare Pages

1. No painel da Cloudflare, abra **Workers & Pages** e crie um projeto Pages conectado ao GitHub.
2. Selecione o repositório `Ferrats/cloudfare-pages-laboratorio`.
3. Use o preset **Astro** ou configure manualmente:
   - comando de build: `pnpm build`
   - diretório de saída: `dist`
4. Defina `main` como branch de produção e conclua a configuração.

Novos commits em `main` publicarão a versão de produção. Pull requests e branches poderão gerar previews para revisão antes do merge.

## Escopo do laboratório

O projeto é propositalmente simples: Astro, HTML semântico e CSS. Não há backend, banco de dados, CMS ou JavaScript no cliente.
