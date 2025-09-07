Alef PhotoShow — site com integração Google Fotos (cliente)
Conteúdo:
- index.html : site completo com painel do dono e botão "Conectar Google Fotos" (usa Google Identity Services token client)
Senha padrão do painel do dono: alef1235

Como usar:
1) Baixe e extraia o ZIP
2) Abra index.html em um navegador moderno (recomendado: Chrome)
3) No painel Configurações cole seu Google OAuth Client ID (crie-o no Google Cloud Console > APIs & Services > Credentials > OAuth client ID). Use tipo 'Web application' e adicione 'http://localhost' como URI de origem se for testar local.
4) Clique em 'Conectar Google Fotos' e faça o login/consent. Após a autorização, você poderá selecionar álbuns e importar fotos para seu site (as imagens são salvas localmente no navegador via IndexedDB).

Observações e limitações:
- Este é um exemplo de integração cliente (front-end). Dependendo das políticas do Google, algumas operações (como listar todas as fotos) podem exigir configurações extras ou uso de um backend que proteja o Client Secret e trate tokens com mais segurança.
- Para publicar em produção e hospedar imagens na nuvem (para visitantes verem sem depender do seu navegador), configure Firebase Storage ou outro armazenamento e ajuste o código para enviar os arquivos ao storage em vez de apenas ao IndexedDB.
- Se encontrar erros relacionados a permissões ou CORS ao buscar as imagens, considere usar um backend ou o próprio Google Photos Picker (server-assisted) para fluxos seguros.
