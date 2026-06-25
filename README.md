# Kingdom Play

Site institucional da **Kingdom Play**, indústria de playgrounds e brinquedotecas.
Página única, estática, focada em conversão (WhatsApp), visual e interativa.

## Como abrir

Abra o arquivo `index.html` no navegador (duplo clique). Não precisa de servidor.

## Publicar no GitHub Pages

1. Suba esta pasta como um repositório no GitHub.
2. Em **Settings → Pages**, escolha a branch (`main`) e a pasta `/root`.
3. O site fica disponível em `https://SEU-USUARIO.github.io/NOME-DO-REPO/`.

## Estrutura

```
.
├── index.html              Página completa (HTML + CSS + JS, tudo embutido)
└── assets/
    ├── *.jpg               Fotos reais de obras entregues
    ├── logo-crest.png      Brasão da marca
    └── fonts/
        ├── NeulisSans-*.otf   Fonte Neulis Sans (fallback dos títulos)
        └── NeulisCursive.*    (adicione aqui — veja abaixo)
```

## Fonte dos títulos (Neulis Cursive)

Os títulos usam **Neulis Cursive**. Para ativá-la:

1. Coloque o arquivo da fonte em `assets/fonts/` com o nome
   `NeulisCursive.woff2` (ideal) ou `NeulisCursive.otf`.
2. Pronto — o `@font-face` no `index.html` já aponta para esse caminho.

Enquanto o arquivo não estiver presente, os títulos usam **Neulis Sans**
(já incluída) como fallback automático.

## Vídeos do YouTube

A seção **Vídeos** usa 3 vídeos do YouTube que carregam só quando a pessoa
clica no play (mais rápido). Para colocar os seus vídeos:

1. Abra o `index.html` e procure por `data-yt="SUBSTITUA_ID_1"`
   (há também `SUBSTITUA_ID_2` e `SUBSTITUA_ID_3`).
2. Troque cada `SUBSTITUA_ID_X` pelo **ID** do seu vídeo do YouTube.
   - Na URL `https://www.youtube.com/watch?v=ABC123xyz`, o ID é `ABC123xyz`.
   - Em links curtos `https://youtu.be/ABC123xyz`, o ID também é `ABC123xyz`.
3. Salve. As capas (thumbnails) já usam fotos reais dos projetos; se quiser,
   troque os `src` das imagens dentro de cada `.video-card`.

## Contato

- WhatsApp: (62) 99690-4920
- CNPJ: 30.700.323/0001-59
