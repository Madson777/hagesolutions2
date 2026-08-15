# Hage Solutions — versão estática para GitHub Pages

## O que é esta versão

Este pacote transforma o site em uma estrutura estática adequada para GitHub Pages, mantendo HTML/CSS/JavaScript no front-end e evitando dependências de WordPress/PHP.

## Pastas

- `index.html` — página principal
- `assets/css/style.css` — estilos
- `assets/js/main.js` — interações
- `assets/js/config.js` — configuração do formulário de currículo
- `assets/images/` — logo, favicon e demais imagens locais
- `assets/videos/` — `video1.mp4`, `video2.mp4`, `video3.mp4`

## Vídeos

Coloque os três arquivos do seu computador em `assets/videos/` com estes nomes: 

- `video1.mp4` — vídeo do Hero
- `video2.mp4` — vídeo institucional
- `video3.mp4` — vídeo do CTA

## Logo

Coloque o logo original em `assets/images/logo.png`.

## GitHub Pages

1. Crie um repositório no GitHub.
2. Envie todo o conteúdo desta pasta para a raiz do repositório.
3. Vá em **Settings → Pages**.
4. Em **Build and deployment**, escolha **Deploy from a branch**.
5. Selecione `main` e a pasta `/ (root)`.
6. Salve.
7. O GitHub Pages gerará o endereço do site.

## Currículos — atenção

GitHub Pages é hospedagem estática. Ele **não executa PHP nem cria banco de dados**. Por isso, o formulário de currículo nesta versão exige um endpoint externo.

Antes de publicar, edite `assets/js/config.js` e preencha `cvEndpoint` com a URL do serviço/backend responsável por receber os currículos. Sem isso, o formulário não finge um envio bem-sucedido: ele informa que o endpoint ainda precisa ser configurado.

Para usar banco de dados e armazenamento seguro de currículos, mantenha o plugin/backend que preparei para WordPress ou use um backend externo.
