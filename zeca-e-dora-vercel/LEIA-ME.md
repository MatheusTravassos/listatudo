# Zeca e Dora no Vercel

O jogo é um site estático: só o `index.html` (o `vercel.json` é opcional). Não precisa de build.

## Jeito 1: pelo GitHub (recomendado)
1. Crie um repositório no GitHub e envie os arquivos desta pasta (`index.html` e `vercel.json`).
2. Em vercel.com, clique em **Add New → Project** e importe esse repositório.
3. Em *Framework Preset* escolha **Other**, deixe *Build Command* e *Output Directory* vazios e clique em **Deploy**.
4. Cada vez que o `index.html` mudar no GitHub, o Vercel publica de novo sozinho.

## Jeito 2: pelo terminal
```
npm i -g vercel
cd zeca-e-dora-vercel
vercel --prod
```

Observação: o progresso fica salvo no navegador de cada jogador (localStorage), separado do progresso do jogo no Claude.
