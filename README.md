# TVF ProRes — Landing Page

Landing page do curso TVF ProRes.

## Deploy no Vercel

1. Faça push deste repositório para o GitHub
2. Acesse [vercel.com](https://vercel.com)
3. Clique em **Add New Project**
4. Importe o repositório do GitHub
5. Clique em **Deploy** — sem configuração adicional necessária

## Estrutura

```
tvf-prores/
├── index.html      ← página completa (HTML + CSS + JS inline)
├── vercel.json     ← configuração do Vercel
├── .gitignore
└── README.md
```

## Atualizar a data de fechamento do carrinho

No `index.html`, localize a linha:

```js
const end = new Date('2026-06-10T23:59:59-03:00');
```

Troque a data conforme necessário.

## Link de compra

O botão de compra aponta para:
`https://pay.kiwify.com.br/b43kYhK`

Para alterar, busque essa URL no `index.html` e substitua.
