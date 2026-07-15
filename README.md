# Text Express 5.0

Ferramenta local de scripts para atendimento e registros internos de protocolo.

## Novidade principal: sequências de falas

As sequências existem **somente na aba Atendimento**.

Ao criar um atendimento, escolha:

- **Fala única**: um texto independente;
- **Sequência de falas**: várias mensagens ligadas ao mesmo assunto.

Os protocolos continuam sendo textos únicos e completos.

### Exemplo incluído

**Roteador sem gerência**

- `/semgerencia` abre a sequência;
- `/semgerencia1` insere a explicação do problema;
- `/semgerencia2` informa que serão realizadas atualizações;
- `/semgerencia3` solicita o reinício dos equipamentos.

Dentro da sequência também existem os botões:

- **Inserir**;
- **Inserir e avançar**;
- reiniciar sequência;
- marcar falas opcionais;
- preencher variáveis compartilhadas uma única vez.

## Interface mais leve

- painel reduzido;
- menos bordas e cores fortes;
- cards compactos;
- categorias menores;
- detalhes simplificados;
- rodapé e botões discretos;
- launcher pequeno e arrastável preservado.

## Recursos mantidos

- scripts e protocolos existentes;
- atalhos personalizados;
- busca, categorias e favoritos;
- variáveis `[nome]`, `[prazo]` etc.;
- importar, exportar e restaurar;
- modo claro e escuro;
- armazenamento local;
- inserção no campo ativo ou cópia.

## Atualização no GitHub

Substitua na raiz do repositório:

- `index.html`
- `styles.css`
- `app.js`
- `bookmarklet.js`
- `README.md`

Depois aguarde o GitHub Pages e pressione `Ctrl + F5`.

A versão migra automaticamente as três falas antigas de “Sem Gerência TP-Link” para uma única sequência, preservando os demais modelos.
