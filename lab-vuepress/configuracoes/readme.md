# Lab VuePress - Configurações

A configuração do VuePress é feita catravés do arquivo `config.yml` ou `confic.js` na pasta `.vuepress`. 

## config.yml

Configuração feita em YAML.

```yml
title: Documentação do Lab VuePress
themeConfig:
  nav:
  - text: Início
    link: "/"
  - text: VuePress
    link: https://vuepress.vuejs.org
  - text: Outros Links
    items:
    - text: VuePress Guide
      link: https://vuepress.vuejs.org/guide
    - text: VuePress Config
      link: https://vuepress.vuejs.org/config
    - text: VuePress Default Theme Config
      link: https://vuepress.vuejs.org/default-theme-config
    - text: VuePress GitHub
      link: https://github.com/vuejs/vuepress
  sidebar:
  - "/"
  - "/configuracoes/"
```

## config.js

A mesma configuração feita em JavaScript.

```js
module.exports = {
  title: 'Documentação do Lab VuePress',
  themeConfig: {
    nav: [
      {
        text: 'Início',
        link: '/',
      },
      {
        text: 'VuePress',
        link: 'https://vuepress.vuejs.org'
      },
      {
        text: 'Outros Links',
        items: [
          { text: 'VuePress Guide', link: 'https://vuepress.vuejs.org/guide' },
          { text: 'VuePress Config', link: 'https://vuepress.vuejs.org/config' },
          { text: 'VuePress Default Theme Config', link: 'https://vuepress.vuejs.org/default-theme-config' },
          { text: 'VuePress GitHub', link: 'https://github.com/vuejs/vuepress' }
        ]
      }
    ],
    sidebar: [
      '/',
      '/configuracoes/'
    ]
  }
}
```