# Text Express 3.0

Ferramenta local para **scripts de atendimento** e **registros de protocolo**, com atalhos personalizados, categorias editáveis e interface flutuante.

## Principal alteração desta versão

O Text Express agora inicia apenas como um **ícone flutuante compacto de 44 px**, no canto inferior direito.

- clique no ícone de raio para abrir o painel;
- clique em minimizar ou fechar para voltar ao ícone;
- o cabeçalho do painel aberto também ficou menor;
- o ícone possui tooltip ao passar o mouse;
- o atalho global `Ctrl + Shift + S` continua abrindo o painel.

Essa alteração evita que uma faixa grande fique sobre o sistema de atendimento.

## Recursos mantidos

- 211 scripts de atendimento e 105 protocolos;
- separação entre Atendimento, Protocolo e Favoritos;
- atalhos definidos pelo usuário;
- ativação por Espaço, Tab ou Enter;
- criação, edição e exclusão de modelos;
- categorias com ícone, cor, contador e edição;
- botão **+ Categoria** na faixa de filtros;
- variáveis em formato `[nome]`;
- inserção no campo ativo ou cópia para a área de transferência;
- importação, exportação e restauração;
- modo claro e escuro;
- dados salvos localmente no navegador.

## Arquivos para o GitHub

Substitua na raiz do repositório:

1. `index.html`
2. `styles.css`
3. `app.js`
4. `bookmarklet.js`
5. `README.md`

Depois aguarde o GitHub Pages publicar e pressione `Ctrl + F5`.

## Uso

1. Abra `https://mateus-progam.github.io/text-express/`.
2. Clique no pequeno ícone de raio no canto inferior direito.
3. Para usar dentro de outro sistema, recrie o favorito com o conteúdo atualizado de `bookmarklet.js`.
4. Clique em um campo do atendimento ou protocolo.
5. Abra o Text Express, escolha o modelo e clique em **Inserir**.

## Armazenamento

- modelos: `text_express_snippets`
- categorias: `text_express_categories`
- configurações: `text_express_settings`
- tema: `te_dark_mode`

Tudo permanece no navegador. Nenhum valor preenchido nas variáveis é enviado ao GitHub.
