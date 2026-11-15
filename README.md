# Vitrola Virtual — site da Web Rádio

Site de uma página (HTML + CSS + JavaScript puro) com o player oficial FastCast4u.

## Estrutura
```text
vitrola-virtual/
├── index.html              (todo o HTML, CSS e JS)
├── README.md
└── assets/
    ├── images/logo.jpg     (logomarca enviada; usada no hero e no compartilhamento)
    ├── icons/favicon.png   (recorte da vitrola, 128 px)
    ├── icons/apple-touch-icon.png
    └── fonts/              (vazia; a fonte Outfit é carregada do Google Fonts)
```

## Publicar no GitHub Pages
1. Crie uma conta em github.com e um repositório **público** (ex.: `vitrola-virtual`).
2. Clique em **Add file > Upload files** e envie `index.html`, `README.md` e a pasta `assets` (mantenha a estrutura).
3. Vá em **Settings > Pages**. Em *Build and deployment*, escolha **Deploy from a branch**, branch `main`, pasta `/ (root)`, e salve.
4. Em 1 a 3 minutos o site estará em `https://SEU-USUARIO.github.io/vitrola-virtual/`.
5. Depois de publicado, edite `index.html` e troque, nas metatags Open Graph, `og:image` pelo endereço completo da logo (ex.: `https://SEU-USUARIO.github.io/vitrola-virtual/assets/images/logo.jpg`) e, se quiser, adicione `og:url`. Redes sociais exigem endereço completo para mostrar a prévia.

## Como editar
Procure no `index.html` pelos comentários `<!-- ===== ... ===== -->`:
- **Textos:** altere dentro das seções `SOBRE A RÁDIO`, `HERO` e `RODAPÉ`.
- **Contatos e redes:** os links aparecem três vezes (cabeçalho, seção de contatos e rodapé). Use a busca do editor (`virtual_vitrola`, `radio.vitrolavirtual`, `contato.vitrolavirtual@gmail.com`) e troque em todos os locais.
- **Cores:** bloco `:root` no início do CSS (`--teal`, `--plum`, `--gold`, `--ink`, `--paper`).
- **Logo:** substitua `assets/images/logo.jpg` mantendo o nome do arquivo.
- **Player:** não altere `data-username="vitrolavirtual"` nem o endereço do script, a menos que a FastCast4u informe um código novo.

## Observações
- O player é carregado do servidor da FastCast4u. Para tocar, o visitante precisa de internet e o serviço de streaming precisa estar no ar.
- O CSS do site não mexe nos elementos internos do player para não conflitar com os estilos da FastCast4u.
