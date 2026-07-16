# Text Express 19.0

## Estado visual salvo automaticamente

Ao fechar, minimizar, atualizar a página ou abrir novamente o Text Express,
o sistema recupera:

- última aba aberta: Atendimento, Protocolo ou Favoritos;
- última categoria selecionada em cada aba;
- posição horizontal da faixa de categorias em cada aba;
- pesquisa digitada em cada aba;
- posição vertical da lista de modelos em cada categoria;
- último card selecionado em cada visualização.

As posições do painel principal e do pequeno launcher já continuavam salvas
e permanecem funcionando.

## Ordem das categorias

A ordem definida pelo usuário ao mover categorias já é salva dentro das
próprias categorias. Nesta versão, além dessa ordem, também é salva a
posição horizontal da faixa. Assim, ao abrir novamente, a faixa volta ao
mesmo ponto em que estava.

## Backup completo

Os novos backups passam a incluir `uiState`, com o estado visual da
interface.

Ao escolher **Restaurar backup completo** em outro navegador, também são
restaurados:

- aba aberta;
- categoria ativa;
- pesquisas;
- rolagens;
- card selecionado;
- posição horizontal das categorias.

Backups antigos continuam compatíveis. Quando não possuem `uiState`, o
Text Express utiliza a visualização padrão.

## Atualização

Envie para a raiz do GitHub:

- index.html
- styles.css
- app.js
- bookmarklet.js
- README.md

Depois pressione Ctrl + F5.
