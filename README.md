# MK

Instruções referenciadas do jogo [Mage Knight](https://ludopedia.com.br/jogo/mage-knight-ultimate-edition). Nesse projeto está somente a camada de visualização, o conteúdo está no projeto [man-mk](https://github.com/neninja/man-mk) e por lá que será versionado.

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
> Apesar de ter um search mobile melhor, ele tem problemas com ids do obsidian `^blabla` e nomes de arquivos no mapa conceitual que requerem utf-8, como `Preparação`
- Desenvolver o próprio tema com [Hugo](https://gohugo.io/)

## Como posso contribuir

É um processo longo de escrita e revisão de texto, adicionando links incrementalmente. Faça um PR com suas sugestão.

## Desenvolvimento

### Configuração

```sh
npm i
```

### Execução

```sh
npx quartz build --serve
```

### Atualização de conteúdo

O conteúdo está versionado no projeto [man-mk](https://github.com/neninja/man-mk) para tornar o versionamento mais específico, ao invés de detalhes de implementação da aplicação. Dessa forma é utilizado o recurso de submodulo do git. Para atualizar o submodulo desse projeto, use o comando abaixo

```sh
git submodule update --init --recursive
```

### Deploy

```sh
npx quartz sync
```
