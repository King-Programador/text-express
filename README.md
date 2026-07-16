# Text Express 14.0

## Arraste mais rápido e posição de destino visível

O arraste nativo do navegador foi removido. Ele causava atraso e mostrava uma imagem fantasma do card.

Agora o Text Express usa movimentação direta pelo ponteiro:

- começa a mover após apenas 3 pixels;
- o card acompanha o mouse imediatamente;
- não existe imagem fantasma;
- não há atraso para trocar de posição;
- um espaço azul do tamanho do card mostra o destino;
- o espaço exibe “Soltar na posição X”;
- a lista rola automaticamente perto das bordas;
- a nova ordem é salva ao soltar;
- funciona em Atendimento e Protocolo;
- Esc cancela o movimento.

Inserir, Editar, Excluir e Favorito continuam funcionando sem iniciar o arraste.

## Persistência

A ordem escolhida:

- fica salva no navegador;
- permanece ao fechar ou desligar o computador;
- entra na exportação;
- volta pela importação;
- sincroniza entre abas abertas no mesmo site.

## Atualização

Envie para o GitHub:

- index.html
- styles.css
- app.js
- bookmarklet.js
- README.md

Depois pressione Ctrl + F5.
