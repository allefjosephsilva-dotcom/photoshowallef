# Allef PhotoShow

Site de galeria fotográfica profissional com upload via URL (Google Fotos) e painel de administração.

## Recursos
- Upload de fotos via URL (cole o link do Google Fotos).
- Armazenamento local com IndexedDB (as fotos ficam no navegador).
- Painel admin para adicionar/excluir fotos e alterar configurações (nome, descrição, background).
- Tema claro/escuro.
- Curtidas e comentários (salvos no IndexedDB).

## Como usar
1. Abra `admin.html` para gerenciar fotos e configurações.
2. Cole a URL da foto (Google Fotos) e clique em "Adicionar foto".
3. Abra `index.html` para ver a galeria pública.
4. Para publicar, envie os arquivos para GitHub Pages ou outro host estático.

> Observação: Este projeto usa armazenamento local (IndexedDB + localStorage). Para ter uma galeria pública permanente, hospede os arquivos (por exemplo, no GitHub Pages). Fotos dependem de URLs que permitam acesso público.

