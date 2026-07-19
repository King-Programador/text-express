# Text Express 26.0 — Protocolo padrão e sequência otimizada

Esta versão continua a base estável da versão 25.0. Todos os cartões, categorias, sequências, protocolos, atalhos, importação, mesclagem, salvamento local, tema e redimensionamento foram preservados.

## Novidades da versão 26.0

### Protocolo como área inicial

Cada nova ativação do Text Express em uma página ou guia começa diretamente em **Protocolo**. Depois de aberto, ainda é possível alternar normalmente para Atendimento ou Favoritos.

### Abertura das sequências no Atendimento

Ao clicar em **ABRIR SEQUÊNCIA**:

- o painel principal é recolhido automaticamente para o ícone flutuante;
- o menu da sequência permanece aberto;
- o painel principal pode ser restaurado clicando no mesmo ícone flutuante;
- restaurar o painel não fecha a sequência;
- os dois menus podem permanecer abertos ao mesmo tempo.

### Prevenção de sobreposição

Quando o painel principal é restaurado com uma sequência aberta, o Text Express verifica se as duas janelas estão sobrepostas. Se necessário, reposiciona e, dentro dos limites mínimos, ajusta o menu da sequência para manter as duas áreas visíveis.

A posição e o tamanho continuam salvos no navegador.

### Confirmação discreta de cópia

Quando o chat não permite inserção automática e uma fala precisa ser copiada, aparece a confirmação curta:

**Texto copiado.**

O menu da sequência continua aberto após a cópia.

## Recursos preservados

- 21 categorias;
- 132 cartões/modelos;
- 29 sequências de Atendimento;
- 97 falas internas;
- Atendimento e Protocolo separados;
- atalhos pesquisados somente na área selecionada;
- arraste do menu de sequência com botão esquerdo ou direito;
- redimensionamento pelas bordas e cantos;
- fechamento da sequência com `ESC` ou `X`;
- importação completa e mesclagem;
- modo claro e escuro;
- salvamento automático e compatibilidade com dados existentes.

## Publicação no GitHub

Envie estes cinco arquivos para a raiz do repositório:

- `index.html`
- `styles.css`
- `app.js`
- `bookmarklet.js`
- `README.md`

Repositório: `https://github.com/King-Programador/text-express`

GitHub Pages: `https://king-programador.github.io/text-express/`
