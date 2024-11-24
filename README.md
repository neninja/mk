# MK

Instruções referenciadas do jogo [Mage Knight](https://ludopedia.com.br/jogo/mage-knight-ultimate-edition)

## Utilização

Acesse `http://neni.dev/mk`

## Requisitos do projeto

- [x] Conteúdo deve ser publicável
- [x] Conteúdo deve ser pesquisável
- [x] Conteúdo deve referenciar facilmente durante a criação e leitura ao conteúdo oficial
- [x] A plataforma deve permitir um link fácil para sugestão de melhorias
- [x] Pesquisabilidade

### Justificativa da stack

[Quartz](https://quartz.jzhao.xyz) traz facilidade na leitura por emular a utilização do [Obsidian](https://obsidian.md/).

Benefícios a mais dos requisitos obtidos com a stack:
- Tema escuro e claro
- Facilidade e gratuidade no deploy
- Mapa conceitual de *backlinks* navegável

Outras possibilidades de stack:
- [Amethyst](https://amethyst.bencuan.me): Semelhante ao [Quartz](https://quartz.jzhao.xyz) porém feito com [Hugo](https://gohugo.io/)
- Desenvolver o próprio tema com [Hugo](https://gohugo.io/)

## Como posso contribuir

É um processo longo de escrita e revisão de texto, adicionando links incrementalmente. Faça um PR com suas sugestão.

## Desenvolvimento

### Configuração

```sh
npm i
```

### Execução

1. Subir o servidor
```sh
npx quartz build --serve
```

2. Abro um *vault* do Obsidian diretamente na pasta [content](/content)

### Deploy

```sh
npx quartz sync
```
