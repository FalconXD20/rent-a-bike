# Rent a Bike

Painel web de exemplo para gestão de locação de bicicletas. O projeto é estático, responsivo e salva os dados no `localStorage` do navegador.

## Funcionalidades
- Dashboard de exemplo com indicadores da frota, locações e faturamento.
- Visualização simples da distribuição da frota por status.
- Cadastro de bicicletas e clientes com validações básicas.
- Abertura e encerramento de locações com estimativa de cobrança.
- Pesquisa e filtro da frota, além de histórico.
- Dados de demonstração e ação para restaurá-los.

## Executar localmente
Abra `index.html` no navegador. Tailwind CSS, Lucide e a fonte DM Sans são carregados por CDN, então a primeira abertura requer conexão com a internet.

## Publicar no GitHub Pages
O workflow em `.github/workflows/deploy-pages.yml` publica o site após push na branch `main`. No GitHub, abra **Settings → Pages** e selecione **GitHub Actions** como origem, caso ainda não esteja selecionada. Depois que o workflow terminar, a URL ficará visível em **Settings → Pages** e no ambiente `github-pages` da execução da Action.

> A versão atual é uma demonstração de navegador: `localStorage` é local ao perfil/dispositivo e não sincroniza entre usuários. Não use dados pessoais reais antes de conectar a um backend seguro. A integração futura com Supabase deve usar políticas RLS; nunca exponha a chave `service_role` no frontend.
