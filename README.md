# Text Express

Ferramenta de expansão de textos para atendimento ao cliente e registro de protocolos, carregada por bookmarklet e sem dependências externas.

## Conteúdo do projeto

- `index.html`: interface completa e página local de demonstração.
- `styles.css`: estilos isolados pelo prefixo `te-`, com modo claro e escuro.
- `app.js`: lógica completa, persistência, atalhos, importação/exportação e os modelos iniciais.
- `bookmarklet.js`: carregador para adicionar aos favoritos do navegador.

A base inicial contém **211 scripts de atendimento** e **105 protocolos**, totalizando **316 modelos**.

## Teste local

Não abra o arquivo diretamente por `file://` caso o navegador imponha restrições. Na pasta do projeto, execute um servidor local:

```bash
python -m http.server 8080
```

Depois acesse:

```text
http://localhost:8080
```

No campo demonstrativo, digite `/a-saudacao-01` e pressione Espaço.

## Publicação no GitHub Pages

1. Crie um repositório, por exemplo, `text-express`.
2. Envie `index.html`, `styles.css`, `app.js` e `bookmarklet.js` para a raiz.
3. No GitHub, abra **Settings → Pages**.
4. Em **Build and deployment**, selecione **Deploy from a branch**.
5. Escolha a branch principal e a pasta `/root`.
6. Aguarde a publicação.

A URL normalmente ficará assim:

```text
https://SEU_USUARIO.github.io/text-express/
```

## Configuração do bookmarklet

Abra `bookmarklet.js` e substitua:

```text
https://SEU_USUARIO.github.io/text-express/
```

pela URL real do projeto publicado.

Depois:

1. Crie um novo favorito no navegador.
2. Use o nome `Text Express`.
3. Cole todo o conteúdo de `bookmarklet.js` no campo de endereço/URL.
4. Abra o sistema de atendimento e clique no favorito.

## Uso dos atalhos

Cada modelo possui:

- tipo: Atendimento ou Protocolo;
- nome;
- atalho escolhido pelo usuário;
- tecla de ativação: Espaço, Tab ou Enter;
- categoria;
- conteúdo;
- variáveis no formato `[variavel]`.

Exemplo:

```text
Atalho: /reiniciar
Ativação: Espaço
Conteúdo: Por gentileza, desligue os equipamentos da tomada, aguarde 30 segundos e ligue novamente.
```

Ao digitar `/reiniciar` e pressionar Espaço, o comando é substituído pelo texto completo.

O usuário pode alterar qualquer atalho pelo botão **Editar**. O sistema impede atalhos duplicados.

## Armazenamento

Os modelos são gravados no `localStorage` com a chave:

```text
text_express_snippets
```

O modo escuro usa:

```text
te_dark_mode
```

O armazenamento pertence ao domínio da página atual. Assim, dados salvos em um sistema podem não aparecer em outro domínio. Use **Exportar** e **Importar** para transportar a base.

## Recursos implementados

- criação, edição, exclusão e listagem;
- abas separadas para Atendimento, Protocolo e Favoritos;
- busca por nome, atalho, categoria ou conteúdo;
- filtros por categoria;
- atalhos personalizados pelo usuário;
- expansão com Espaço, Tab ou Enter;
- inserção em `input`, `textarea` e campos `contenteditable`;
- variáveis preenchidas antes da inserção;
- cópia automática quando não há campo ativo;
- importação e exportação em JSON;
- prevenção de IDs e atalhos duplicados;
- restauração da base original;
- painel arrastável, minimizável e fechável;
- botão flutuante de reabertura;
- atalho global `Ctrl + Shift + S`;
- modo claro e escuro;
- notificações do tipo toast;
- configurações de expansão, permanência do painel e confirmação de exclusão.

## Limitações de páginas corporativas

Algumas páginas podem bloquear bookmarklets, `fetch`, scripts externos ou estilos remotos por políticas de segurança, como CSP. Campos dentro de `iframe` de outro domínio também não podem ser acessados pela página principal. Nesses casos, o favorito precisa ser executado dentro do próprio frame ou o ambiente precisa liberar a origem do GitHub Pages.
