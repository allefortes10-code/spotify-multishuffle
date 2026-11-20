# Spotify MultiShuffle

Aplicação web experimental para selecionar playlists e gerar uma sequência de faixas individualmente embaralhadas.

## Publicação no GitHub Pages
1. Abra **Settings → Pages** no repositório.
2. Em **Build and deployment**, escolha **Deploy from a branch**.
3. Selecione a branch **main** e a pasta **/(root)**; toque em **Save**.
4. No Spotify Developer Dashboard, adicione como Redirect URI exatamente:
   https://allefortes10-code.github.io/spotify-multishuffle/
5. Abra o endereço publicado no Safari do iPhone e conecte o Spotify.

## Funcionamento
- OAuth Authorization Code com PKCE; nenhum Client Secret fica no navegador.
- Seleção de playlists privadas e colaborativas, sujeita às permissões e regras de acesso do Spotify.
- Distribuição equilibrada entre playlists e deduplicação por ID de faixa dentro de cada ciclo.
- Requer Spotify Premium e um dispositivo Spotify ativo.

## Limitações
- O iOS pode suspender abas em segundo plano; mantenha a página aberta para monitoramento.
- A fila inicial envia até 100 faixas. A continuidade e o controle da fila dependem dos endpoints e limites vigentes do Spotify.
- O Development Mode do Spotify pode restringir usuários e playlists acessíveis.
- O Redirect URI deve corresponder exatamente ao cadastrado no Spotify Developer Dashboard.
- Este é um projeto experimental, não afiliado ao Spotify.
